---
layout: page
title: research
permalink: /research/
description:
nav: true
nav_order: 1
---

In my research, I aim to uncover the general principles that restrict how syntactic structures can be built and interpreted in natural languages, and why these principles should hold. Most of my research uses structures with clausal embedding as a lens through which to investigate such principles. Two other prominent empirical areas of my research are complex agreement systems and discontinuous phrases. Here are the main theoretical questions that drive my research:

1. What kinds of meanings are associated with the syntactic elements responsible for clausal embedding, and what is the role of these elements in modal displacement?
2. What argument and event structures can clause-embedding verbs have, and how do they affect selection and interpretations of embedded clauses and cross-clausal dependencies?
3. What is the role of semantic triviality in restrictions on clausal embedding?
4. Why do locality restrictions on syntactic dependencies arise, and how are they affected by the syntax and semantics of embedded clauses?
5. How do languages deal with surplus of syntactic features, and what can this tell us about interactions between Vocabulary Insertion and operations in the narrow syntax?
6. What gives rise to discontinuous spell-out of certain constituents? Is it a product of true syntactic sub-extraction, or a PF phenomenon, and what principles constrain it?

In answering these questions, I search for new phenomena and robust empirical generalizations that can better inform our theories, and thus fieldwork is a major component of my research process. 

Besides theoretical linguistics, I am interested in documentation and preservation of understudied languages. I believe that this work is critical in the present moment, when [about 44% of the world's languages are endangered](https://www.ethnologue.com/insights/how-many-languages-endangered/). Together with the members of [my lab](/lab/), I seek to collaborate with indigenous communities on language projects that contribute to preservation of linguistic and cultural diversity in the world. Since 2024, my lab has been colloborating with the [Alabama-Coushatta Tribe of Texas](https://www.alabama-coushatta.com/) on language documentation and preservation of the Alabama language (Muskogean family).




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
