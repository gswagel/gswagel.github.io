---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[<i class="fas fa-file-pdf"></i> Download my CV (PDF)](/files/gabriel-swagel-cv.pdf){: .btn .btn--info}

Education
======
* Ph.D. in Economics, Princeton University (in progress)

Publications
======
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
