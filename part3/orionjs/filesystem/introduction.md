# Filesystem

The filesystem module is a unified upload system that keep track
of all the files that are uploaded to orion and use any provider
you want.

## Getting Started

Install filesystem

```sh
meteor add orionjs:filesystem
```

Install a provider 
(currently the only one is S3. 
To use S3 need to config some things, see [here](https://github.com/orionjs/s3))

```sh
meteor add orionjs:s3
```

## Uploading Files Through Filesystem

If you want to make an extension for orion and
you need to upload files, you **must** use this.

Example:

```js
var files = $('input').files;
var upload = orion.filesystem.upload({
  fileList: files,
  name: files[0].name
});
Tracker.autorun(function () {
  if (upload.ready()) {
    console.log(upload.fileId)
  }
});
Tracker.autorun(function () {
  var progress = upload.progress();
  console.log(progress);
});
```

### Removing Files

Example:

```js
var fileId = 'The id of the file';
orion.filesystem.remove(fileId);
```