---
layout: page
title: Markdown DataTables Demo
subtitle: Excerpt from Soulshaping Sial Simthu by TTonsing
cover-img: assets/img/path.jpg
thumbnail-img: assets/img/thumb.png
share-img: assets/img/path.jpg
tags: [keimah, Sial Simthu]
date: 2021-12-09
---
(setq markdown-css-paths '("https://cdn.datatables.net/1.10.21/css/jquery.dataTables.min.css"))
(setq markdown-css-paths '("https://cdn.datatables.net/1.10.21/css/jquery.dataTables.min.css"))
(setq markdown-css-paths '("https://code.jquery.com/jquery-3.5.1.js"))
(setq markdown-css-paths '("https://cdn.datatables.net/1.10.21/js/jquery.dataTables.min.js"))

<h1>Datatables Markdown Demo</h1>

<p>
  Based on <a href="https://idratherbewriting.com/documentation-theme-jekyll/mydoc_tables.html#jquery-datatables">tutorial</a> for Jekyll.
</p>

Steps:

1. Add datatables CSS
    [https://cdn.datatables.net/1.10.21/css/jquery.dataTables.min.css](https://cdn.datatables.net/1.10.21/css/jquery.dataTables.min.css)
1. Add any custom CSS, like font-family
1. Add jQuery JS
    [https://code.jquery.com/jquery-3.5.1.js](https://code.jquery.com/jquery-3.5.1.js)
1. Add jQuery datatable JS
    [https://cdn.datatables.net/1.10.21/js/jquery.dataTables.min.js](https://cdn.datatables.net/1.10.21/js/jquery.dataTables.min.js)
1. Add table (HTML, or Markdown with pre-processor). No special class is needed, you just need to reference your table next.
1. Add JS snippet to run jQuery DataTable setup your table.

You datatable will be generated. It will include an entries limit (default 10), a search bar, sorting and pagination.

<br>

<div id="my-table">

<!-- The pre-processor for this pen is set to Markdown   -->

| Food    | Description                           | Category | Sample type |
| ------- | ------------------------------------- | -------- | ----------- |
| Apples  | A small, somewhat round ...           | Fruit    | Fuji        |
| Bananas | A long and curved, often-yellow ...   | Fruit    | Snow        |
| Kiwis   | A small, hairy-skinned sweet ...      | Fruit    | Golden      |
| Oranges | A spherical, orange-colored sweet ... | Fruit    | Navel       |

</div>
// Must reference the table inside the div, not the div itself,
// as the div is not a table and you'll get an error from jQuery.
//
// If you had an HTML table and not a markdown one, you could setup <table id="my-table"> and reference with $("#my-table").  
  <script>
$(document).ready(function () {
  $("#my-table > table").DataTable();
});
  </script>
