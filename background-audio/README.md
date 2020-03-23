# Video Puppet background sounds example 

This example shows how to add a background audio to Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

To add background music to your video, just provide a `background` top-level property in the page header. You can specify an audio file, or a combination of an audio file and volume separated by a space. The value should be a number reflecting the multiplier for the original volume (`1` is default, equal to the original volume).

You can use WAV, MP3 and M4A files. The sound will be automatically repeated to match the total duration of the video.

The following header will include `sound.wav` at full volume:

```yml
---
size: 720p
background: sound.wav
---
```

The following examples will include `sound.wav` at half volume:

```yml
---
size: 720p
background: sound.wav 0.5
---
```

## Related examples

You can use some royalty-free sounds provided by Video Puppet directly without uploading your own files. Check out the [Vendor Audio Example](../vendor-audio/README.md).
