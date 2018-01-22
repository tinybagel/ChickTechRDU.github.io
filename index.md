---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

<section class="food">
  <div class="fooditem">
  <ul>
    {% for post in site.posts %}
    <li>
      <a href="{{site.baseurl}}{{post.url}}">
        <div class="img">
          <img width="400" height="400" src="{{post.img}}" alt="{{post.detail}}">
          <p>{{post.detail}}</p>
        </div>
      </a>
    </li>
    {% endfor %}
  </ul>
  </div>
