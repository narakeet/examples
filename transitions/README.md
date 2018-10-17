# Video Puppet transitions example 

This example shows how to automatically apply transitions to video clips.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works

Add a `transition` property to the scene, and set the `type` and `duration` sub-properties. 

Duration is a number, the duration of the transition in seconds, and must be between 0.1 and 60.

Currently supported types are:

* `crossfade`: fade the last frame of the scene into the first frame of the next scene 
* `wipe`: horizontal overlay from the left 

Note that the transition property combines the previous scene with the current scene, so any transition on the first scene is ignored.

```yaml
scenes:
  - video: 
      file: birds.mp4
  - video: 
      file: stopwatch.mp4
    transition:
      type: crossfade
      duration: 0.5
```
