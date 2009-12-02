PassShark
===========

PassShark.js is a free and easy-to-implement *password masking* class developed
using MooTools. Inspired and based on the excellent iPhone and iPod touch 
password dialogue.

![Screenshot](http://github.com/Rendez/PassShark/blob/master/Docs/screenshot1.png)

How to use
----------

	#JS
	window.addEvent('domready', function(){
        new PassShark('sample_pass',{
            interval: 200,
            duration: 2000,
            replacement: '%u25CF',
            debug: false
        });
    });
	#HTML
	<head>
		//  1_ Include MooTools-Core and MooTools-More* in your document head
		<script type="text/javascript" charset="utf-8" src="Mootools-Core.js"></script>
		<script type="text/javascript" charset="utf-8" src="Mootools-More.js"></script>

		// 2_ Include the PassShark script in your document head
		<script type="text/javascript" charset="utf-8" src="PassShark.js"></script>
	</head>
	<body>
	[...]
		<label for="sample_pass">Password</label> <!-- Label is optional but recommended -->
		<input type="password" id="sample_pass" name="password" />
	[...]
	</body>

Screenshots
-----------

![Screenshot 1](http://github.com/Rendez/PassShark/blob/master/Docs/screenshot1.png)

Acknowledgements
-----------------

* Features and Compatibility
	* Written in MooTools. Requires -Core version 1.2.4 + and -More 1.2.4.2 +.
	* Tested on Safari 3+, Firefox 3+, Opera 10+, Internet Explorer 6 and 7.
	* No need to modify your original HTML. The password field is automatically found by type (input type="password").
	* Unobtrusive: users with Javascript deactivated still get the standard 'masked' password field.
	* Supports copy & paste.

* Notes
	* The "onStateChange" event is commented so that the activate() and deactivate() methods, when implemented, can be executed with fireEvent() if needed.

* PassShark with MooTools resolves many issues found in other implementations:
	* Inability to use ' (apostrophe) characters.
	* The cursor would move to the end on any key stroke, especially annoying 
if the cursor is elsewhere.
	* When converting the last character-to-symbol with the a duration delay, the input
field is focused, which is irritating if the input field is previously unfocused (blur).
	* Errors on deletion of the original field value, which is highly unsafe.
	* Deleting a multiple character selection would cause the same errors as stated
above and others.
	* Deleting a single character wouldn't work if the character was not the last one.

* Known issues
	* None

* License
	* PassShark is released under the Open Source MIT license.