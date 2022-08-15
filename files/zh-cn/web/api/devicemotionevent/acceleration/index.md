---
title: DeviceMotionEvent.acceleration
slug: Web/API/DeviceMotionEvent/acceleration
---
<p>{{ ApiRef("Device Orientation Events") }}</p>

<p>acceleration 属性会返回设备的加速度记录（单位：<a href="https://en.wikipedia.org/wiki/Meter_per_second_squared">m / s<sup>2</sup></a>）。</p>

<div class="note"><strong>注意：</strong> 如果硬件无法从 acceleration 数据中移除重力加速度，则该值在{{ domxref("DeviceMotionEvent") }}中可能并不存在，你应当使用{{ domxref("DeviceMotionEvent.accelerationIncludingGravity") }}代替</div>

<h2 id="语法">语法</h2>

<pre class="syntaxbox">var acceleration = <em>instanceOfDeviceMotionEvent</em>.acceleration;
</pre>

<h2 id="值">值</h2>

<p><code>acceleration</code>是一个包括三轴（x、y、z）加速度信息的对象，每个轴都有自己的属性：</p>

<dl>
 <dt><code>x</code></dt>
 <dd>表示 x 轴（西到东）上的加速度</dd>
 <dt><code>y</code></dt>
 <dd>表示 y 轴（南到北）上的加速度</dd>
 <dt><code>z</code></dt>
 <dd>表示 z 轴（下到上）上的加速度</dd>
</dl>

<h2 id="说明">说明</h2>

{{Specifications}}

<h2 id="浏览器兼容性">浏览器兼容性</h2>

{{Compat("api.DeviceMotionEvent.acceleration")}}

<h2 id="推荐浏览">推荐浏览</h2>

<ul>
 <li>{{ domxref("DeviceMotionEvent.accelerationIncludingGravity") }}</li>
 <li>{{ event("devicemotion") }}</li>
 <li>{{ domxref("window.ondevicemotion") }}</li>
 <li>{{ event("deviceorientation") }}</li>
 <li>{{ domxref("DeviceOrientationEvent") }}</li>
 <li><a href="/en-US/docs/WebAPI/Detecting_device_orientation">Detecting device orientation</a></li>
 <li><a href="/en/DOM/Orientation_and_motion_data_explained">Orientation and motion data explained</a></li>
</ul>