Google Fastbutton
=================

When clicking a element that triggers javascript on a mobile device they wait 300ms to 
see if the user is going to preform a dubble tap (zooming in). Google fastbutton is a method to avoid 
this 300ms delay.

This javascript file is basicly the google fastbutton class ready for use.


Basic usage
===========

To start creating fast buttons, first import the javascript.

	<script src='js/google-fastbutton-min.js'></script>

For each button you want to apply the method to, create a new instance specifying the button element and the handler

	new FastButton(document.getElementById('fast_button'), function(){
		alert('works');
	});


######Little tip

For better control over your fast buttons you could create a function which
creates a new fast button instance like so:

  Object.prototype.makeFastButton = function(handler){

    if(typeof FastButton !== 'function'){
      return console.error('Google fastbutton class not found');
    }

    new FastButton(this, handler);

  };

This way you have better control over what happens when creating new fast buttons without having to 
touch the google-fastbutton javascript file.


