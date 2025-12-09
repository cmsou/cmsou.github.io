---
layout: archive
permalink: /talks/
title: Talks and posters
author_profile: true
toc: true
---

{% include toc %}

# Talk map

<p style="text-decoration:none;"> See a map of all the places I've given a talk! </p>
<iframe src="talkmap/map.html" width="100%" height="500px"></iframe>





{% if site.talkmap_link == true %}

<p style="text-decoration:underline;"><a href="/talkmap.html">See a map of all the places I've given a talk!</a></p>

{% endif %}



---


# Conference and workshop talks 
{% for post in site.talks reversed %}
  {% if post.type <> "Seminar talk" %}
    {% include archive-single-talk-cv.html %}
  {% endif %}
{% endfor %}

---

# Seminar talks 
{% for post in site.talks reversed %}
  {% if post.type == "Seminar talk" %}
    {% include archive-single-talk-cv.html %}
  {% endif %}
{% endfor %}

---

# Posters 
{% for post in site.posters reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}