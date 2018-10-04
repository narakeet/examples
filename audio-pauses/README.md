# Video Puppet audio pauses example

This example shows how to add a narration pause in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the `script` directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works


Stage directions for narration are paragraphs with keywords such as `pause` in brackets. You can add a multi-paragraph narration and use the `pause` stage direction to stop the speech for a bit. For example:

```yml
scenes:
  - image: london.jpg
    narration: |
      This is the first sentence, and we'll pause for a bit after it.

      (pause: 3)

      This is the second sentence
```

Note the pipe symbol `|` -- this is a way to create multi-line text in YAML while preserving line breaks.

