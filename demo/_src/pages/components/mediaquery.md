{"template":"component.html","title":"Media Query","demo":"<h4>Basic</h4>\r\n\r\n<!-- START: FIRSTDEMO -->\r\n\r\n<style>\r\n  .demo_output { margin: 20px 0; }\r\n  .demo_output span { display: inline-block; width: 90px; }\r\n  .demo_output p { margin: 0 0 20px; }\r\n  .demo_output p:first-child { font-weight: 600; }\r\n</style>\r\n\r\n<script>\r\n  Formstone.Ready(function() {\r\n    $(window).on(\"mqchange.mediaquery\", logChange);\r\n\r\n    if (!$.mediaquery(\"state\")) {\r\n      $.mediaquery({\r\n        minWidth     : [ 320, 500, 740, 980, 1220 ],\r\n        maxWidth     : [ 1220, 980, 740, 500, 320 ],\r\n        minHeight    : [ 400, 800 ],\r\n        maxHeight    : [ 800, 400 ]\r\n      });\r\n    } else {\r\n      logChange({}, $.mediaquery(\"state\"));\r\n    }\r\n\r\n    $.mediaquery(\"bind\", \"demo\", \"(min-width: 740px)\", {\r\n      enter: logBind,\r\n      leave: logBind\r\n    });\r\n\r\n  });\r\n\r\n  function logChange(e, state) {\r\n    var html = \"\";\r\n    html += \"<p><span>Change:</span><span>MinWidth:</span>\" + state.minWidth + \"<br>\";\r\n    html += \"<span></span><span>MaxWidth:</span>\"+ state.maxWidth + \"<br>\";\r\n    html += \"<span></span><span>MinHeight:</span>\"+ state.minHeight + \"<br>\";\r\n    html += \"<span></span><span>MaxHeight:</span>\"+ state.maxHeight + \"</p>\";\r\n\r\n    $(\".demo_basic\").prepend(html);\r\n  }\r\n\r\n  function logBind() {\r\n    var mql = this,\r\n      type = mql.matches ? \"Enter\" : \"Leave\"\r\n      html = \"<p><span>\" + type + \":</span>\" + mql.media + \"<br>\";\r\n\r\n    $(\".demo_binding\").prepend(html);\r\n  }\r\n</script>\r\n\r\n<div class=\"demo_output demo_basic form_textarea\"></div>\r\n\r\n<!-- END: FIRSTDEMO -->\r\n\r\n<h4>Binding</h2>\r\n<div class=\"demo_output demo_binding form_textarea\"></div>\n","asset_root":"../","year":2019}

 #Media Query Demo
<p class="back_link"><a href="https://formstone.it/components/mediaquery">View Documentation</a></p>