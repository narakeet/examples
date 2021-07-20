# Adding subtitles

This example shows how to add subtitles to Narakeet scenes.

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

You can automatically generate subtitles from narration text by setting the `subtitles` property to `overlay` in the script header:

```yml
---
size: 720p
subtitles: overlay
---
```

You can also explicitly set the subtitles for a scene using Markdown block quotes (`>`), for example to add subtitles to a scene without narration, or to show something else on the screen instead of the narration text

```md

> Narakeet will show this 

Narakeet will read this

```

This trick also works to remove subtitles from a scene where you do not want them.

```md

This sentence will not be shown in the subtitles, because of an empty
subtitle block below.

>

```
