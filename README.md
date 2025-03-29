# Exif.js

* == JavaScript library / read image files' [EXIF & IPTC meta data](https://en.wikipedia.org/wiki/Exchangeable_image_file_format)
  * EXIF logic here -- is based on the -- [EXIF standard v2.2](/spec/Exif2-2.pdf)
  * use cases
    * images | browser
    * image or file input element
  * ALLOWED uses
    * AMD environments or
    * CommonJS environments

* EXIF standard
  * uses
    * ONLY | `.jpg` & `.tiff` images

## How to install?
* ways
  * `npm install exif-js --save`
  * `bower install exif-js --save`
    * [Bower](http://bower.io/)

## How to use?
* add as script
  * ways
    * ALL 
      ```html
      <script src="vendors/exif-js/exif-js"></script>
      ```
    * minified version
      ```html
      <script src="https://cdn.jsdelivr.net/npm/exif-js"></script>
      ```
  * call `EXIF.getData()`
