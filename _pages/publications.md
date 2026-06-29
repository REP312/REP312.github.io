---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<style>
  .publications .abbr abbr,
  .publications .abbr abbr * {
    color: #fff !important;
  }

  .publications ol.bibliography li > .row > div[id] {
    display: grid;
    grid-template-columns: max-content minmax(0, 1fr);
    column-gap: 0.35rem;
  }

  .publications ol.bibliography li > .row > div[id] > * {
    grid-column: 2;
  }

  .publications ol.bibliography li > .row > div[id] > .publication-sequence {
    grid-column: 1;
    grid-row: 1;
    align-self: start;
    font-weight: 700;
  }

  .publications ol.bibliography li > .row > div[id] > .title {
    grid-column: 2;
    grid-row: 1;
  }

  .publications .publication-sequence-journal {
    color: #3f6fc1;
  }

  .publications .publication-sequence-conference {
    color: #2f7d4f;
  }

  html[data-theme="dark"] .publications .publication-sequence-journal {
    color: #7fa2dc;
  }

  html[data-theme="dark"] .publications .publication-sequence-conference {
    color: #75b58b;
  }
</style>

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
