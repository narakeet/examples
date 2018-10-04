# Basic Video Puppet example

This example shows how the basic features of Video Puppet.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works


A Video Puppet script is a simple key-value file. You can use YAML or JSON. The simplest structure has a:
* `size` property specifying the dimensions of the video (`720p` is a standard size for 16x9 videos usual on Youtube and social networks, but you can also use values in the `Width x Height` format, for example `800x600`)
* a list of one or more `scenes`, each containing assets to show.

Here is a very simple example, adding just an image to the scene:

```yaml
size: 720p
scenes:
  - image: london.jpg
```

Video Puppet can automatically generate narration from text, using a life-like audio track:

```yaml
size: 720p
scenes:
  - image: london.jpg
    narration: Welcome to London
```

Add additional scenes by creating more elements in the list:

```yaml
size: 720p
scenes:
  - image: london.jpg
    narration: Welcome to London
  - image: berlin.jpg
    narration: Welcome to Berlin
```

If you want to use your own voice, just add the `audio` sub-property:
  
```yaml
size: 720p
scenes:
  - image: london.png
    audio: london-audio.mp3
```

You can also provide videos as scenes:

```yaml
size: 720p
scenes:
  - video: my-first-scene.mp4
  - video: my-second-scene.mp4
```

Check out the [Video Segments](../video-segments) example to see how to extract just parts of a video from a file.

