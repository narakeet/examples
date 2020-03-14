# Video Puppet transitions example 

This example shows how to automatically apply transitions to video clips.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

To set transitions between scenes for the whole video, add the transition property in the script header. The following header will set a half-second wipe transition between the scenes.

```
---
size: 720p
transition:
  type: wipe
  duration: 0.5
---
```

You can also use a shortcut with the transition name and duration in a single line. For example, the following header will set a two second crossfade transition:
```
---
size: 720p
transition: crossfade 2
---
```


To set a transition for an individual scene, add it using the `transition` stage direction


```
![](london.jpg)

(transition: crossfade 2)
```

Note that the transition property combines the previous scene with the current scene, so any transition on the first scene is ignored.

## Available transition options

* `crossfade`: fade the last frame of the scene into the first frame of the next scene 
* `wipe`: horizontal overlay from the left 
