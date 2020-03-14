# Controlling pronunciation 

This example shows how to control pronunciation and narration pauses in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.md).

## How it works


You can specify a pause in narration by using the `pause` stage direction, and setting the number of seconds. For example, the following scene has a two second pause between the sentences.

```
![cover](london.jpg)

This is the first sentence, and we'll pause for a bit after it.

(pause: 3)

This is the second sentence.
```

To control emphasis, speed up or slow down the speech, use [SSML](https://en.wikipedia.org/wiki/Speech_Synthesis_Markup_Language) markup, and wrap the narration into `<speak></speak>` tags. For example, the following scene sets a moderate emphasis using SSML.

```xml
<speak>
  <emphasis level="moderate">
    This is an important announcement
  </emphasis>
</speak>

![cover](london.jpg)
```
