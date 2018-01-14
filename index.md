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
    {% for project in item.foods %}
    <li>
      <a href="{{project.url}}">
        <div class="img">
          <img width="384" src="{{project.img}}" alt="{{project.details}}">
          <p>{{project.details}}</p>
        </div>
      </a>
    </li>
    {% endfor %}
  </ul>
  {% endfor %}
  </div>
