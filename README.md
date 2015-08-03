angular-cropper
===============

> Touch-enabled image cropper for AngularJS

[Demo](http://plnkr.co/edit/s96ZCYmP5ELtqdIMieKC?p=preview)

### Get it
```sh
$ bower install angular-cropper
```

or

```sh
$ npm install angular-cropper
```

### Use it
* Include files in your html
  * `bower_components/angular-file-reader/angular-file-reader.js`
  * `bower_components/angular-cropper/angular-cropper.js`
* Include `tw.directives.cropper` in your module dependencies
  * `angular.module('myApp', ['tw.directives.cropper']);`
* Place the `tw-cropper` attribute on a canvas
  * `<canvas width="300" height="300" tw-cropper="cropper"></canvas>`
* Give your cropper a `source`
  * `<canvas width="300" height="300" tw-cropper="cropper" source="myFile"></canvas>`
  * `source` must be a File
  * See the demo for one way to get a File to your scope
  * Or use [twhitbeck/angular-file-input](https://github.com/twhitbeck/angular-file-input)
* Get the dataURL of your crop with controller `toDataURL` method
  * `<button ng-click="upload(cropper.toDataURL())">Save</button>`
* That's it!
