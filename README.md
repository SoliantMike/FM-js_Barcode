FM-js_Barcode
===========
A question posed in the FileMaker Community asked if there was a way to save an image generated from Javascript and save it in a container field. This solution uses code from the Github repository of Johan Lindell, linked below.

Since storing as an image in a container field allows for clean printing in all platforms that FileMaker supports, this is a preferred way to generate and store barcodes. There is also nothing to install on client machines like 3rd party plugins or fonts to maintain. 

Github Project used here:
https://github.com/lindell/JsBarcode

Also note that some barcode types may have requirements on the values they can represent, such as EAN type must be a 13 digit number. See the documentation for the barcode type you are using before implementing in your solution.

Added better support for Windows version where long URLs are not supported and may fail. Note that this uses the user clipboard to transfer data from the web viewer to a field.

Updated for FileMaker 16 with security setting to allow for fmpurl protocol.

Read more here:
http://www.soliantconsulting.com/blog/2017/06/filemaker-16-javascript-changes