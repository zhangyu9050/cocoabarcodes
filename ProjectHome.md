![http://img508.imageshack.us/img508/6634/barcodewelcomecv6.gif](http://img508.imageshack.us/img508/6634/barcodewelcomecv6.gif)

Cocoa Barcodes is a set of classes (and a test application) for generating two-dimensional barcodes. It supports many of the more common one-dimensional linear barcodes in use today, allows you to export a barcode as a TIFF, EPS, or PDF image, to copy the barcode image to the pasteboard, or to drag it to any other application that accepts standard OS X PDF data from the pasteboard, including TextEdit. You can also print barcodes directly to any supported printer. Please note that you may not be able to create readable barcodes at all bar widths allowed by a specification. For example, Code 3 of 9 allows a bar width of as small as 7.5 mils, but I haven't had much luck going smaller than 13 mils on ink jet printers.

You have a fair amount of control over the final appearance of the barcode, including the bar width (in 1/10 mil increments), bar height, font size, and captioning. The following barcode types are supported:

  * Code 3 of 9
  * Extended Code 3 of 9
  * Code 128
  * Interleaved 2 of 5
  * Industrial 2 of 5
  * Codabar
  * PostNet
  * Modified Plessey
  * Modified Plessey (hexadecimal)
  * UPC-A
  * UPC-E
  * EAN-13
  * EAN-8
  * Royal Mail Barcode (also known as RM4SCC or CBC)
  * Planet Barcode
  * Japan Post Barcode


Cocoa Barcodes is based on Barcode Generator, an open source Mac program which began its life as a test scaffold for a set of Cocoa classes I was writing. I did not initially intend to release it as a standalone program, but by the time I was done testing the code, it had the lion's share of the features available on other OS X barcode programs at the time so I decided to release it.

I intend to add iPhone support at some point, but currently, drawing the barcodes is accomplished using categories on NSView and NSImage, neither of which are available on the iPhone.