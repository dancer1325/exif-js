* `var Exif = function(obj) {}`
  * `EXIF.getData = function(img, callback) {}`
    * ALLOWED `img`
      * -- from -- `<img src="image.jpg">`
      * | page's `<input type="file">`
    * `callback` 
      * recommendations
        * if you want to access the image / aforementioned metadata -> use `this`  
    * requirements
      * ⚠️load COMPLETELY the image BEFORE ⚠️
        * OTHERWISE, it will fail
        * ways
          * run your exif-extracting logic | 
            * | `window.onLoad`
            * if you use jQuery -> use `$(window).load()`
              * rather than `$(document.ready()`
                * Reason: 🧠it fires BEFORE images are loaded 🧠
          * image's own `onLoad` function
  * `EXIF.getTag(img, tag)`
    * == get tag 
  * `EXIF.Tags`
    * == ALLOWED tag names
  * `EXIF.TiffTags`
    * == ALLOWED Tiff tag names
  * `EXIF.pretty(img): string`
    * return ALL EXIF information / pretty printed
  * `EXIF.enableXmp();`
    * enable extracting XMP data
    * how to use?
      * BEFORE using `EXIF.getData()`
  * `EXIF.readFromBinaryFile(file)`
    * from [File/Blob](https://developer.mozilla.org/en/docs/Web/API/Blob) object -> get image data
  * TODO:
* `exifdata`
  * == EXTRA image's property 
  * 👀== Javascript object / has EXIF metadata 👀
    * _Example:_ image caption, date / photo was taken, orientation 