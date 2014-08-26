Google Fastbutton
=================

When clicking an element that triggers JavaScript on a mobile device there is a 300ms delay to see if the you are going to preform a double tap (zooming in). Google Fastbutton is a method to avoid this 300ms delay.

google-fastbutton.js is basicly the [google fastbutton](https://developers.google.com/mobile/articles/fast_buttons) library ready-to-use.

## Basic usage

To start creating fast buttons, first import the required JavaScript.

    <script src='js/google-fastbutton-min.js'></script>

For each button you want to apply the method to, create a new instance specifying the HTML element and the handler function.

	new FastButton(document.getElementById('fast_button'), function(){
		console.log('works');
	});


