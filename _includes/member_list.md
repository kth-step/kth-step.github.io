<div>
{% for member in include.members.current %}
<div class="grid__item members">
        {% if member.picture %}
        <img src="{{ member.picture }}" alt="Profile picture">
        {% else %}
        <img src="/assets/images/people/placeholder.png" alt="Profile picture">
        {% endif %}
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
<h2 style="clear:both;"> Past Members </h2>
<div>
{% for member in include.members.past %}
<div class="grid__item members">
        {% if member.picture %}
        <img src="{{ member.picture }}" alt="Profile picture">
        {% else %}
        <img src="/assets/images/people/placeholder.png" alt="Profile picture">
        {% endif %}
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
