# Synchronising audio and video using Video Puppet  

This example shows how to automatically adjust a scene duration with a video and audio track. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works

Instead of specifying `video` directly with a filename, make it a key-value map and set the asset file name in the `file` sub-property. Then set the `sync` property to one of the following three options:

* `freeze`: (default) keeps the last video frame frozen to wait for audio to finish, but does not speed up or shorten the video if longer than audio
* `match`: speed up or slow down the video to match the audio track length
* `trim`: keep the original video speed, but stop the scene when either the video or the audio end. This will also cut off any remaining audio if the video is shorter.

```yaml
scenes:
  - narration: >
      this is a very long narration, so we'll get the video to 
      slow down so it can match the length of this talk.
  - video:
    file: stopwatch.mp4
    sync: match
```
