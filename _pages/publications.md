---
layout: page
permalink: /publications/
title: publications
description: Journal articles and work under review.
nav: true
nav_order: 2
---

{% comment %} Sections are filled from _bibliography/papers.bib by entry type:
     article = journal articles, misc = preprints, unpublished = under review {% endcomment %}

<div class="publications">

<h2 class="bibliography">Journal articles</h2>
{% bibliography --query @article --group_by none %}

{% comment %} Preprints section hidden for now (Nov 2026). To restore, delete the comment tags around it
  and move the entry from _on_hold/preprint.bib back into papers.bib.
<h2 class="bibliography">Preprints</h2>
{% bibliography --query @misc --group_by none %}
{% endcomment %}

<h2 class="bibliography">Under review</h2>
{% bibliography --query @unpublished --group_by none %}

</div>

A current list is also on [Google Scholar](https://scholar.google.com/citations?user=1xvO34gAAAAJ).
