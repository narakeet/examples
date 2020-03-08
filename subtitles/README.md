# Adding subtitles

This example shows how to add subtitles to videopuppet scenes.

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works

You can manually subtitle a scene by adding text in the subtitles property:

```yaml
scenes:
  - video: stopwatch.mp4
    subtitles: When shown over a video, subtitles match the duration
```

You can also automatically generate subtitles from narration by setting `subtitles: auto` as a global property for the video

```yaml
size: 720p
subtitles: auto
scenes:
  - ...
```

To show subtitles gradually, split the narration (or subtitles property if you are setting it manually) into a list:

```yaml
scenes:
  - image: london.jpg
    narration:
      - to show subtitles gradually
      - split narration into a list
```

