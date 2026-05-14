# jpgbeauty

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A client-side tool to resize and compress large JPG and PNG files for the web. All processing happens in your browser; no files are uploaded to a server.

## Demo

**https://github.com/code4fukui/jpgbeauty

## Features

-   **In-Browser Processing:** Optimizes images securely on your machine without server uploads.
-   **Batch Conversion:** Drag and drop multiple files to process them all at once.
-   **Smart Resizing:** Reduces image dimensions to a specified maximum width or height.
-   **PNG to JPEG Conversion:** Automatically converts PNG files to JPEG if they exceed size or dimension limits.
-   **Quality Control:** Adjust the JPEG compression quality (from 0.0 to 1.0).
-   **Color Space Management:** Optionally force conversion to the sRGB color space for web compatibility.
-   **File Size Limit:** Triggers conversion for images that exceed a specified kilobyte threshold.
-   **Automatic Download:** Downloads a single optimized image directly, or bundles multiple images into a ZIP archive.

## Usage

1.  Drag and drop one or more JPG or PNG files onto the drop zone on the page.
2.  Adjust the settings as needed:
    -   **Max width/height (px):** The maximum pixel dimension for the output image's width or height.
    -   **Quality (0-1.0):** The JPEG quality for converted images. `1.0` is highest quality.
    -   **Force sRGB:** Check the box to ensure the output image uses the sRGB color space.
    -   **Max size (kbyte):** Images larger than this will be re-compressed.
3.  The processed files will be downloaded automatically. If you dropped multiple files, they will be saved as a single `jpgs.zip` file.

## Dependencies

This application is built with the following open-source libraries:

-   [ImageUtil.js](https://github.com/code4fukui/ImageUtil) - Core image manipulation utilities.
-   [exif-js](https://github.com/taisukef/exif-js) - For reading EXIF metadata from images.
-   [downloadZip.js](https://github.com/code4sabae/js/blob/master/downloadZip.js) - For creating and downloading ZIP archives.
-   [waitDropFiles.js](https://github.com/code4sabae/js/blob/master/waitDropFiles.js) - For handling file drag-and-drop events.
-   [downloadFile.js](https://github.com/code4sabae/js/blob/master/downloadFile.js) - For triggering single file downloads.
-   [readAsArrayBufferAsync.js](https://github.com/code4sabae/js/blob/master/readAsArrayBufferAsync.js) - For reading local files asynchronously.
-   [Bootstrap](https://getbootstrap.com/) - For UI styling.

## License

MIT License — see [LICENSE](LICENSE).