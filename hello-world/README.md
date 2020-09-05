# Basic Narakeet example

This example shows how the basic features of Narakeet.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

Narakeet creates a video from one or scenes. Each scene can include videos, images, audio or narration. 

### Adding images and videos

In the Markdown script file format, you can add images or videos by using the standard Markdown syntax (`![](file)`). 

```md
![](london.jpg)
```

### Adding narration

Narakeet automatically generates narration from scene text. The following scene will include an image, and automatically generated voice narration:

```md
![](london.jpg)

Welcome to London
```

### Using your audio

Instead of automatically generated narration, you can add your own audio files, with recorded voice, music or something else to play during a scene. To do so, just add `(audio: file)` in a separate paragraph. For example, this scene will show an image from `london.jpg` and play the audio from `london-audio.mp3`:

```md
![](london.jpg)

(audio: london-audio.mp3)
```

### Adding scenes

To add more scenes, use three or more dashes (`---`) as a separator. The following script file creates two scenes:

```md
![](london.jpg)

Welcome to London

---

![](berlin.jpg)

Welcome to Berlin
```

## More examples

Next, check out the [voices](../voices/README.md) example to see how to control the narration voice, or the [subtitles](../subtitles/README.md) example for information on how to generate subtitles for your video.
