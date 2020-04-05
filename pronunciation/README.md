# Controlling pronunciation 

This example shows how to control pronunciation and narration pauses in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works


You can use the standard markdown emphasis or strikethroughs to add emphasis or reduce importance for a specific sentence, and use stage directions such as `pause`, `voice-volume` or `voice-emphasis` to control the pronunciation. Check out the [Controlling pronunciation reference](https://videopuppet.com/docs/format/#controlling-pronunciation) for more information.

You can also use [SSML](https://en.wikipedia.org/wiki/Speech_Synthesis_Markup_Language) markup, and wrap the narration into `<speak></speak>` tags. For example, the following scene sets a moderate emphasis using SSML.

```xml
<speak>
  <emphasis level="moderate">
    This is an important announcement
  </emphasis>
</speak>

![cover](london.jpg)
```
