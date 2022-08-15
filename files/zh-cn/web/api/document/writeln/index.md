---
title: document.writeln
slug: Web/API/Document/writeln
---
<p>{{ ApiRef() }}</p>
<h3 id="Summary">概述</h3>
<p>向文档中写入一串文本，并紧跟着一个换行符。</p>
<h3 id="Syntax">语法</h3>
<pre class="eval">document.writeln(<em>line</em>);
</pre>
<h3 id="Parameters">参数</h3>
<ul>
 <li><code>line</code> 为包含文本的字符串</li>
</ul>
<h3 id="Example">示例</h3>
<pre>document.writeln("&lt;p&gt;enter password:&lt;/p&gt;");
</pre>
<h3 id="Notes">备注</h3>
<p><strong>document.writeln</strong> 和 <a href="/en/DOM/document.write">document.write</a> 一样，但是会添加一个换行符。</p>
<div class="note">
 <strong>Note:</strong> <strong>document.writeln</strong> (like <strong>document.write</strong>) does not work in XHTML documents (you'll get a "Operation is not supported" (<code>NS_ERROR_DOM_NOT_SUPPORTED_ERR</code>) error on the error console). This is the case if opening a local file with a .xhtml file extension or for any document served with an application/xhtml+xml MIME type. More information is available in the <a href="http://www.w3.org/MarkUp/2004/xhtml-faq#docwrite">W3C XHTML FAQ</a>.</div>
<h3 id="Specification">规范</h3>
<p><a href="http://www.w3.org/TR/2000/WD-DOM-Level-2-HTML-20001113/html.html#ID-35318390">writeln </a></p>