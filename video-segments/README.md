# Extracting video segments using Video Puppet  

This example shows how to add parts of a video to a scene. This is useful in cases where you made a longer screen recording, but only want to use certain pieces of it in your video.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works

Instead of specifying `video` directly with a filename, make it a key-value map and set the asset file name in the `file` sub-property. Then set the `segment` in the `MM:SS - MM:SS` format to extract just a piece of the video:

```yaml
scenes:
  - video:
    file: stopwatch.mp4
    segment: 00:02 - 00:04
```


You can also extract a still image of the start or end of a video using the special `start` and `end` segment values:

```yaml
scenes: 
  - video:
      file: stopwatch.mp4
      segment: end
    narration: Use the end segment to show the last frame of a video.
  - video:
      file: stopwatch.mp4
      segment: start
    narration: Use the start segment to show the first frame of a video.
```
