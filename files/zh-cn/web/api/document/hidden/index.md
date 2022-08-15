---
title: Document.hidden
slug: Web/API/Document/hidden
---
<p>{{ ApiRef("DOM") }}</p>

<p><code><strong>Document.hidden</strong></code> （只读属性）返回布尔值，表示页面是（true）否（false）隐藏。</p>

<h2 id="语法">语法</h2>

<pre class="syntaxbox">var <em>string</em> = document.hidden</pre>

<h2 id="例子">例子</h2>

<pre class="brush:js;">document.addEventListener("visibilitychange", function() {
  console.log( document.hidden );
  // Modify behavior...
});</pre>

<h2 id="规范">规范</h2>

{{Specifications}}

<h2 id="浏览器兼容性">浏览器兼容性</h2>



<article>
<p>{{Compat("api.Document.hidden")}}</p>
</article>