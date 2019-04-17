{"template":"component.html","title":"Pagination","demo":"<h4>Basic</h4>\r\n\r\n<!-- START: FIRSTDEMO -->\n\r\n<script>\r\n  var $demoOutput;\r\n\r\n  Formstone.Ready(function() {\r\n    $demoOutput = $(\".demo_output\");\r\n\r\n    $(\".demo_pagination\").on(\"update.pagination\", function(e, page) {\r\n      $demoOutput.prepend('<strong>Index: </strong>' + page + '</span><br>');\r\n    });\r\n  });\r\n</script>\r\n\r\n<div class=\"demo_container\">\r\n  <div class=\"demo_example\">\r\n    <nav class=\"js-pagination demo_pagination\">\r\n      <a href=\"#1\">1</a>\r\n      <a href=\"#2\">2</a>\r\n      <a href=\"#3\">3</a>\r\n      <a href=\"#4\">4</a>\r\n      <a href=\"#5\">5</a>\r\n      <a href=\"#6\">6</a>\r\n      <a href=\"#7\">7</a>\r\n      <a href=\"#8\">8</a>\r\n      <a href=\"#9\">9</a>\r\n      <a href=\"#10\">10</a>\r\n    </nav>\r\n    <div class=\"demo_output form_textarea\"></div>\r\n  </div>\r\n  <div class=\"demo_code\">\r\n    <pre><code class=\"language-html\">&lt;nav class=&quot;pagination&quot;&gt;\r\n&Tab;&lt;a href=&quot;1.html&quot;&gt;1&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;2.html&quot;&gt;2&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;3.html&quot;&gt;3&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;4.html&quot;&gt;4&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;5.html&quot;&gt;5&lt;/a&gt;\r\n&lt;/nav&gt;</code></pre>\r\n    <pre><code class=\"language-javascript\">$(\".pagination\").pagination();</code></pre>\r\n  </div>\r\n</div>\r\n\r\n<!-- END: FIRSTDEMO -->\r\n\r\n<h4>Active Page</h4>\r\n<div class=\"demo_container\">\r\n  <div class=\"demo_example\">\r\n    <nav class=\"js-pagination\">\r\n      <a href=\"#1\">1</a>\r\n      <a href=\"#2\">2</a>\r\n      <a href=\"#3\">3</a>\r\n      <a href=\"#4\">4</a>\r\n      <a href=\"#5\" data-pagination-active=\"true\">5</a>\r\n      <a href=\"#6\">6</a>\r\n      <a href=\"#7\">7</a>\r\n      <a href=\"#8\">8</a>\r\n      <a href=\"#9\">9</a>\r\n      <a href=\"#10\">10</a>\r\n    </nav>\r\n  </div>\r\n  <div class=\"demo_code\">\r\n    <pre><code class=\"language-html\">&lt;nav class=&quot;pagination&quot;&gt;\r\n&Tab;&lt;a href=&quot;1.html&quot;&gt;1&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;2.html&quot;&gt;2&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;3.html&quot; data-pagination-active=&quot;true&quot;&gt;3&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;4.html&quot;&gt;4&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;5.html&quot;&gt;5&lt;/a&gt;\r\n&lt;/nav&gt;</code></pre>\r\n    <pre><code class=\"language-javascript\">$(\".pagination\").pagination();</code></pre>\r\n  </div>\r\n</div>\r\n\r\n<h4>No Theme</h4>\r\n<div class=\"demo_container\">\r\n  <div class=\"demo_example\">\r\n    <nav class=\"js-pagination\" data-pagination-options='{\"theme\":\"\"}'>\r\n      <a href=\"#1\">1</a>\r\n      <a href=\"#2\">2</a>\r\n      <a href=\"#3\">3</a>\r\n      <a href=\"#4\">4</a>\r\n      <a href=\"#5\">5</a>\r\n      <a href=\"#6\">6</a>\r\n      <a href=\"#7\">7</a>\r\n      <a href=\"#8\">8</a>\r\n      <a href=\"#9\">9</a>\r\n      <a href=\"#10\">10</a>\r\n    </nav>\r\n  </div>\r\n  <div class=\"demo_code\">\r\n    <pre><code class=\"language-html\">&lt;nav class=&quot;pagination&quot;&gt;\r\n&Tab;&lt;a href=&quot;1.html&quot;&gt;1&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;2.html&quot;&gt;2&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;3.html&quot;&gt;3&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;4.html&quot;&gt;4&lt;/a&gt;\r\n&Tab;&lt;a href=&quot;5.html&quot;&gt;5&lt;/a&gt;\r\n&lt;/nav&gt;</code></pre>\r\n    <pre><code class=\"language-javascript\">$(\".pagination\").pagination({\r\n  theme: \"\"\r\n});</code></pre>\r\n  </div>\r\n</div>\r\n","asset_root":"../","year":2019}

 #Pagination Demo
<p class="back_link"><a href="https://formstone.it/components/pagination">View Documentation</a></p>