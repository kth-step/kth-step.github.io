<div>
{% for member in include.members %}
<div class="grid__item members">
        {% if member.picture %}
        <img class="archive__item-teaser" src="{{ member.picture }}" alt="Profile picture">
        {% else %}
        <img class="archive__item-teaser" src="/assets/images/people/placeholder.png" alt="Profile picture">
        {% endif %}
        <br/>
        <b>
        {% if member.url %}
        <a href="{{ member.url }}" rel="permalink">{{ member.name }}</a>
        {% else %}
        {{ member.name }}
        {% endif %}
        </b><br/>
        {{ member.position }}
</div>
{% endfor %}
</div>
