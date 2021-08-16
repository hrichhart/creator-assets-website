---
layout: page
permalink: /search
title: Search
description: noindex
---

<!-- Html Elements for Search -->
<input type="text" id="search-input" placeholder="Search blog posts..">
<ul id="results-container"></ul>
<script src="https://unpkg.com/simple-jekyll-search@latest/dest/simple-jekyll-search.min.js"></script>
<!-- Configuration -->
<script>
var sjs = SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/assets/article-data.json'
})
</script>