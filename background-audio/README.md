# Video Puppet background sounds example 

This example shows how to add a background audio to Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

To add background music to your video, just provide a `background` top-level property in the page header. You can specify an audio file, or a combination of an audio file and volume (in which case, use the `audio` and `volume` subproperties).

You can use WAV and MP3 files. The sound will be automatically repeated to match the total duration of the video.

```yml
---
size: 720p
background:
    audio: 0ff22a15475e27fcc200f6d618a9-orig.wav
    volume: 0.3
---
```

## Related examples

You can use some royalty-free sounds provided by Video Puppet directly without uploading your own files. Check out the [Vendor Audio Example](../vendor-audio/README.md).
