---
layout: page
title: Research
ord: 20
permalink: /research/
description:
nav: true
display_categories: # [work, fun]
horizontal: false
---
<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:1rem;">
  Dissertation
</h1>
Description forthcoming.

<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:1rem;">
  Hebrew t-sibilant sequences
</h1>
<h2 style="font-size:16px;font-weight:400;margin-top:0.67em;padding-top:-5px;padding-bottom:0.5rem;">
  Collaborator(s): Lily Xu
</h2>
Sequences of [t] followed by a sibilant in Hebrew are overall underattested yet only actively repaired via metathesis in very specific morphological environments. We are interested in the role of morphology in constraining the well-formedness of such sequences and the application of the metathesis process in Hebrew speakers' grammars. 

We presented the results of a phonotactics judgement study at the MFM. We are currently using formal modelling to explore how such division in grammars might arise. We are also running a wug test on the same pattern. 


<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:1rem;">
  Acquisition of non-local phonotactic dependencies
</h1>
<h2 style="font-size:16px;font-weight:400;margin-top:0.67em;padding-top:-5px;padding-bottom:0.5rem;">
  Collaborator(s): Megha Sundara
</h2>

Sundara et al.'s (2022) [meta-analysis on phonotactic acquisition](https://doi.org/10.1016/j.cognition.2021.104993) found that infants display sensitivity to vowel harmony before any other local or non-local phonotactic dependency. This is despite the fact that non-local dependencies are reportedly more difficult to learn than local dependencies. We are currently planning a series of experiments to investigate two main questions:
<ol>
  <li>Is the early sensitivity that infants display for VH due to its perceptual saliency?</li>
  <li>Does experience with VH facilitate infants' learning of more arbitrary non-local dependencies?</li>
</ol>



<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:2rem;">
  Non-concatenative morphological priming in Semitic languages
  </h1>
<h2 style="font-size:16px;font-weight:400;margin-top:0.67em;padding-top:-5px;padding-bottom:0.5rem;">
  Collaborator(s): Lily Xu, Huilei Wang, & Megha Sundara
</h2>

We are using Bayesian meta-analysis to investigate morphological priming effects in Arabic and Hebrew. Semitic languages are well-known for their extensive non-concatenative "root-template" morphology; most Semitic words can be decomposed into a consonantal root carrying the main lexical semantics and a prosodic template associated with morphosyntactic information. We are using the aggregate data points to look at the status of root and template morphology in the adult grammar.
<br>
* [You can find a list of papers included in the meta-analysis on osf](https://osf.io/2wr5t/?view_only=69f72c59060640d9a5309fb75f6ed983)


<!-- <br>
<hr width="50%" size="8" align="left">
Other linguists who work or have done work on Lachirioag Zapotec include: <br>
* Madeleine Booth (UCLA)<br>
* Michael Galant (UC Dominguez Hills)<br>
* [Harold Torrence](https://linguistics.ucla.edu/person/harold-torrence/) (UCLA)<br>
* [Pamela Munro](https://linguistics.ucla.edu/person/pamela-munro/) (UCLA)

There have also been community efforts to document and create language materials. A page with a collection of Zapotec resources is upcoming. -->
<br>
#### <b>Fieldwork on Lachirioag Zapotec</b>
***

<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:1rem;padding-bottom:0.5rem;">
  Verbal prefixes
</h1>

My [MA thesis](https://www.proquest.com/pagepdf/2611991924?accountid=14512) provided a general description of the verbal morphology found in Lachirioag Zapotec, with a particular focus on the verbal TAM prefixes and the argument enclitics. Currently, I am continuing my investigation into the verbal prefixes with focus on two main questions:
<ol>
  <li>What conditions the allomorphy displayed by the irrealis and perfective prefixes?</li>
  <li>What is the semantic information conveyed by the TAM prefixes?</li>
</ol>

<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:2rem;">
  The fortis/lenis contrast and fortition processes
</h1>
<h2 style="font-size:16px;font-weight:400;margin-top:0.67em;padding-top:-5px;padding-bottom:0.5rem;">
  Collaborator(s): Lily Xu
</h2>

Zapotec languages are described as having a fortis/lenis contrast for both obstruent and sonorant consonants. Despite the name, the two classes of consonants have been found to be primarily distinguished by duration in other Zapotec languages. Our <a href="/assets/pdf/ssila22_SCLZfortislenis.pdf" target="_new">preliminary results</a> support the previous findings, and additionally find voicing to be a significant acoustic correlate for obstruents. We are currently gathering more data, and hope that our results will provide us a better understanding of how the fortis/lenis contrast in Zapotec fits in the larger typology of laryngeal contrasts.

<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:2rem;">
  Other
</h1>
Description forthcoming.



<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
