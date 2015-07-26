# UploadPreview
Upload Preview down to IE7 (partially)
By partially, it means it doesn't support checking file size on ie 7,8,9 as I would require clients side ActiveX or flash
This plugin is mainly for preview image before uploading on both old IE browser and modern browser.

Requirement
=============================
Jquery (1.4+)
php as Backend?

Base Usage
=============================
$("input[name=preview]").uploadpreview({
	div: ".preview",
	imgwidth: 180,
	imgheight: 120
});
* 1.Input element doesn't have name attribute it will throw error
* *1.1. Name attribute need to end with [] so that php understands it an array
* 2.it will throw error if div option is not declared
* 3. imgsize option will not take effect on IE 7, 8, 9
* 4. As it will automatically generate new input element, php will always receive the first index to be empty because the newly generated input element hasn't had any selected file yet

Browser Support
=============================
IE: 7+

Chrome: 6

FireFox: 3+ ?

Opera: 11.5+

Others: Check http://caniuse.com/#search=file%20api For More File API
