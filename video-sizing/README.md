# Video Puppet video sizing example 

This example shows how to automatically resize video clips to fit the output format in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

When adding a video to a scene, Video Puppet will automatically resize it to fit the target video format. You can control resizing by adding an option to the square brackets when setting the video. For example, to shrink and pad a larger video to fit the smaller target size, use the `contain` option:

```md
![contain](birds.mp4)
```

Alternatively, you can provide a `video` stage direction in brackets, and add the `size` option in subproperties. When adding subproperties, indent them with two spaces or a tab. (Technically, stage directions are in YAML format).

```
(video:
  file: birds.mp4
  size: contain)
```

## Available sizing properties

Check out [Scene videos](https://videopuppet.com/docs/format/#videos) for more information on scene video sizing options

