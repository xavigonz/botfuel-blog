---
title: 'Post: Image (Caption)'
date: 2010-08-07 00:00:00 -04:00
categories:
- Post Formats
tags:
- image
- Post Formats
---

{% capture fig_img %}
![Foo]({{ "/assets/images/unsplash-gallery-image-3.jpg" | absolute_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo from Unsplash.</figcaption>
</figure>