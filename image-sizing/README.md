# Narakeet image sizing example 

This example shows how to automatically resize images to fit the output format in Narakeet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

When adding an image to a scene, Narakeet will automatically resize it to fit the target video format. You can control resizing by adding an option to the square brackets when setting the video. For example, to shrink and pad a larger image to fit the smaller target size, use the `contain` option:

```md
![contain](image.png)
```

Without additional options, Narakeet will crop a large image around the center to cover the video size. If you want to show a different part of the image, specify the cropping position. For example, the following scene takes the left part of an image instead of the center:


```md
![left](file.png)
```

For available sizing and position options, check out [Scene Image](/docs/format/#images) documentation.




