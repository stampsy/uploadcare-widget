# History

### 0.17.2, 24.01.2013

* better compatibility with host page markup

### 0.17.1, 13.01.2013

* Large files uploads in parallel by small pieces with automatic recovering
  in case of network errors.
* Requests aborts after user cancels upload.
* Slightly reduced cpu usage during large files uploading.

### 0.17.0, 25.12.2013

* We now support large files uploads. Merry Christmas.

### 0.16.2, 16.12.2013

* Removing file from multiupload preview step no longer closes whole dialog.
  Bug introduced in 0.16.0.

### 0.16.1, 13.12.2013

* Widget.onChange now fires immediately after user chooses file.

### 0.16.0, 02.12.2013

* `uploadcare.openPanel()` method added. It allows open panel with tabs
  embedded in page (no modal mode).
* `uploadcare.registerTab()` method added. Now you can add custom tabs to
  dialogs and panels.
* jQuery version updated to 1.10.2. If you use `uploadcare.jQuery`, please
  check update guide http://jquery.com/upgrade-guide/1.9/
* spelling of `body.uploadcare-dragging` class fixed (it was draging). If you
  use this class, update your code.
* `uploadcare-dragging` class now appear on elements used as target for
  `receiveDrop` and `uploadDrop`

### 0.15.5, 25.11.2013

* Skydrive tab added.

### 0.15.4, 18.11.2013

* Box.com tab added.

### 0.15.3, 05.11.2013

* Fixed bug, do not allow set value while page loading.

### 0.15.2, 30.10.2013

* Widget's width can be easily changed in css.
* Css is now prepended to head, this allows overriding css rules without
  `important` keyword.

### 0.15.1, 17.10.2013

* Tiny replacement of jQuery UI sotrable plugin used. This saves about 12kb
  of gziped widget size for multiupload documents.

### 0.15.0, 16.10.2013

* New settings `clearable` allows user to remove uploaded file from widget.
  It is turned off by default.
* Widget does not cleared if user cancels dialog.

### 0.14.2, 15.10.2013

* Portuguese localization added.
* Minimum and maximum limits for number of files in MultipleWidget added.

### 0.14.1, 14.10.2013

* Chinese localization updated.

### 0.14.0, 11.10.2013

* French localization was added.
* Custom file's validators can be used to restrict user's choice.
* Undocumented method `fileInfo.dimensions()` was removed.
* Undocumented callback `Dialog.uploadDone` was removed.

### 0.13.5, 09.10.2013

* `uploadcare.filesFrom` function exposed in api.

### 0.13.4, 05.10.2013

* Fixed loading from url and social sources. Bug introduced in 0.13.3.

### 0.13.3, 03.10.2013

* Opening speed is significantly impoved for widget with hundreds of files
* Restored compatibility with IE8 and some Firefox versions

### 0.13.2, 30.09.2013

* Translations fixes

### 0.13.1, 26.09.2013

* widget size reduced from 341 to 293 kb (from 104 to 93 kb gziped)

### 0.13.0, 26.09.2013

* Widget no longer accepts urls in `value` HTML-attribute or `value()` method.
  You should use `widget.value(uploadcare.fileFrom('url', 'http://url/'))`.
* Widget now can be used with any custom domain.

### 0.12.5, 23.09.2013

* switch to preview tab right after selecting files
* prevent to request not ready images in multiupload preview

### 0.12.4, 16.09.2013

* `uploadcare.tabsCss` api fixed

### 0.12.3, 13.09.2013

* restrictions on the number of files in multiupload group removed

### 0.12.2, 12.09.2013

* fixed bug introduced in 0.12.0 related to loading info about already uploaded files

### 0.12.1, 12.09.2013

* crop options "upscale" and "minimum" also applicable to ratio
* built-in jQuery (version 1.8.3) now available in `uploadcare.jQuery`

### 0.12.0, 28.08.2013

* new property `originalImageInfo` of `fileInfo` object
* now you can use `fileInfo.cdnUrl` with all operations right after uploading
* traffic and preview delay significantly reduced for large images
* new option for crop — "minimum". Doesn't allows user to select area less
  then you specified

### 0.11.2, 13.08.2013

* add Chinese (Simplified) locale

### 0.11.1, 06.08.2013

* [drag and drop api](https://uploadcare.com/documentation/javascript_api/#drag-and-drop)
* [source tabs styling](https://uploadcare.com/documentation/javascript_api/#sources-style)
* widget size reduced from 455 to 346 kb (from 144 to 105 kb gziped)
* fixed bug when can't upload new file from uploadcare cdn url
* better compatibility with host page markup

### 0.10.1, 11.07.2013

* evernote is supported as a source of files
* if images_only is used, video thumbnails are loaded from the instagram
* fixed bug, preventing some of our clients from using uploadcare with AMD
