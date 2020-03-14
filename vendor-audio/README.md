# Video Puppet provided backgrounds 

This example shows how to add a one of the standard background sounds to your video using Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

Similar to adding your own background music to the video, provide a `background` top-level property. Instead of the `audio`  subproperty, use a `vendor` subproperty and choose one of the supported background sounds.

You can also set the `volume` sub-property, controlling the relative volume of the sound in the file. The value should be a number reflecting the multiplier for the original volume (`1` is default, equal to the original volume).


```yml
---
size: 720p
background:
  vendor: ukulele-1
  volume: 0.5
---
```

## Supported audio names

* `ukulele-1` - Easy-listening, melodic music
* `ukulele-2` - Simpler easy-listening background, without the melody
* `corporate-1` - A corporate sound for business presentations
* `uplifting-1` - An uplifting electronic sound
* `uplifting-2` - A more dynamic uplifting electronic sound

## Related examples

You can use your own background sounds Check out the [Background Audio Example](../background-audio/README.md).
