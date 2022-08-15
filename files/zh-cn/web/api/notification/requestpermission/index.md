---
title: Notification.requestPermission()
slug: Web/API/notification/requestPermission
---
<p>{{APIRef("Web Notifications")}}</p>

<p>{{domxref("Notification")}} 接口的 <strong><code>requestPermission()</code> </strong>方法请求用户当前来源的权限以显示通知。</p>

<h2 id="语法">语法</h2>

<p>最新的规范已将此方法更新为基于 promise 的语法，工作原理如下：</p>

<pre class="brush: js">Notification.requestPermission().then(function(permission) { ... });</pre>

<p>以前，语法是基于一个简单的回调；此版本现<s style="color: red;">已弃用</s>：</p>

<pre class="brush: js line-numbers  language-js"><code class="language-js">Notification.requestPermission(callback);</code></pre>

<h3 id="参数">参数</h3>

<dl>
 <dt><code>callback</code> {{optional_inline}} {{deprecated_inline("gecko46")}}</dt>
 <dd>一个可选的参数为权限请求的结果的回调函数。此参数已废弃，请使用 Promise 的语法。</dd>
</dl>

<h3 id="返回值">返回值</h3>

<p>一个 {{jsxref("Promise")}} ，将解析为一个 {{domxref("DOMString")}} ，它是用户对权限请求的选择。这个字符串可以是 <code>granted</code>（被授予）， <code>denied</code>（被拒绝） 或者 <code>default</code>（默认）。</p>

<h2 id="实例">实例</h2>

<p>下面这个代码片段将向用户请求权限，然后根据用户的不同选择，输出不同的日志。</p>

<pre class="brush: js">Notification.requestPermission().then(function(result) {
  if (result === 'denied') {
    console.log('Permission wasn\'t granted. Allow a retry.');
    return;
  }
  if (result === 'default') {
    console.log('The permission request was dismissed.');
    return;
  }
  // Do something with the granted permission.
});</pre>

<h2 id="规范">规范</h2>

{{Specifications}}

<h2 id="浏览器兼容性">浏览器兼容性</h2>

{{Compat("api.Notification.requestPermission")}}

<h2 id="参见">参见</h2>

<ul>
 <li><a href="/zh-CN/docs/Web/API/notification/Using_Web_Notifications">使用 Web Notifications</a></li>
</ul>