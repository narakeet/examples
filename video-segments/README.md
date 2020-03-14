# Extracting video segments using Video Puppet  

This example shows how to add parts of a video to a scene. This is useful in cases where you made a longer screen recording, but only want to use certain pieces of it in your video.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

To show only part of a video in a scene, specify it as a stage direction instead of the markdown resource, and include the `segment` subproperty:

```
(video:
  file: stopwatch.mp4
  segment: 00:02 - 00:04)
```

When specifying a complex stage direction, indent subproperties with two spaces or a tab. (Technically, stage directions are in YAML format surrounded by brackets). 

You can also extract a still image of the start or end of a video using the special `start` and `end` segment values.

```
(video:
  file: stopwatch.mp4
  segment: end)
```
