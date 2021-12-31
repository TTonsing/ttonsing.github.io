                 

{% include header.html type="page" %}

[Back Home](/)
==============

The Movie Database
==================

Sl.No

Movie Name

Description

Rating

Review

Link

Sl.No

Movie Name

Description

Rating

Review

Link

$(document).ready(function() { $('#example').DataTable( { /\*"ajax": '../ajax/data/arrays.txt' \*/ //"ajax": 'ajax/data/arrays.txt' "ajax": 'movie1.txt', "order":\[1,'asc'\], //"lengthMenu": \[\[10, 25, 50, -1\], \[10, 25, 50, "All"\]\], //"lengthMenu": \[\[10\], \[10\]\] } ); } );

© 2021 GitHub, Inc. Terms
