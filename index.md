---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

<section class="food">
  <div class="fooditem">
    {% for item in site.data.foods %}
  <ul>
    {% for food in item.foods %}
    <li>
      <a href="{{food.url}}">
        <div class="img">
          <img width="400" height="400" src="{{food.img}}" alt="{{food.detail}}">
          <p>{{food.detail}}</p>
        </div>
      </a>
    </li>
    {% endfor %}
  </ul>
  {% endfor %}
  </div>
