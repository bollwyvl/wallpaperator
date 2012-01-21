# Wallpaperator: HTML5 Wallpaper Generator for E-Readers, Smartphones, etc.
![Concept Screenshot](/bollwyvl/wallpaperator/raw/master/ux/screenshot.png)

## Motivation
The other day, I was trying to build a screensaver set for my e-reader. Given the inflexibility of the display, and the quality of scaled images, it became clear that, even with great Gimp-fu, I would still be stuck doing a lot of work to make the shots look the way I wanted: resolution, color depth, etc.

## Inspiration
There are a number of browser-based image resizing tools, but they are:

- not easy to use for constrained sizes
- covered in ads
- doing a lot of juggling on the server, and I don't know what they do with my images... not so good for home photos
- not good for preparing a series of images with the same constrained sizes

## Approach
Build a browser-based image manipulation tool which is device-aware. Allow user to load images from their local machine, or provide a URL. Allow for the generation of zipped sets of images. Save "projects" as a shareable/reloadable file (including the raw source image data) for tweaking after the fact.

## Libraries
- [three.js][3j] for image loading, etc. see [Rutt-Etra-Izer][rei] for file drop, image rendering, 
- [twitter bootstrap][tb] for the web app frame, buttons, etc.
- [jszip][jz] for generating zips of multi-image projects

## Nice to haves
- [Apply effects][fx]: make an image like the woodcuts on Nook and Kindle with THREE.ShaderExtras

[3j]: http://github.com/mrdoob/three.js
[tb]: http://twitter.github.com/bootstrap/
[jz]: http://jszip.stuartk.co.uk/
[rei]: http://airtightinteractive.com/demos/js/ruttetra/
[fx]: http://mrdoob.github.com/three.js/examples/webgl_postprocessing.html