# Video Puppet image sizing example 

This example shows how to automatically resize images to fit the output format in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

When adding an image to a scene, Video Puppet will automatically resize it to fit the target video format. You can control resizing by adding an option to the square brackets when setting the video. For example, to shrink and pad a larger image to fit the smaller target size, use the `contain` option:

```md
![contain](image.png)
```

Without additional options, Video Puppet will crop a large image around the center to cover the video size. If you want to show a different part of the image, specify the cropping position. For example, the following scene takes the left part of an image instead of the center:


```md
![left](file.png)
```

## Available sizing options

* `fit`: image will be rescaled without keeping the proportions
* `contain`: image will be completely visible, and padded if necessary with black bars to fit the output frame
* `cover`: (default) image will be scaled so it completely covers the output frame, and cropped if necessary to keep the proportions

## Available position options

* `center`: (default) crop image around the vertical and horizontal middle
* `top-left`: crop the image so the top-left corner aligns with the top-left of the video
* `left`: crop the image so the left edge of image aligns with the left edge of the video, and center image vertically
* `right`: crop the image so the right edge of image aligns with the right edge of the video, and center image vertically
* `top`: crop the image so the top edge of image aligns with the top edge of the video, and center image horizontally
* `bottom`: crop the image so the bottom edge of image aligns with the bottom edge of the video, and center image horizontally




