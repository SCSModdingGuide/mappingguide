# Editor backgrounds for custom modules

This tutorial teaches you how to make a custom editor background, the reference map image that appears in the editor when you press 'A'.

This part will describe how to take a map image and import it into the SCS Editor. A technique for getting high-resolution map images can be found in [part 1](1_imagery.md).

1. [Image size & format](#section1)
2. [Creating the material files](#section2)

<a name="section1"></a>
## 1. Image size & format

The editor background image needs to be a DDS format image with width and heights that are both divisible by 4.

Because our image is square, we'll use the game texture convention of using square numbers. (i.e. 512, 1024, 2048, 4096) Whilst images of 8192x8192 should work, I have experienced issues loading such large images in the editor, so you should use a 4096x4096 image to begin with before trying a larger image.

A DDS format plugin for Adobe Photoshop can be downloaded from the [NVIDIA developer site](https://developer.nvidia.com/nvidia-texture-tools-adobe-photoshop), and for free software both [Paint.NET](http://www.getpaint.net/index.html) and the [GNU Image Manipulation Program](https://www.gimp.org/) have built-in support for DDS.

Ensure that that the exported DDS file fits the dimension requirements, and is exported as DXT5. Mipmaps are not necessary for the image.

![Paint.NET canvas size adjustment](img/2_crop.png)
![Paint.NET export settings](img/2_dds.png)

You should now have a compatible image. You can copy our version from the GitHub repo [here](#).

<a name="section2"></a>
## 2. Creating the material files

Create a new mod folder (the working folder you create the .scs file from) called ```Malta``` and create a ```material\editor``` folder inside it. Paste your map DDS image in this folder. The name in this example is ```Malta.dds```.

as well as the image file itself, we also need:

- A texture information file
- A Material definition file

### Texture information file

It's not entirely certain why we need the .tobj information file, as they seem to be mostly blank, but we do need it. A program called [tobjEdit](http://www.mediafire.com/?zxlf5ta0ot7h0l1) has been written to create these files.

_Editor's note: tobjEdit originates from [haulinmods.com](http://www.haulinmods.com/), and is currently unsupported. In case this file is lost from its current host, I have mirrored the file [here](https://drive.google.com/open?id=0B1SFjX5JrmNUhpdXU1SG9TRjg)._
