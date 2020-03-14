# Synchronising audio and video using Video Puppet  

This example shows how to automatically adjust a scene duration with a video and audio track. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

When specifying a video resource, you can include a synchronization option in square brackets. For example, this loops the video for the duration of the audio in the scene:

```md
![loop](stopwatch.mp4)
```

Alternatively, you can provide a `video` stage direction, and specify the `sync` sub-property. When adding subproperties to a stage direction, indent them by two spaces or a tab. (Technically, a stage direction is in YAML format).

```
(video:
  file: stopwatch.mp4
  sync: loop)
```

## Supported synchronisation options

Here are the available synchronisation options:

* `freeze`: (default) keeps the last video frame frozen to wait for audio to finish, but does not speed up or shorten the video if longer than audio
* `match`: speed up or slow down the video to match the audio track length
* `trim`: keep the original video speed, but stop the scene when either the video or the audio end. This will also cut off any remaining audio if the video is shorter.
* `loop`: repeat either the video or the audio to match the longer asset duration

