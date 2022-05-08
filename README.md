# libpngu-mod
A library for Wii and GameCube that "wraps" libpng, facilitating PNG handling and conversions to the native Wii/GC formats.

libpngu-mod is based on [libpngu](https://wiibrew.org/wiki/PNGU) with [GRRLIB patches](https://github.com/GRRLIB/GRRLIB/tree/master/GRRLIB/lib/pngu).

## Features
* Works with the latest libpng (1.6.37 as of writing)
* Handles images of 8 and 16 bits per channel
* Handles images in RGB, RGBA, grayscale and grayscale + alpha formats
* Reads image dimensions, pixel format, background color and transparent colors list
* Converts images to YCbYCr, linear RGB565, linear RGBA8, 4x4 RGB565, 4x4 RGB5A3 and 4x4 RGBA8 formats
* Saves YCbYCr images in png RGB8 format
* Handles images stored in memory or in devoptab devices (SD, USB, SDGecko, etc...)
* Ready to be used in multithreaded applications

## Limitations
* Image width and height should be a multiple of 4
* Doesn't handle images of 1, 2 or 4 bits per channel
* Doesn't handle paletted images
