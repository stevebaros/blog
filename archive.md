---
layout: page
title: Archive
---

<section class="archive-post-list">
   {% capture now %}{{'now' | date: '%s' | plus: 0}}{% endcapture %}  
   {% for post in site.posts %}
        {% capture date %}{{post.date | date: '%s' | plus: 0}}{% endcapture %}
        {% if date <= now %}
            {% assign currentDate = post.date | date: "%Y" %}
            {% if currentDate != myDate %}
                 <!-- {% unless forloop.first %}</ul>{% endunless %} -->

                <h1>{{ currentDate }}</h1>
                <ul>
                {% assign myDate = currentDate %}
            {% endif %}
            <li><a href="{{ post.url }}"><span>{{ post.date | date: "%B %-d, %Y" }}</span> - {{ post.title }}</a></li>
            {% if forloop.last %}</ul>{% endif %}
        {% endif %}
   {% endfor %}

</section>