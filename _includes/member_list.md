<div>
{% for member in include.members %}
<div class="grid__item members">
        {% if member.picture %}
        <img src="{{ member.picture }}" alt="Profile picture" class="portrait" >
        {% else %}
        <img src="/assets/images/people/placeholder.png" alt="Profile picture" class="portrait" >
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
