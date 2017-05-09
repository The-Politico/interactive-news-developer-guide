# ADS

Ads, we need em. We got em.

---

Using ads

* Each ad on a page must have a **unique ID**. Please select from the **approved** ad options below
* **Slot the appropriate ID** in the id field below.

  `<div style="text-align: center;" class="content-group ad">`

  `<div style="text-align: center;" class="ad-slot flex vertical " id="`**`pol-02`**`" >`

  `</div>`

  `</div>`

### Banner ads

* pol-01
* pol-08

### Cube ads

* pol-05 \(300x225\)
* pol-04 \(300x225\)
* pol-02 \(this may also render as a supercube 300x600\)

##### 

### Responsive ad code

`<script>`

`// Responsive Ads Functionality - pulled from main.js`

`(function($) {`

`var getScrollBarWidth = function() {`

`var inner = document.createElement('p');`

`inner.style.width = "100%";`

`inner.style.height = "200px";`

`var outer = document.createElement('div');`

`outer.style.position = "absolute";`

`outer.style.top = "0px";`

`outer.style.left = "0px";`

`outer.style.visibility = "hidden";`

`outer.style.width = "200px";`

`outer.style.height = "150px";`

`outer.style.overflow = "hidden";`

`outer.appendChild(inner);`

`document.body.appendChild(outer);`

`var w1 = inner.offsetWidth;`

`outer.style.overflow = 'scroll';`

`var w2 = inner.offsetWidth;`

`if (w1 === w2) {`

`w2 = outer.clientWidth;`

`}`

`document.body.removeChild(outer);`

`return (w1 - w2);`

`}`

`var adRefresh = function() {`

`if (typeof googletag !== 'undefined') {`

`googletag.cmd.push(function() {`

`googletag.pubads().refresh();`

`});`

`}`

`}`

`var setAdThreshold = function() {`

`var adThresholdName = 'alpha'; //Viewport below 748px`

`if (currentViewportWidth >= 748 && currentViewportWidth < 990) {`

`adThresholdName = 'beta';`

`} else if (currentViewportWidth >= 990 && currentViewportWidth < breakLarge) {`

`adThresholdName = 'gamma';`

`} else if (currentViewportWidth >= breakLarge && currentViewportWidth < 1028) {`

`adThresholdName = 'delta';`

`} else if (currentViewportWidth >= 1028) {`

`adThresholdName = 'epsilon';`

`}`

`if (adThresholdName != 'epsilon' && adThresholdName != 'delta') {`

`jQuery('.global-utility-bar .reveal-toggle .reveal').removeClass('is-active');`

`jQuery('.utility-bar-bottom').removeClass('is-active');`

`jQuery('.dynamic-ad-wrapper .ad-slot').remove();`

`jQuery('.global-utility-bar .dynamic-ad-wrapper').html('');`

`}`

`return adThresholdName;`

`}`

`var PoliticoAds = {`

`'currentAdThreshold': ''`

`};`

`var checkAdThreshold = function() {`

`var newAdThreshold = setAdThreshold();`

`if (PoliticoAds.currentAdThreshold !== newAdThreshold) {`

`PoliticoAds.currentAdThreshold = newAdThreshold;`

`adRefresh();`

`}`

`}`

`var getAdThreshold = function() {`

`PoliticoAds.currentAdThreshold = setAdThreshold();`

`}`

`$(window).on("resize", function() {`

`currentViewportWidth = document.documentElement.clientWidth + scrollbarWidth;`

`checkAdThreshold();`

`});`

`// init`

`var scrollbarWidth = getScrollBarWidth(),`

`currentViewportWidth = document.documentElement.clientWidth + scrollbarWidth,`

`breakSmall = 503, //Equals 31.4375em`

`breakMedium = 686, //Equals 42.875em`

`breakLarge = 1012, //Equals 63.25em`

`breakExtra = 1220; //Equals 76.25em`

`getAdThreshold();`

`})(jQuery)`

`</script>`

### 



