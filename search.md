---
layout: page
title: Search
subtitle: Find what you are looking for...
use-site-title: true
show-avatar: false
css: /css/search.css

---

For now, searching is done through a Google search function customized for this site. It comes
with ads, which is not great, but that keeps it free.

<div id="google-custom-search">
<script>
  (function() {
    var cx = '008751022318489805044:9afylpxpz4g';
    var gcse = document.createElement('script');
    gcse.type = 'text/javascript';
    gcse.async = true;
    gcse.src = 'https://cse.google.com/cse.js?cx=' + cx;
    var s = document.getElementsByTagName('script')[0];
    s.parentNode.insertBefore(gcse, s);
  })();
</script>
<gcse:searchbox></gcse:searchbox>
<gcse:searchresults></gcse:searchresults>
</div>