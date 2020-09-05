# Creating a video from animated GIFs 

This example shows how to include animated GIFs into videos using Narakeet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

Animated GIFs will automatically loop for the duration of the audio - just include them in the script as an image:

```md
![](arena.gif)
```

You can optionally make the GIF play one loop and stop on the last frame, using the `freeze` synchronization option in square brackets. For example:

```md
![freeze](arena.gif)
```

To loop a GIF without any narration, or for longer than the duration of the audio, just include a `pause` stage direction to the scene.


```md

![](arena.gif)

(pause: 5)
```

## Supported synchronisation options

Check out [Using Animated GIFs](https://www.narakeet.com/docs/format/#using-animated-gifs) for more information on scene synchronization options.
