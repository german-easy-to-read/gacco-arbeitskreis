---
layout: single
permalink: /en/
ref: home
title: "Working Group German Accessible Communication (GACCO)"
excerpt: >-
  The working group German Accessible Communication (GACCO) connects
  researchers and practitioners in the field of accessible communication
  in German-speaking countries.
author_profile: false
toc: true
toc_label: "Contents"
toc_sticky: true
---

## About the Working Group

Our working group works with all forms of accessible communication in German, such as Easy Language (Leichte Sprache) and Plain Language (Einfache Sprache), and aims to strengthen their visibility in German research.

Our work is supported by the [German Society for Computational Linguistics and Language Technology (GSCL)](https://gscl.org/).


## Goals

- Interdisciplinary networking between researchers in computational linguistics, educational sciences and accessible communication
- Creating resources and tools for automatic text simplification in German, including parallel corpora and benchmarks for Easy Language and Plain Language
- Developing and evaluating comprehensibility metrics for German, also beyond classical measures (e.g. the Flesch Reading Ease)
- Organising workshops and shared tasks on text simplification, readability assessment and related tasks, above all our [KlarText workshop at KONVENS](https://klar-text.github.io/)
- Exchanging knowledge on involving target groups, e.g. through user studies, eye tracking and cognitive load measurement


## Members

| Name | Institution |
| ---- | ----------- |
| Miriam Anschütz | Heidelberg University |
| Yingqiang Gao | ETH Zurich |
| Regina Stodden | Bielefeld University |
| Thorben Schomacker | HAW Hamburg & University of Hamburg |


## Contact

Are you interested in our working group or do you have a question? Then [get in touch with the organising team](mailto:yingqiang.gao@uzh.ch?cc=miriam.anschuetz@iued.uni-heidelberg.de,regina.stodden@uni-bielefeld.de,Thorben.Schomacker@haw-hamburg.de&subject=GACCO)!

## News

{% assign posts = site.posts | where: "lang", "en" %}
{% if posts.size > 0 %}
{% for post in posts limit: 3 %}
- **{{ post.date | date: "%Y-%m-%d" }}** – [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

[All news]({{ "/en/news/" | relative_url }}){: .btn .btn--primary}
{% else %}
There is no news at the moment.
{% endif %}
