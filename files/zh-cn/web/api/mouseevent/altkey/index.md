---
title: MouseEvent.altKey
slug: Web/API/MouseEvent/altKey
---
<p>{{APIRef("DOM Events")}}</p>

<p><strong><code>MouseEvent.altKey</code></strong> 只读属性是一个{{jsxref("Boolean")}}变量。当事件触发时，如果<kbd>alt</kbd> 被按下，则返回 true，否则返回 false。</p>

<h2 id="语法">语法</h2>

<pre class="syntaxbox">var <em>altKeyPressed</em> = <em>instanceOfMouseEvent</em>.altKey
</pre>

<h2 id="示例">示例</h2>

<pre class="brush: js">&lt;html&gt;
&lt;head&gt;
&lt;title&gt;altKey example&lt;/title&gt;

&lt;script type="text/javascript"&gt;

function showChar(e){
  alert(
    "Key Pressed: " + String.fromCharCode(e.charCode) + "\n"
    + "charCode: " + e.charCode + "\n"
    + "ALT key pressed: " + e.altKey + "\n"
  );
}

&lt;/script&gt;
&lt;/head&gt;

&lt;body onkeypress="showChar(event);"&gt;
&lt;p&gt;
Press any character key,
with or without holding down the ALT key.&lt;br /&gt;
You can also use the SHIFT key together with the ALT key.
&lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;</pre>

<h2 id="规范">规范</h2>

{{Specifications}}

<h2 id="Browser_compatibility">浏览器兼容性</h2>

{{Compat("api.MouseEvent.altKey")}}

<h2 id="See_also">相关</h2>

<ul>
 <li>{{ domxref("MouseEvent") }}</li>
</ul>