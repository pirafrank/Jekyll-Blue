---
layout: page
title: About
permalink: /about/
show_title: false
---

<!-- trailing slash in permalink is needed -->

Some information about you!

### More Information

A place to include any other types of information that you'd like to include about yourself.

### Portfolio

Include here your portfolio.

### Contact me

{% if site.encryptedemail %}
<div class="safe-email">
    <a href="mailto:{{ site.encryptedemail }}" onclick="this.href=this.href.replace(/ /g,'')">{{ site.encryptedemail }}</a>
</div>
{% elsif site.social-links.email %}
<a href="mailto:{{ site.social-links.email }}">{{ site.social-links.email }}</a>
{% endif %}

### Credits

Created with Jekyll Blue.