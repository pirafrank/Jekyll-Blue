---
layout: redirect
title: twitter
permalink: /twitter/
show_title: false
---

{% if site.social-links.twitter %}

<META HTTP-EQUIV="Refresh"
CONTENT="0; URL="http://twitter.com/{{ site.social-links.twitter }}">

{% else %}

<META HTTP-EQUIV="Refresh"
CONTENT="0; URL="{{ site.baseurl }}">

{% endif %}