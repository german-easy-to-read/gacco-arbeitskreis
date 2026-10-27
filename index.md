---
layout: single
permalink: /
title: "Arbeitskreis German Accessible Communication (GACCO)"
author_profile: false
toc: true
toc_label: "Inhalt"
toc_sticky: true
---

## Über den Arbeitskreis

Unser Arbeitskreis beschäftigt sich mit allen Formen der barrierefreien Kommunikation im Deutschen, bspw. Leichter und Einfache Sprache, und versucht deren Sichtbarkeit in der Deutschen Forschung zu stärken.


## Ziele

- Interdisziplinäre Vernetzung zwischen Forschenden der Computerlinguistik, Bildungswissenschaften und barrierefreier Kommunikation
- Erstellung von Ressourcen und Tools für die automatische Textvereinfachung im Deutschen, einschließlich Parallelkorpora und Benchmarks für Leichte Sprache und Einfache Sprache
- Entwicklung und Evaluation von Verständlichkeitsmetriken für das Deutsche, auch jenseits klassischer Maße (z. B. Flesch-Lesbarkeitsindex)
- Organisation von Workshops und Shared Tasks zu Textvereinfachung, Lesbarkeitsanalyse und verwandten Aufgaben, vor allem unseres [https://klar-text.github.io/](KlarTexts Workshops auf der KONVENS).
- Wissensaustausch zur Zielgruppenintegration, etwa durch Nutzerstudien, Eye-Tracking und kognitive Belastungsmessung


## Mitglieder

| Name | Institution |
| ---- | ----------- |
| Miriam Anschütz | Universität Heidelberg |
| Yingqiang Gao | ETH Zürich |
| Regina Stodden | Universität Bielefeld |
| Thorben Schomacker | HAW Hamburg & Universität Hamburg |


## Kontakt

Du hast Interesse an unserem Arbeitskreis oder eine Frage? Dann ["mailto:yingqiang.gao@uzh.ch?cc=miriam.anschuetz@iued.uni-heidelberg.de.de,regina.stodden@uni-bielefeld.de,Thorben.Schomacker@haw-hamburg.de&subject=GACCO"](melde dich beim Orga-Team)!

## Aktuelles

{% if site.posts.size > 0 %}
{% for post in site.posts limit: 3 %}
- **{{ post.date | date: "%d.%m.%Y" }}** – [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

[Alle News]({{ "/news/" | relative_url }}){: .btn .btn--primary}
{% else %}
Derzeit gibt es keine Neuigkeiten.
{% endif %}
