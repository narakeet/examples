# Adding subtitles

This example shows how to add subtitles to Video Puppet scenes.

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

You can automatically generate subtitles from narration text by setting the `subtitles` property to `auto` in the script header:

```yml
---
size: 720p
subtitles: auto
---
```

You can also explicitly set the subtitles for a scene using Markdown block quotes (`>`), for example to add subtitles to a scene without narration, or to show something else on the screen instead of the narration text

```md

> Video Puppet will show this 

Video Puppet will read this

```

For scenes with longer narration, or to show subtitles gradually, split the text into paragraphs. 
