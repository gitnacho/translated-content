---
title: DeviceMotionEvent.rotationRate
slug: Web/API/DeviceMotionEvent/rotationRate
---
<p>{{ ApiRef("Device Orientation Events") }}</p>

<p>返回设备围绕其每个轴（x、y、z）旋转的速率（单位：度/秒）。</p>

<div class="note"><strong>注意</strong>: 如果设备无法提供此信息，则为 null</div>

<h2 id="语法">语法</h2>

<pre class="syntaxbox">var rates = <em>instanceOfDeviceMotionEvent</em>.rotationRate;
</pre>

<h2 id="值">值</h2>

<p>rotationRates 属性是一个只读对象，用于描述设备围绕其每个轴的旋转速率：</p>

<dl>
 <dt><code>alpha</code></dt>
 <dd>设备绕其 Z 轴旋转的速率（即绕垂直于屏幕的线旋转）</dd>
 <dt><code>beta</code></dt>
 <dd>设备绕其 X 轴旋转的速率（即从前到后旋转）</dd>
 <dt><code>gamma</code></dt>
 <dd>设备绕其 Y 轴旋转的速率（即从一侧到另一侧）</dd>
</dl>

<h2 id="说明">说明</h2>

{{Specifications}}

<h2 id="浏览器兼容性">浏览器兼容性</h2>

{{Compat("api.DeviceMotionEvent.rotationRate")}}

<h2 id="推荐阅读">推荐阅读</h2>

<ul>
 <li>{{ domxref("DeviceMotionEvent") }}</li>
 <li>{{ event("devicemotion") }}</li>
 <li>{{ domxref("window.ondevicemotion") }}</li>
 <li>{{ event("deviceorientation") }}</li>
 <li>{{ domxref("DeviceOrientationEvent") }}</li>
 <li><a href="/en-US/docs/WebAPI/Detecting_device_orientation">Detecting device orientation</a></li>
 <li><a href="/en/DOM/Orientation_and_motion_data_explained">Orientation and motion data explained</a></li>
</ul>