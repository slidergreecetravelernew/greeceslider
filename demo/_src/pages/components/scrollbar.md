{"template":"component.html","title":"Scrollbar","demo":"<h4>Basic</h4>\n\n<!-- START: FIRSTDEMO -->\n\r\n<style>\r\n  .scrollbar { height: 200px; overflow: auto; margin: 20px 0 0; }\r\n</style>\n\r\n<div class=\"demo_container\">\r\n  <div class=\"demo_example\">\r\n    <div class=\"scrollbar scrollbar_theme js-scrollbar\" data-scrollbar-options='{\"trackMargin\":5}'>\n      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla porta aliquet gravida. Aenean pulvinar blandit orci vel fermentum. Phasellus viverra pulvinar viverra. Quisque et sagittis ante. Nulla sem neque, fermentum at laoreet vel, rhoncus sit amet nisl. Donec consectetur urna ac massa placerat ac pharetra sem mollis. Integer nibh urna, placerat vel placerat in, tempor at nisi. Aenean rutrum, enim sit amet rutrum fermentum, magna justo volutpat massa, lacinia adipiscing nisl magna eget nibh. In auctor, nibh eget faucibus tristique, arcu turpis molestie orci, placerat suscipit diam nibh et erat. Curabitur tempus lectus quis odio ornare porta.</p>\r\n      <p>Aenean odio libero, eleifend eu luctus quis, accumsan ac risus. Mauris egestas bibendum tortor vel semper. Ut egestas, erat ut rutrum tempus, massa erat commodo arcu, id congue justo odio ac erat. Quisque non purus et nunc consequat scelerisque. Vestibulum vitae tristique dolor. Suspendisse ac quam interdum libero euismod tempus. Sed a ante justo, varius commodo urna.</p>\r\n      <p>Ut ante felis, malesuada eu eleifend convallis, tempor eget tellus. Vestibulum rhoncus elementum dui a sagittis. Praesent eu nunc vitae massa cursus luctus ac eget massa. Etiam sagittis nibh nisi, vel sagittis felis. Aliquam vulputate mauris id nunc pellentesque at fermentum lacus dapibus. Donec pretium consectetur magna sit amet egestas. Ut dignissim adipiscing purus sit amet lobortis.</p>\r\n      <p>Curabitur ullamcorper, nisi quis convallis luctus, nunc nisi mollis felis, eu mattis nunc sapien sed sapien. Vestibulum in nisi mauris, mattis sagittis lacus. Pellentesque in sem augue, a blandit augue. Aliquam bibendum diam ac erat imperdiet vestibulum. Vivamus dignissim, quam in feugiat scelerisque, enim risus interdum turpis, in vehicula ante lorem eu erat. Mauris ac turpis luctus libero pulvinar ultricies. Praesent porttitor nulla non risus porta consequat. Nunc vulputate porta nulla non ultrices. Donec et magna eu nisl elementum scelerisque. Curabitur in vehicula dui.</p>\r\n      <p>Suspendisse eu nibh in libero euismod condimentum eget nec enim. Suspendisse nec ligula nec augue tristique semper sed suscipit erat. Integer et nunc a augue pellentesque fringilla. Nullam leo ligula, mattis id pretium ac, suscipit sed nunc. Duis ac lorem nec velit malesuada tempus hendrerit ut metus. Quisque a lacus vel lectus rhoncus luctus. Aliquam ornare, nunc sit amet porttitor ornare, libero lectus congue enim, vitae tincidunt sapien justo et ligula. Proin vestibulum blandit fringilla. </p>\r\n    </div>\r\n  </div>\r\n  <div class=\"demo_code\">\r\n    <pre><code class=\"language-html\">&lt;div class=&quot;scrollbar&quot;&gt;\r\n&Tab;...\r\n&lt;/div&gt;</code></pre>\r\n    <pre><code class=\"language-javascript\">$(\".scrollbar\").scrollbar();</code></pre>\r\n  </div>\r\n</div>\r\n\r\n<!-- END: FIRSTDEMO -->\r\n\r\n<style>\r\n  .scrollbar_theme { padding: 10px 20px 10px 20px; }\r\n  .scrollbar_theme.fs-scrollbar { padding: 0; }\r\n  .scrollbar_theme.fs-scrollbar .fs-scrollbar-content,\r\n  .scrollbar_theme.fs-scrollbar-active .fs-scrollbar-content { padding: 20px 40px 20px 20px; }\r\n\r\n  .scrollbar p { margin: 0 0 20px; }\r\n\r\n  .scrollbar.horizontal { height: 225px; padding: 0; }\r\n\r\n  .wide_load { width: 2400px; overflow: hidden; }\r\n  .wide_load p { float: left; margin: 0 25px 0 0; width: 450px; }\r\n</style>\r\n\r\n<h4>Horizontal</h4>\r\n<div class=\"demo_container\">\r\n  <div class=\"demo_example\">\r\n    <div class=\"scrollbar scrollbar_theme horizontal js-scrollbar\" data-scrollbar-options='{\"horizontal\":true,\"trackMargin\":5}'>\r\n      <div class=\"wide_load\">\r\n        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla porta aliquet gravida. Aenean pulvinar blandit orci vel fermentum. Phasellus viverra pulvinar viverra. Quisque et sagittis ante. Nulla sem neque, fermentum at laoreet vel, rhoncus sit amet nisl. Donec consectetur urna ac massa placerat ac pharetra sem mollis. Integer nibh urna, placerat vel placerat in, tempor at nisi.</p>\r\n        <p>Aenean odio libero, eleifend eu luctus quis, accumsan ac risus. Mauris egestas bibendum tortor vel semper. Ut egestas, erat ut rutrum tempus, massa erat commodo arcu, id congue justo odio ac erat. Quisque non purus et nunc consequat scelerisque. Vestibulum vitae tristique dolor. Suspendisse ac quam interdum libero euismod tempus. Sed a ante justo, varius commodo urna.</p>\r\n        <p>Ut ante felis, malesuada eu eleifend convallis, tempor eget tellus. Vestibulum rhoncus elementum dui a sagittis. Praesent eu nunc vitae massa cursus luctus ac eget massa. Etiam sagittis nibh nisi, vel sagittis felis. Aliquam vulputate mauris id nunc pellentesque at fermentum lacus dapibus. Donec pretium consectetur magna sit amet egestas. Ut dignissim adipiscing purus sit amet lobortis.</p>\r\n        <p>Curabitur ullamcorper, nisi quis convallis luctus, nunc nisi mollis felis, eu mattis nunc sapien sed sapien. Vestibulum in nisi mauris, mattis sagittis lacus. Pellentesque in sem augue, a blandit augue. Aliquam bibendum diam ac erat imperdiet vestibulum. Vivamus dignissim, quam in feugiat scelerisque, enim risus interdum turpis, in vehicula ante lorem eu erat. Mauris ac turpis luctus libero pulvinar ultricies.</p>\r\n        <p>Suspendisse eu nibh in libero euismod condimentum eget nec enim. Suspendisse nec ligula nec augue tristique semper sed suscipit erat. Integer et nunc a augue pellentesque fringilla. Nullam leo ligula, mattis id pretium ac, suscipit sed nunc. Duis ac lorem nec velit malesuada tempus hendrerit ut metus. Quisque a lacus vel lectus rhoncus luctus. </p>\r\n      </div>\r\n    </div>\r\n  </div>\r\n  <div class=\"demo_code\">\r\n    <pre><code class=\"language-html\">&lt;div class=&quot;scrollbar&quot;&gt;\r\n&Tab;...\r\n&lt;/div&gt;</code></pre>\r\n    <pre><code class=\"language-javascript\">$(\".scrollbar\").scrollbar({\r\n  horizontal: true\r\n});</code></pre>\r\n  </div>\r\n</div>\n\n<h4>Nested</h4>\n<div class=\"demo_container\">\n  <div class=\"demo_example\">\n    <div class=\"scrollbar scrollbar_theme js-scrollbar\" data-scrollbar-options='{\"trackMargin\":5}'>\n\n      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla porta aliquet gravida. Aenean pulvinar blandit orci vel fermentum. Phasellus viverra pulvinar viverra. Quisque et sagittis ante. Nulla sem neque, fermentum at laoreet vel, rhoncus sit amet nisl. Donec consectetur urna ac massa placerat ac pharetra sem mollis. Integer nibh urna, placerat vel placerat in, tempor at nisi. Aenean rutrum, enim sit amet rutrum fermentum, magna justo volutpat massa, lacinia adipiscing nisl magna eget nibh. In auctor, nibh eget faucibus tristique, arcu turpis molestie orci, placerat suscipit diam nibh et erat. Curabitur tempus lectus quis odio ornare porta.</p>\n\n      <div class=\"scrollbar scrollbar_theme horizontal js-scrollbar\" data-scrollbar-options='{\"horizontal\":true,\"trackMargin\":5}' style=\"margin: 20px 0;\">\n        <div class=\"wide_load\">\n          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla porta aliquet gravida. Aenean pulvinar blandit orci vel fermentum. Phasellus viverra pulvinar viverra. Quisque et sagittis ante. Nulla sem neque, fermentum at laoreet vel, rhoncus sit amet nisl. Donec consectetur urna ac massa placerat ac pharetra sem mollis. Integer nibh urna, placerat vel placerat in, tempor at nisi.</p>\n          <p>Aenean odio libero, eleifend eu luctus quis, accumsan ac risus. Mauris egestas bibendum tortor vel semper. Ut egestas, erat ut rutrum tempus, massa erat commodo arcu, id congue justo odio ac erat. Quisque non purus et nunc consequat scelerisque. Vestibulum vitae tristique dolor. Suspendisse ac quam interdum libero euismod tempus. Sed a ante justo, varius commodo urna.</p>\n          <p>Ut ante felis, malesuada eu eleifend convallis, tempor eget tellus. Vestibulum rhoncus elementum dui a sagittis. Praesent eu nunc vitae massa cursus luctus ac eget massa. Etiam sagittis nibh nisi, vel sagittis felis. Aliquam vulputate mauris id nunc pellentesque at fermentum lacus dapibus. Donec pretium consectetur magna sit amet egestas. Ut dignissim adipiscing purus sit amet lobortis.</p>\n          <p>Curabitur ullamcorper, nisi quis convallis luctus, nunc nisi mollis felis, eu mattis nunc sapien sed sapien. Vestibulum in nisi mauris, mattis sagittis lacus. Pellentesque in sem augue, a blandit augue. Aliquam bibendum diam ac erat imperdiet vestibulum. Vivamus dignissim, quam in feugiat scelerisque, enim risus interdum turpis, in vehicula ante lorem eu erat. Mauris ac turpis luctus libero pulvinar ultricies.</p>\n          <p>Suspendisse eu nibh in libero euismod condimentum eget nec enim. Suspendisse nec ligula nec augue tristique semper sed suscipit erat. Integer et nunc a augue pellentesque fringilla. Nullam leo ligula, mattis id pretium ac, suscipit sed nunc. Duis ac lorem nec velit malesuada tempus hendrerit ut metus. Quisque a lacus vel lectus rhoncus luctus. </p>\n        </div>\n      </div>\n\n      <p>Suspendisse eu nibh in libero euismod condimentum eget nec enim. Suspendisse nec ligula nec augue tristique semper sed suscipit erat. Integer et nunc a augue pellentesque fringilla. Nullam leo ligula, mattis id pretium ac, suscipit sed nunc. Duis ac lorem nec velit malesuada tempus hendrerit ut metus. Quisque a lacus vel lectus rhoncus luctus. Aliquam ornare, nunc sit amet porttitor ornare, libero lectus congue enim, vitae tincidunt sapien justo et ligula. Proin vestibulum blandit fringilla. </p>\n    </div>\n  </div>\n  <div class=\"demo_code\">\n    <pre><code class=\"language-html\">&lt;div class=&quot;scrollbar-vertical&quot;&gt;\n&Tab;...\n&Tab;&lt;div class=&quot;scrollbar-horizontal&quot;&gt;\n&Tab;&Tab;...\n&Tab;&lt;/div&gt;\n&Tab;...\n&lt;/div&gt;</code></pre>\n    <pre><code class=\"language-javascript\">$(\".scrollbar-vertical\").scrollbar();\n$(\".scrollbar-horizontal\").scrollbar({\n&Tab;horizontal: true\n});</code></pre>\n  </div>\n</div>\r\n\r\n<h4>No Theme</h4>\r\n<div class=\"demo_container\">\r\n  <div class=\"demo_example\">\r\n    <div class=\"scrollbar js-scrollbar\" data-scrollbar-options='{\"theme\":\"\",\"trackMargin\":5}'>\r\n      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla porta aliquet gravida. Aenean pulvinar blandit orci vel fermentum. Phasellus viverra pulvinar viverra. Quisque et sagittis ante. Nulla sem neque, fermentum at laoreet vel, rhoncus sit amet nisl. Donec consectetur urna ac massa placerat ac pharetra sem mollis. Integer nibh urna, placerat vel placerat in, tempor at nisi. Aenean rutrum, enim sit amet rutrum fermentum, magna justo volutpat massa, lacinia adipiscing nisl magna eget nibh. In auctor, nibh eget faucibus tristique, arcu turpis molestie orci, placerat suscipit diam nibh et erat. Curabitur tempus lectus quis odio ornare porta.</p>\r\n      <p>Aenean odio libero, eleifend eu luctus quis, accumsan ac risus. Mauris egestas bibendum tortor vel semper. Ut egestas, erat ut rutrum tempus, massa erat commodo arcu, id congue justo odio ac erat. Quisque non purus et nunc consequat scelerisque. Vestibulum vitae tristique dolor. Suspendisse ac quam interdum libero euismod tempus. Sed a ante justo, varius commodo urna.</p>\r\n      <p>Ut ante felis, malesuada eu eleifend convallis, tempor eget tellus. Vestibulum rhoncus elementum dui a sagittis. Praesent eu nunc vitae massa cursus luctus ac eget massa. Etiam sagittis nibh nisi, vel sagittis felis. Aliquam vulputate mauris id nunc pellentesque at fermentum lacus dapibus. Donec pretium consectetur magna sit amet egestas. Ut dignissim adipiscing purus sit amet lobortis.</p>\r\n      <p>Curabitur ullamcorper, nisi quis convallis luctus, nunc nisi mollis felis, eu mattis nunc sapien sed sapien. Vestibulum in nisi mauris, mattis sagittis lacus. Pellentesque in sem augue, a blandit augue. Aliquam bibendum diam ac erat imperdiet vestibulum. Vivamus dignissim, quam in feugiat scelerisque, enim risus interdum turpis, in vehicula ante lorem eu erat. Mauris ac turpis luctus libero pulvinar ultricies. Praesent porttitor nulla non risus porta consequat. Nunc vulputate porta nulla non ultrices. Donec et magna eu nisl elementum scelerisque. Curabitur in vehicula dui.</p>\r\n      <p>Suspendisse eu nibh in libero euismod condimentum eget nec enim. Suspendisse nec ligula nec augue tristique semper sed suscipit erat. Integer et nunc a augue pellentesque fringilla. Nullam leo ligula, mattis id pretium ac, suscipit sed nunc. Duis ac lorem nec velit malesuada tempus hendrerit ut metus. Quisque a lacus vel lectus rhoncus luctus. Aliquam ornare, nunc sit amet porttitor ornare, libero lectus congue enim, vitae tincidunt sapien justo et ligula. Proin vestibulum blandit fringilla. </p>\r\n    </div>\r\n  </div>\r\n  <div class=\"demo_code\">\r\n    <pre><code class=\"language-html\">&lt;div class=&quot;scrollbar&quot;&gt;\r\n&Tab;...\r\n&lt;/div&gt;</code></pre>\r\n    <pre><code class=\"language-javascript\">$(\".scrollbar\").scrollbar({\r\n  theme: \"\"\r\n});</code></pre>\r\n  </div>\r\n</div>\r\n","asset_root":"../","year":2019}

 #Scrollbar Demo
<p class="back_link"><a href="https://formstone.it/components/scrollbar">View Documentation</a></p>