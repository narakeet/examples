![cover](london.jpg)

This is the first sentence, and we'll pause for a bit after it.

<!-- to add a pause between sentences, just use the pause stage direction, and set the number of seconds -->

(pause: 3)

This is the second sentence.

---

```txt
_Important_
**Really important**
~~Not important~~
```

![cover](london.jpg)

<!-- Use markdown emphasis, strong and strikeout to control emphasis -->

This is my usual voice. *This is more important.* **This is really important.** ~~This is not so much.~~ This is my normal voice again.

---

![cover](london.jpg)

(font-size: 30)

```
(voice-emphasis: moderate)
```

(voice-emphasis: moderate)

This is more important.

---

![cover](london.jpg)

I'm speaking normally.

(voice-volume: soft)

I'm speaking softly.

(voice-volume: loud)

Now I'm loud.

---

![cover](london.jpg)

I'm speaking normally.

(voice-speed: slow)

I'm speaking slowly.

(voice-speed: fast)

Now I'm fast.

---

<!-- for advanced control with generated voice, wrap the narration into <speak></speak> and use SSML -->

<speak>
  <emphasis level="strong">This is an important announcement</emphasis>
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
