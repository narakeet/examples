# Animating images with Pan/Zoom effects 

This example shows how to animate images using Pan/Zoom (Ken Burns effect)  in Narakeet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

With an image larger than the video frame, you can control resizing using one of the available size property values, or shorthand values. 


The following five size values will produce a slight animation:

* `zoom` - zoom gradually in, the animation starts at full cover size
* `pan` - cover the video frame with the image, and then animate slightly moving to the specified position
* `panzoom` - combine pan and zoom at the same time
* `zoomout` - zoom gradually out, so that the animation starts zoomed in, and ends at full cover size
* `panzoomout` - combine zoom out and panning


With panning, you can control the direction of the pan using the image `position` property. Specify one of the edges (`top`, `left`, `bottom`, `right`) to move away from the center. 

For example, the following scene will animate an image by panning and zooming  to the left  at the same time

```md
![left panzoom](image.png)
```

You can combine multiple images in the same scene to produce a seamless animated slideshow.

## Available options

Check out the Narakeet [Available Sizing Options](https://www.narakeet.com/docs/format/#available-sizing-options) for images for an up-to-date list of all the sizing options.

## Image credits

Images in this example are by R Architecture on Unsplash <https://unsplash.com/@rarchitecture_melbourne>

