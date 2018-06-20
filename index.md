---
title: Fran Fabrizio's Blog
---

Welcome to my blog. I blog on a few different topics, so I've organized this blog into categories.

<ul class="taxonomy-index">
  {% assign categories_max = 0 %}
  {% for category in site.categories.sort %}
    {% if category[1].size > categories_max %}
      {% assign categories_max = category[1].size %}
    {% endif %}
  {% endfor %}
  {% for i in (1..categories_max) reversed %}
    {% for category in site.categories %}
      {% if category[1].size == i %}
        <li>
          <a href="/{{ category[0] | slugify }}">
            <strong>{{ category[0] }}</strong> <span class="taxonomy-count">{{ i }}</span>
          </a>
        </li>
      {% endif %}
    {% endfor %}
  {% endfor %}
</ul>

# Latest Post from Each Category

{% for category in site.categories %}
  <section id="{{ category[0] | slugify | downcase }}" class="taxonomy-section">
    <h2 class="taxonomy-title">{{ category[0] }}</h2>
    <div class="entries-{{ page.entries_layout | default: 'list' }}">
      {% for post in category.last limit:1%}
        {% include entry.html %}
      {% endfor %}
    </div>
  </section>
{% endfor %}

Done.
