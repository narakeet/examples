# Video Puppet audio pauses example

This example shows how to add a narration pause in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works


You can specify a pause in narration by turning the narration element from a string into an object, and providing the `pause` property. 

```yml
scenes:
  - slide: only a pause
    narration:
      pause: 2
```

To insert a pause between sentences, turn the narration into an array of objects. You can then mix strings and pauses.

```yml
scenes:
  - image: london.jpg
    narration: 
      - This is the first sentence, and we'll pause for a bit after it.
      - pause: 3
      - This is the second sentence
```

