{"template":"component.html","title":"Grid","demo":"<script>\r\n  Formstone.Ready(function() {\r\n    var $body = $(\"body\");\r\n      $gridSelect = $(\"#grid_select\").on(\"change\", function() {\r\n        var $target = $(this),\r\n          type = $target.val();\r\n\r\n        $body.removeClass(\"fs-grid-fluid fs-grid-adaptive\")\r\n           .addClass(type);\r\n      });\r\n  });\r\n</script>\r\n\r\n<form action=\"#\" method=\"GET\" class=\"fs-row form demo_form\">\r\n  <fieldset class=\"fs-cell fs-lg-third form_fieldset\">\r\n    <label class=\"form_label\" for=\"grid_select\">Select Grid Type</label>\r\n    <select class=\"js-dropdown\" name=\"grid_select\" id=\"grid_select\">\r\n      <option value=\"__grid-base\">Base Grid</option>\r\n      <option value=\"fs-grid-adaptive\">Full Adaptive Grid</option>\r\n      <option value=\"fs-grid-fluid\">Full Fluid Grid</option>\r\n    </select>\r\n  </fieldset>\r\n</form>\r\n\r\n\r\n<!-- Bookmarklet -->\r\n<h4>Bookmarklet</h4>\r\n<p>Drag the bookmarklet to your bookmarks bar.</p>\r\n<a href=\"javascript:(function(){if(typeof%20FSGridBookmarklet==='undefined'){document.body.appendChild(document.createElement('script')).src='//formstone.it/js/bookmarklet/grid.js';}else{FSGridBookmarklet();}})();\" class=\"button bookmarklet\">Formstone Grid</a>\r\n\r\n<br class=\"clear\">\r\n\r\n<p>Or, include it on every page of your development site:</p>\r\n<pre class=\"example\"><code class=\"language-markup\">&lt;script&gt;\r\n(function(){if(typeof FSGridBookmarklet==='undefined'){document.body.appendChild(document.createElement('script')).src='//formstone.it/js/bookmarklet/grid.js';}else{FSGridBookmarklet();}})();\r\n&lt;/script&gt;</code></pre>\r\n\r\n<script>\r\n(function(){if(typeof FSGridBookmarklet==='undefined'){document.body.appendChild(document.createElement('script')).src='//formstone.it/js/bookmarklet/grid.js';}else{FSGridBookmarklet();}})();\r\n</script>\r\n\r\n<br>\r\n\r\n\r\n<h4>Asymmetrical</h4>\r\n\r\n<!-- START: FIRSTDEMO -->\r\n\r\n<style>\r\n  .button.bookmarklet { clear: both; }\r\n\r\n  .example { margin: 20px 0; }\r\n  .example .fs-row { background: #CFD8DC; border-radius: 2px; padding-top: 1.8%; }\r\n  .example [class*=\"fs-cell\"] { background: #455a64; color: #fff; border-radius: 2px; margin-bottom: 1.8%; text-align: center; }\n  .example .tall { height: 100px; }\n  .example .highlight { background: #00bcd4; }\r\n  .example .nested { background: none; margin-top: 0; margin-bottom: 0; }\r\n  .example .nested .fs-row { padding-top: 0; }\r\n  .example [class*=\"label\"] { display: block; padding-top: 15px; padding-bottom: 15px; }\r\n\r\n  /*.example .label,\r\n  .example .label_small,\r\n  .example .label_medium,\r\n  .example .label_large { background: #455a64; }*/\r\n\r\n  .example .label_small,\r\n  .example .label_medium,\r\n  .example .label_large { display: none; }\r\n\r\n  @media screen and (min-width: 0px) and (max-width: 739px) {\r\n    .example .label_small { display: block; }\r\n  }\r\n  @media screen and (min-width: 740px) and (max-width: 979px) {\r\n    .example .label_medium { display: block; }\r\n  }\r\n  @media screen and (min-width: 980px) {\r\n    .example .label_large { display: block; }\r\n  }\r\n</style>\r\n\r\n<div class=\"example\">\r\n  <div class=\"fs-row\">\r\n    <div class=\"fs-cell fs-sm-1 fs-md-2 fs-lg-4\">\r\n      <span class=\"label_small\">fs-sm-1</span>\r\n      <span class=\"label_medium\">fs-md-2</span>\r\n      <span class=\"label_large\">fs-lg-4</span>\r\n    </div>\r\n    <div class=\"fs-cell fs-sm-2 fs-md-4 fs-lg-8\">\r\n      <span class=\"label_small\">fs-sm-2</span>\r\n      <span class=\"label_medium\">fs-md-4</span>\r\n      <span class=\"label_large\">fs-lg-8</span>\r\n    </div>\r\n  </div>\r\n</div>\r\n\r\n<!-- END: FIRSTDEMO -->\r\n\r\n<h4>Symmetrical</h4>\r\n<div class=\"example\">\r\n  <div class=\"fs-row\">\r\n    <div class=\"fs-cell fs-sm-3 fs-md-3 fs-lg-6\">\r\n      <span class=\"label_small\">fs-sm-3</span>\r\n      <span class=\"label_medium\">fs-md-3</span>\r\n      <span class=\"label_large\">fs-lg-6</span>\r\n    </div>\r\n    <div class=\"fs-cell fs-sm-3 fs-md-3 fs-lg-6\">\r\n      <span class=\"label_small\">fs-sm-3</span>\r\n      <span class=\"label_medium\">fs-md-3</span>\r\n      <span class=\"label_large\">fs-lg-6</span>\r\n    </div>\r\n  </div>\r\n</div>\r\n\r\n<h4>3 Column</h4>\r\n<div class=\"example\">\r\n  <div class=\"fs-row\">\r\n    <div class=\"fs-cell fs-all-third\">\r\n      <span class=\"label\">fs-all-third</span>\r\n    </div>\r\n    <div class=\"fs-cell fs-all-third\">\r\n      <span class=\"label\">fs-all-third</span>\r\n    </div>\r\n    <div class=\"fs-cell fs-all-third\">\r\n      <span class=\"label\">fs-all-third</span>\r\n    </div>\r\n  </div>\r\n</div>\n\n<h4>Nested</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-md-4 fs-lg-8 nested\">\n      <div class=\"fs-row\">\n        <div class=\"fs-cell fs-md-half fs-lg-half\">\n          <span class=\"label_small\">fs-sm-full</span>\n          <span class=\"label_medium\">fs-md-half</span>\n          <span class=\"label_large\">fs-lg-half</span>\n        </div>\n        <div class=\"fs-cell fs-md-half fs-lg-half\">\n          <span class=\"label_small\">fs-sm-full</span>\n          <span class=\"label_medium\">fs-md-half</span>\n          <span class=\"label_large\">fs-lg-half</span>\n        </div>\n      </div>\n    </div>\n    <div class=\"fs-cell fs-md-2 fs-lg-4\">\n      <span class=\"label_small\">fs-sm-full</span>\n      <span class=\"label_medium\">fs-md-2</span>\n      <span class=\"label_large\">fs-lg-4</span>\n    </div>\n  </div>\n</div>\n\n<h4>Push</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-sm-2 fs-sm-push-1 fs-md-3 fs-md-push-3 fs-lg-8 fs-lg-push-4\">\n      <span class=\"label_small\">fs-sm-2 fs-sm-push-1</span>\n      <span class=\"label_medium\">fs-md-3 fs-md-push-3</span>\n      <span class=\"label_large\">fs-lg-8 fs-lg-push-4</span>\n    </div>\n  </div>\n</div>\n\n<h4>Contained</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell-contained fs-all-half\">\n      <span class=\"label\">fs-cell-contained</span>\n    </div>\n    <div class=\"fs-cell-contained fs-all-half\">\n      <span class=\"label\">fs-cell-contained</span>\n    </div>\n  </div>\n</div>\n\n<h4>Padded</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell-padded fs-all-half\">\n      <span class=\"label\">fs-cell-padded</span>\n    </div>\n    <div class=\"fs-cell-padded fs-all-half\">\n      <span class=\"label\">fs-cell-padded</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Align Start</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third tall\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-align-start fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n    <div class=\"fs-cell fs-all-third third\">\n      <span class=\"label\">3</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Align Center</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third tall\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-align-center fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n    <div class=\"fs-cell fs-all-third tall\">\n      <span class=\"label\">3</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Align End</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third tall\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-align-end fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n    <div class=\"fs-cell fs-all-third tall\">\n      <span class=\"label\">3</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Justify Start</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third fs-all-justify-start\">\n      <span class=\"label\">1</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Justify Center</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third fs-all-justify-center\">\n      <span class=\"label\">1</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Justify End</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third fs-all-justify-end\">\n      <span class=\"label\">1</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Order First</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n    <div class=\"fs-cell fs-all-third fs-first highlight\">\n      <span class=\"label\">3</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Order Last</h4>\n<div class=\"example\">\n  <div class=\"fs-row\">\n    <div class=\"fs-cell fs-all-third fs-last highlight\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">3</span>\n    </div>\n  </div>\n</div>\n\n<h4>Cell Width Auto</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-reverse\">\n    <div class=\"fs-cell fs-all-auto\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-auto\">\n      <span class=\"label\">2</span>\n    </div>\n    <div class=\"fs-cell fs-all-auto\">\n      <span class=\"label\">3</span>\n    </div>\n    <div class=\"fs-cell fs-all-auto\">\n      <span class=\"label\">4</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Justify Around</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-justify-around\">\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Justify Between</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-justify-between\">\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Justify Start</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-justify-start\">\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Justify Center</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-justify-center\">\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Justify End</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-justify-end\">\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Align Start</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-align-start\">\n    <div class=\"fs-cell fs-all-half tall\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-half\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Align Center</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-align-center\">\n    <div class=\"fs-cell fs-all-half tall\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-half\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Align End</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-all-align-end\">\n    <div class=\"fs-cell fs-all-half tall\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-half\">\n      <span class=\"label\">2</span>\n    </div>\n  </div>\n</div>\n\n<h4>Row Order Reverse</h4>\n<div class=\"example\">\n  <div class=\"fs-row fs-reverse\">\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">1</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">2</span>\n    </div>\n    <div class=\"fs-cell fs-all-third\">\n      <span class=\"label\">3</span>\n    </div>\n  </div>\n</div>\n\n\n<div class=\"fs-row\">\n  <div class=\"fs-cell fs-all-full\">\n    <div class=\"fs-row\">\n      <div class=\"fs-cell fs-all-third fs-contained\"><span class=\"label\">1</span></div>\n      <div class=\"fs-cell fs-all-third fs-contained\"><span class=\"label\">2</span></div>\n      <div class=\"fs-cell fs-all-third fs-contained\"><span class=\"label\">3</span></div>\n    </div>\n  </div>\n</div>\n","asset_root":"../","year":2019}

 #Grid Demo
<p class="back_link"><a href="https://formstone.it/components/grid">View Documentation</a></p>