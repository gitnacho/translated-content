---
title: Window.ondragdrop
slug: Web/API/Window/ondragdrop
---
<div class="warning">
<p>在 Firefox 50 中已删除，并且从未在任何其他浏览器中实行。 请改用现代标准的<a href="/en-US/docs/Web/API/HTML_Drag_and_Drop_API">HTML5 拖放</a>功能。</p>
</div>

<h2 id="Summary">摘要</h2>

<p>一个事件处理程序，用于将拖放事件发送到窗口。</p>

<p><strong>语法</strong></p>

<pre class="eval notranslate"><s>window.ondragdrop = funcRef;</s>
window.addEventListener("dragdrop", funcRef, useCapturing);
</pre>

<dl>
 <dt>funcRef </dt>
 <dd>要注册的事件处理函数。</dd>
</dl>

<p><a href="/zh-CN/docs/Web/API/Window/en/Gecko">Gecko</a>({{ Bug(112288) }}) 中未实现<code>window.ondragdrop</code>属性和<code>ondragdrop</code>属性，您必须使用<code>addEventListener</code>。 有关详细信息，请参见<a href="/zh-CN/docs/Web/API/Window/en/DOM/element.addEventListener">addEventListener</a>。</p>

<p><strong>示例</strong></p>

<h3 id="Fire_an_alert_on_dragdrop">在拖放时触发 alert</h3>

<p>在此示例中，事件侦听器被添加到窗口（事件目标）。 如果从外部源将选项卡，链接，标记的文本或文件拖放到此窗口上，则会触发警报。 注意<code>event.stopPropagation()</code>; 阻止浏览器加载放置的标签，链接或文件。</p>

<pre class="notranslate">&lt;html&gt;
&lt;head&gt;&lt;title&gt;dragdroptest&lt;/title&gt;

&lt;script type="text/javascript"&gt;

window.addEventListener("dragdrop", testfunc, false);

function testfunc(event) {
    alert("dragdrop!");
    event.stopPropagation();
}
&lt;/script&gt;

&lt;/head&gt;
&lt;body&gt;
I am bodytext
&lt;/body&gt;
&lt;/html&gt;
</pre>

<p><strong>规范</strong></p>

<p>不属于规范部分。 </p>