# Narakeet slide CSS themes

This example shows how to create slide themes with CSS, in Narakeet.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

You can customise the visual look and feel of a slide by creating a CSS file, and using it as the slide theme. To set the theme globally for all slides in the video, use the theme header:

```md
---
theme: custom.css
---

~~~md
Some slide content
~~~
```

You can also set the theme for a specific scene using the `theme` stage direction

```md
---

(theme: custom.css)

~~~md
theme for this scene only
~~~

---
```

For more information, check out the [theme format reference](http://www.narakeet.com/docs/format#theme).
