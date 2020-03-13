---
size: 720p
---

> without a sync option, the last video frame is frozen to wait for audio

![](stopwatch.mp4)

This is going to be a slightly longer narration, so the video stopwatch will run out of time, but the last frame will wait for me to finish speaking. 

---

> ...but videos are not trimmed to match audio
  
![](stopwatch.mp4)

One, Two, Three.

---

>  ... set sync:match to speed up a longer video to match an audio track
    
![match](stopwatch.mp4)

One, Two, Three.

---

> ... sync:match also slows down a shorter video to match longer narration

![match](stopwatch.mp4)
  
One, Two, Three, Four, Five, Six, Seven, Eight, Nine, Ten, Eleven, Twelve

---

> ... set sync:trim to play a longer video at normal speed, but cut it off when the audio stops
  
![trim](stopwatch.mp4)

One, Two, Three

---

> ... sync:trim will also cut off an audio if it is longer than the video

(video:
  file: stopwatch.mp4
  sync: trim
  segment: 0 - 2)

I hate it when people just keep on talking and don't know when to stop.

---

> ... sync:loop will repeat a video when the audio is longer
  
(video:
  file: stopwatch.mp4
  sync: loop
  segment: 0 - 2)

This video will loop to match the duration of my sentence, so I can speak for as long as I want.


---

> ... sync:loop will repeat the audio when the video is longer

![loop](stopwatch.mp4)

One, Two, Three.

