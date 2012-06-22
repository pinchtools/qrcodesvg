qrcodesvg
=========

http://vp-dev.net/qrcodesvg/

Create personalized Qr Code in Javascript.
Qrcodesvg allow you to create beautiful QrCode on client-side.

You can apply colors and effects to your QrCode. 

Qrcodesvg is based on Raphael.js a javascript library for generating vector graphic.
You can grap the latest version here : http://raphaeljs.com/



## Compatibility

Tested on : Firefox 13.0, Chrome 19, IE 8.


## Features
Set an ecclevel for data redundancy

Apply one or many colors to squares or patterns

Add round or bevel effect to squares or patterns

Add a background and a frame.



## Examples


### Basic example

```html
<!DOCTYPE html>
<html>
  <head>
		<script type="text/javascript" src="raphael-2.1.0-min.js"></script>
		<script type="text/javascript" src="qrcodesvg.js"></script>
  </head>
  <body>
  	<div id="qrcode" ></div>
  	
	<script type="text/javascript">
			//create a Qrcode in 250x250 with input 'Testing' in the HTMLElement 'qrcode'
			var qrcodesvg 	= new Qrcodesvg( "Testing Qrcodesvg", "qrcode", 250);
	
			qrcodesvg.draw();
   	</script>
  </body>
</html>
```


### QrCode With Options
```html
<!DOCTYPE html>
<html>
  <head>
		<script type="text/javascript" src="raphael-2.1.0-min.js"></script>
		<script type="text/javascript" src="qrcodesvg.js"></script>
  </head>
  <body>
  	<div id="qrcode" ></div>
  	
	<script type="text/javascript">
			var qrcodesvg 	= new Qrcodesvg( "Testing Qrcodesvg", "qrcode", 250, {"ecclevel" : 1});

			//add a bevel effect on patterns with a radius of 5.
			//apply one of these three colors to patterns
			qrcodesvg.draw({"method":"bevel", "radius" : 5, "fill-colors":["#1C46ED","#021872","#0125C4"]}, {"stroke-width":1});
   	</script>
  </body>
</html>
```

### More Examples.

See mor example in test.html file.

You will see all the available options.



And don't forget to test your Qrcode !







