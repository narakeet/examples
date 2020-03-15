# Video Puppet slides 

This example shows how to create slides with text, optionally adding them on top of images, in Video Puppet.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

You can use Markdown code blocks (fenced with three backticks or three tildas) to create a textual slide:

~~~
```
Hi there!
```
~~~

In case there is also an image or a video in the same scene, Video Puppet will show the slide over the scene, with a dark backdrop shadow to create contrast between the text and the background. This works well if the image or video behind the slide is mostly in light colours. 


For darker images or videos,  set the slide theme to `light` using the theme stage direction, to switch to lighter colors in the slide.

~~~
(theme: light)


```
Start counting!
```

![](stopwatch.mp4)

~~~


If there is no audio or narration in the slide, the standard duration on screen will be 1 second. To make the scene longer, add a `duration` stage direction, and specify the number of seconds to keep the text on screen.


~~~
```
Penguins!
```

![cover](seaside.jpg)

(duration: 2)
~~~

## Rich text slides

You can render rich text on slides by using markdown syntax, and marking the slide as markdown content by appending `md` after the opening code fence:

~~~
```md
# Heading 1
## Heading 2

* bullets are left-aligned
* bullet 2
  * sub-bullet
```
~~~

## Syntax highlighting

If you want to include code snippets as slides, Video Puppet will automatically support syntax highlighting as long as you specify the language after the opening code fence.

~~~
```css
.container {
  align-items: center;
  display: flex;
}
```
~~~

## Controlling font size

By default, Video Puppet sets the font for slides to relatively large (50px) to show clearly on smaller screens. For slides with a lot of text, you can set the size using the `(font-size)` stage direction. Set the value to an integer number of pixels.

~~~
(font-size: 20)

```css
.container {
  align-items: center;
}
```
~~~

