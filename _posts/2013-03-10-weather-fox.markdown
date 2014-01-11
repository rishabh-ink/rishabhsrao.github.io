---
layout: post
title: "WeatherFox"
date: 2013-03-10 17:32
comments: true
categories: technical
---

I've been working on a simple Weather application using HTML5-based technologies. I completed the first version recently.  The source is available at [Github](https://github.com/rishabhsrao/weather-fox).

<!-- more -->

The technologies used are:

* [KnockoutJS](http://knockoutjs.com)
* [Yeoman.io](http://yeoman.io)
* [RequireJS](http://requirejs.org)
* [SCSS](http://sass-lang.com)
* [jQuery Mobile](http://jquerymobile.com)
* [jQuery deferreds](http://api.jquery.com/category/deferred-object)
* [HTML5 GeoLocation API](http://diveintohtml5.info/geolocation.html)
* [Yahoo! Weather API](http://developer.yahoo.com/weather) via [Yahoo! Query Language](http://developer.yahoo.com/yql) and [Yahoo! Pipes](http://pipes.yahoo.com)
  * The Yahoo! Pipe URL is [http://pipes.yahoo.com/pipes/pipe.info?_id=687279a3ea30ea78c978b1bf6e235055](http://pipes.yahoo.com/pipes/pipe.info?_id=687279a3ea30ea78c978b1bf6e235055)

<div class="row pricing-table-row">
  <div class="four columns">
    <ul class="pricing-table">
      <li class="title">Android</li>
      <li class="description">
        <img src="/images/posts/2013-03-10-weather-fox/android-logo.png" alt="Android logo" />
      </li>
      <li class="bullet-item">
        <img src="/images/posts/2013-03-10-weather-fox/qr-android.png" alt="Android QR code" />
      </li>
      <li class="bullet-item">
        <p>bit.ly/<strong>weatherfox-a</strong></p>
      </li>
      <li class="cta-button"><a class="button success" href="/images/posts/2013-03-10-weather-fox/WeatherFox-Android.apk">Download!</a></li>
    </ul>
  </div>
  <div class="four columns">
    <ul class="pricing-table">
      <li class="title">Windows Mobile</li>
      <li class="description">
        <img src="/images/posts/2013-03-10-weather-fox/windows-mobile-logo.png" alt="Windows Mobile logo" />
      </li>
      <li class="bullet-item">
        <img src="/images/posts/2013-03-10-weather-fox/qr-winmob.png" alt="Windows Mobile QR code" />
      </li>
      <li class="bullet-item">
        <p>bit.ly/<strong>weatherfox-wm</strong></p>
      </li>
      <li class="cta-button"><a class="button success" href="/images/posts/2013-03-10-weather-fox/WeatherFox-WinMob.xap">Donwload!</a></li>
    </ul>
  </div>
  <div class="four columns">
    <ul class="pricing-table">
      <li class="title">Firefox OS</li>
      <li class="description">
        <img src="/images/posts/2013-03-10-weather-fox/firefox-os-logo.png" alt="Firefox OS logo" />
      </li>
      <li class="bullet-item">
        <img src="/images/posts/2013-03-10-weather-fox/qr-firefox-os.png" alt="Firefox OS QR code" />
      </li>
      <li class="bullet-item">
        <p>bit.ly/<strong>weatherfox-fm</strong></p>
      </li>
      <li class="cta-button"><a id="firefox-os-install" href="https://marketplace.firefox.com/app/weatherfox" class="button success">Download!</a></li>
    </ul>
  </div>
</div>

Here are some screenshots of the application:

<div class="image-gallery">
  <img src="/images/posts/2013-03-10-weather-fox/1.jpg" />
  <img src="/images/posts/2013-03-10-weather-fox/2.jpg" />
  <img src="/images/posts/2013-03-10-weather-fox/3.jpg" />
  <img src="/images/posts/2013-03-10-weather-fox/4.jpg" />
  <img src="/images/posts/2013-03-10-weather-fox/5.jpg" />
  <img src="/images/posts/2013-03-10-weather-fox/6.png" />
  <img src="/images/posts/2013-03-10-weather-fox/7.png" />
  <img src="/images/posts/2013-03-10-weather-fox/8.png" />
  <img src="/images/posts/2013-03-10-weather-fox/9.jpg" />
  <img src="/images/posts/2013-03-10-weather-fox/10.jpg" />
</div>

<script>
  //<![CDATA[

  var manifestURL = "http://rishabhsrao.github.com/weather-fox/dist/manifest.webapp";

  if("undefined" !== typeof (window.navigator.mozApps)) {
    jQuery("#firefox-os-install").on("click", function(event) {
      event.preventDefault();
      navigator.mozApps.install(manifestURL);
    });
  }

  //]]>
</script>