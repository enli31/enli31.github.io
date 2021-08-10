---
layout: page
title: 搜索
---

<!-- HTML elements for search -->
<input type="text" id="search-input" placeholder="搜索信息-输入标题/相关内容.." style="width:480px;"/>
<ul id="results-container"></ul>

<!-- script pointing to jekyll-search.js -->
<script src="/js/simple-jekyll-search.min.js"></script>

<script>
SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    json: '/search.json',
    searchResultTemplate: '<li><a href="{url}" title="{desc}">{title}</a></li>',
    noResultsText: '对不起，没有搜索到此内容',
    limit: 20,
    fuzzy: false
  })
</script>