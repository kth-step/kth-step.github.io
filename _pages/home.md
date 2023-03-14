---
title: "Secure and Trustworthy Execution Platforms"
permalink: /
layout: single
---
Welcome to the Secure and Trustworthy Execution Platforms (STEP) group at KTH!

You can access thesis and publications in the dedicated [Publications page](/publications).

<hr/>
<h1>News</h1>
<!-- Get 10 latest news -->
{% assign news = site.data.news.news | slice: 0, 7 %}
<!-- Print the news -->
<div style="font-size:80%">
<dl class="news">
{% for item in news %}
        <dt>{{ item.title }} </dt>
        <dd> {{ item.text |  markdownify }} <p style="text-align: right;">{{ item.date }}</p></dd>
{% endfor %}
</dl>
</div>

