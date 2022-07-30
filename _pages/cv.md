---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======

* B.S. Biomedical Engineering (cell and tissue engineering), University of Rochester, 2017 (T5)
* M.Phil. Chemical and Process Engineering, University of Strathclyde, 2019
* Ph.D. Environmental Engineering, Pennsylvannia State University, 2023 (expected)

Publications
======

  <ul>{% for post in site.publications reversed limit:2 %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

[More here](https://jkboualavong.github.io/publications/)

Work Experience
======

Pennsylvania State University
--------------

07/2019: Science U: Water Heroes

University of Strathclyde
--------------

01/2018-05/’18: Society of Chemical Industry Electrochemistry Postgraduate Conference Committee

10/2017-08/’19: Really Small Science Group


University of Rochester
--------------

08/2015-05/’17: Biomedical Engineering Peer Advisor (through College Center for Advising Services)

Other Research Experience
======

Pacific Northwest National Laboratory
--------------

06-08/2016: Science Undergraduate Laboratory Internship (SULI) program
* PIs: Brady Lee, Hope Lee (Pacific Northwest National Laboratory)
* Microbially induced calcite precipitation for bioremediation of I-129 in the Hanford Site subsurface
  * rate analysis using two model bacteria
  * phylogenetic characterization of Hanford Site enrichments

Colorado State University
--------------

05-07/2015: NSF REU: Colorado Center for Biorefining and Bioproducts
* PI: Shantanu Jathar (Mech. Eng.) and Charles Henry (Chem.)
* A Microfluidic Electrochemical Sensor for the Oxidative Load of Particulate Matter
  * sensor characterization and optimization
  * assessment of diesel vs biodiesel combustion particulates


Talks
======
{% assign posts = site.talks | reverse %}
{% assign counter = 0 %}
{% for post in posts limit:1 %}
    {% include card.html post=post %}
{% endfor %}


{% assign posts = site.talks | reverse %}
{% assign counter = 0 %}
{% for post in posts %}
  {% if counter < 3 and post.categories contains 'featured' and post.path != page.path %}
    {% include card.html post=post %}
    {% assign counter = counter | plus: 1 %}
  {% endif %}
{% endfor %}

  <ul>{% for post in site.talks limit:1 reversed %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>

[More here](https://jkboualavong.github.io/talks/)
  
Teaching
======

  <ul>{% for post in site.teaching limit:1 reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
[More here](https://jkboualavong.github.io/teaching/)

