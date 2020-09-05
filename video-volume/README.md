# Narakeet video volume example

This example shows how to automatically adjust the volume of embedded videos in Narakeet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

When adding a video to a scene, Narakeet can adjust the volume. You can set a numerical volume multipler in a stage direction:



```
(video:
  file: tube.mp4
  volume: 0.5)
```

You can also set the volume `mute` (equivalent to 0). This is particularly useful as a shortcut because you can use it in markdown properties, for example

```md
![mute](tube.mp4)
```

## More information 

Check out [Scene videos](https://www.narakeet.com/docs/format/#videos) for more information on scene video options.

