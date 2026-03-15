# jpgbeauty

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

Large JPG files can be resized for web publishing (supports batch conversion, no server upload required).

## Demo
https://code4fukui.github.io/jpgbeauty/

## Features
- Resize JPG and PNG files to a maximum width/height
- Adjust image quality
- Optionally force sRGB color space
- Limit maximum file size

## Usage
1. Drag and drop JPG or PNG files onto the page.
2. Adjust the settings as needed (max width/height, quality, sRGB, max size).
3. The resized files will be downloaded as a ZIP archive.

## Dependencies
The app uses the following open-source libraries:
- [downloadZip.js](https://github.com/code4sabae/js/blob/master/downloadZip.js)
- [waitDropFiles.js](https://github.com/code4sabae/js/blob/master/waitDropFiles.js)
- [downloadFile.js](https://github.com/code4sabae/js/blob/master/downloadFile.js)
- [readAsArrayBufferAsync.js](https://github.com/code4sabae/js/blob/master/readAsArrayBufferAsync.js)
- [ImageUtil.js](https://github.com/code4fukui/ImageUtil)
- [exif-js](https://github.com/taisukef/exif-js)

## License
MIT License