![cover](london.jpg)

This is the first sentence, and we'll pause for a bit after it.

<!-- to add a pause between sentences, just use the pause stage direction, and set the number of seconds -->

(pause: 3)

This is the second sentence.

---

<!-- for advanced control with generated voice, wrap the narration into <speak></speak> and use SSML -->

<speak>
  <emphasis level="moderate">This is an important announcement</emphasis>
  <prosody rate="slow" pitch="-2st">Can you hear me now?</prosody>  
  <say-as interpret-as="verbatim">abcdefg</say-as>
</speak>

```xml
<speak>
  <emphasis level="moderate">
    This is an important announcement
  </emphasis>
  <prosody rate="slow" pitch="-2st">
    Can you hear me now?
  </prosody>  
  <say-as interpret-as="verbatim">
    abcdefg
  </say-as>
</speak>
```

![cover](london.jpg)
