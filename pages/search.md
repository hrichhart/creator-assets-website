---
layout: search
permalink: /search
title: Search
description: noindex
noAds: true
---

<!-- Html Elements for Search -->
<input type="text" id="search-input" placeholder="Search for assets...">
<ul id="results-container"></ul>

<script src="/assets/js/jekyll-search.js"></script>

<!-- Configuration -->
<script>
var sjs = SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/assets/article-data.json'
})
</script>