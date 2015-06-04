FlipFlap
========

Easily create animations using a series of images

Quickstart
----------

Download the dependencies and use them as follows:

Dependencies
------------

```html
<script type="text/javascript" src="js/libs/jquery.js"></script>
<script type="text/javascript" src="js/libs/preload.js.js"></script>
<script type="text/javascript" src="js/libs/flipflap.js"></script>
```

JavaScript
----------

```javascript
$('#sequence').flipFlap({
	dir: "img/",
	digits: 4,
	end: 60,
	extension: ".png",
	fps: 60,
	loopAmount: 'infinite',
	loopType: "reverse",
	name: "crystal",
	start: 0,
	trailing: true
)};
```

HTML
----

```html
<div id="sequence" class="img-sequence">
	<div class="loading">
		<p>0%</p>
		<div class="progress"></div>
	</div>
	<h2>Infinite Reverse Loop</h2>
</div>
````

CSS
---

```css
.img-sequence {
	position: relative;
	width: 400px;
	height: 300px;
	margin: 0 15px;
	display: inline-block;
}

.img-sequence img {
	display: none;
}

.loading {
	position: relative;
	display: block;
	margin: 0 auto;
	width: 400px;
	box-sizing: border-box;
	border: 3px solid #FF0000;
	text-align: center;
}

.loading p {
	color: #FFFFFF;
	font-weight: 900;
	font-size: 2em;
	position: relative;
	z-index: 1;
}

.loading .progress {
	top: 0;
	left: 0;
	z-index: 0;
	background: #FF0000;
	width: 0%;
	height: 100%;
	display: block;
	position: absolute;
}
```


