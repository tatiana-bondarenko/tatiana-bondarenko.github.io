---
layout: page
title: research
permalink: /research/
description:
nav: true
nav_order: 1
---

In my research, I aim to uncover the general principles that restrict how  syntactic structures can be built and interpreted in natural languages, and why these principles should hold. I often use structures with clausal embedding as a lens through which to investigate such principles across a variety of research topics in syntax and semantics. Another component of my research is to understand how the syntactic structures that we build can be externalized\----what rules govern their linearization and exponence. In answering the questions above, I search for new phenomena and robust empirical generalizations that can better inform our theories, and thus fieldwork is a major component of my research process. 

Besides theoretical linguistics, I am interested in documentation and preservation of understudied languages. I believe that this work is critical in the present moment, when [about 42% of the world's languages are endangered](https://www.ethnologue.com/insights/how-many-languages-endangered/). Together with the members of [my lab](https://fieldlinguistics.github.io/), I seek to collaborate with indigenous communities on language projects that contribute to preservation of linguistic and cultural diversity in the world. Since 2024, my lab has been colloborating with the [Alabama-Coushatta Tribe of Texas](https://www.alabama-coushatta.com/) on language documentation and preservation of the Alabama language (Muskogean family).




<div class="projects">

{% assign research_projects = site.projects | where: "category", "research" | sort: "importance" %}

{% for project in research_projects %}

<div style="margin-bottom: 3rem;">

  <h2>{{ project.title }}</h2>

  {% if project.img %}
    <img
      src="{{ project.img | relative_url }}"
      alt="{{ project.title }}"
      style="max-width: 500px; width: 100%; margin-bottom: 1rem;"
    >
  {% endif %}

  {{ project.content }}

</div>

{% endfor %}

</div>
