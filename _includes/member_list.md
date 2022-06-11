<div style="clear:both">
{% for member in include.members.current %}
<article class="grid__item members">
        {% if member.picture %}
        <img src="{{ member.picture }}" alt="Profile picture">
        {% else %}
        <img src="/assets/images/people/placeholder.png" alt="Profile picture">
        {% endif %}
        <h2 class="archive__item-title" itemprop="headline">
        {% if member.url %}
        <a href="{{ member.url }}" rel="permalink">{{ member.name }}</a>
        {% else %}
        {{ member.name }}
        {% endif %}
        </h2>
        <p class="archive__item-excerpt" itemprop="description">{{ member.position }}</p>
</article>
{% endfor %}
</div>
<h2> Past Members </h2>
<div style="clear:both;">
{% for member in include.members.past %}
<article class="grid__item members">
        {% if member.picture %}
        <img src="{{ member.picture }}" alt="Profile picture">
        {% else %}
        <img src="/assets/images/people/placeholder.png" alt="Profile picture">
        {% endif %}
        <h2 class="archive__item-title" itemprop="headline">
        {% if member.url %}
        <a href="{{ member.url }}" rel="permalink">{{ member.name }}</a>
        {% else %}
        {{ member.name }}
        {% endif %}
        </h2>
        <p class="archive__item-excerpt" itemprop="description">{{ member.position }}</p>
</article>
{% endfor %}
</div>
