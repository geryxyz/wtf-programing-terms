---
layout: archive
---

{% assign terms = site.pages | sort: 'title' %}
{% for page in terms %}
    {% if page.term == true %}
        <p class="notice">
            <strong>{{ page.title }}</strong> (<a href="{{ page.url }}">{{ page.short }}</a>) {{ page.motto }}
        </p>
    {% endif %}
{% endfor %}