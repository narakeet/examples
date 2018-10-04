# Video Puppet slides 

This example shows how to create slides with text, optionally adding them on top of images, in Video Puppet.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works

You can use the `slide` property of a scene to create a textual slide:

```yaml
scenes:
  - slide: Let's talk about penguins
```

If you also have an image in the same scene, Video Puppet will darken it a bit to show the text more clearly:

```yaml
scenes:
  - slide: Let's talk about penguins
    image: penguin.jpg
```

If there is no audio or narration in the slide, the standard duration on screen will be 1 second. To make the scene longer, add a `duration` property, and specify the number of seconds to keep the text on screen.

```yaml
scenes:
  - slide: Let's talk about penguins
    image: penguin.jpg
    duration: 5
```

You can easily add multi-line text and style it in Markdown. Remember to use the pipe symbol (`|`) to signal multi-line text where line breaks are preserved:

```yaml
scenes:
  - duration: 2
    slide: |
      # Heading 1
      ## Heading 2
      
      * bullets are left-aligned
      * bullet 2
        * sub-bullet
```

Syntax highlighting also works, for example this is how to automatically highlight CSS syntax:

~~~yaml
scenes:
 - slide: |
      Syntax highlighting
      ``` css
        .container {
          align-items: center;
          display: flex;
          justify-content: center;
          height: 100%;
          width: 100%;
          padding: 40px;
        }
      ```
    duration: 2
~~~
