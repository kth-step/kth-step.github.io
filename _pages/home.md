---
title: "Home"
permalink: /
layout: single
---
Welcome to the Secure and Trustworthy Execution Platforms (STEP) group at KTH!

You can access thesis and publications in the dedicated [Publications page](/publications).
{: .notice}

<h2>News</h2>
<!-- Get 10 latest news -->
{% assign news = site.data.news.news | slice: 0, 10 %}
<!-- Print the news -->
<dl class="news">
{% for item in news %}
        <dt>{{ item.date }}</dt>
        <dd> {{ item.text |  markdownify }} </dd>
{% endfor %}
</dl>

