---
size: 720p
voice: William
---

<!--
You can set the global document properties in the preamble. 
If the first line is starting with three dashes, the whole first
block includes global document properties, and is not 
parsed as a scene
-->

![](london.jpg)

Before we fix any rules let us think of some familiar cases. There are
60 minutes in the hour, 24 hours in the day, 7 days in the week. 

<!-- 

Video Puppet will automatically turn fenced code blocks into 
slides on top of the image or video included in the scene. 

You can specify a language for syntax highlighting  
-->

```yml
---
size: 720p
voice: William
---
```

---

![](london.jpg)

<!-- 
to set a voice on an individual narration, 
use the stage narration in a separate paragraph.
-->

(voice: Elisabeth)

Passengers booked to fly British Airways to Cairo this week, will 
instead be boarding a plane belonging to a Belgian budget airline.

```
(voice: Elisabeth)
```

---

![](berlin.jpg)
    
(voice: Monika)

Heute Nacht sollen wir in Bombay einlaufen, es ist schon höchste
Zeit, da meine gesammte Wäsche erschöpft ist und ich nothwendig
einer Neuausrüstung bedarf.

```
(voice: Monika)
```

---

![](berlin.jpg)

(voice: Helmut)

Abends spät sollen wir in Port Saïd eintreffen. Hoffentlich erst
morgen, denn bei dem Lärm des Kohlens könnten wir ja doch nicht
schlafen.

```
(voice: Helmut)
```

---

![top](ny.jpg)

(voice: Lisa)

Many districts and landmarks in New York City are well known, with the
city having three of the world's ten most visited tourist attractions in
2013.

```
(voice: Lisa)
```

---

![top](ny.jpg)

(voice: Mike)

Situated on one of the world's largest natural harbors, New York
City consists of five boroughs, each of which is a separate county of the
State of New York.

```
(voice: Mike)
```

---

![](paris.jpg)
      
(voice: Alain)

Plus tard, cette société toujours plus puissante prit une force que le
temps lui avait préparée et qui parfois se trouva être à l'unisson du
pouvoir royal.

```
(voice: Alain)
```

---

![](paris.jpg)

(voice: margot)

Le moment de la plus grande influence des lettres sur la nation fut
celui où la littérature déserta les écoles, pour faire ses cours dans
les salons.
    
```
(voice: Margot)
```

---

![](esp.jpg)

(voice: carmen)

La filosofía de la periferia es, necesariamente, una filosofía de la
liberación. La filosofía de los centros de poder no es otra cosa que una
ontología que enuncia una mismidad: "El ser es, el no-ser no es", lo cual
significa que todo lo que esté fuera de las fronteras del ser, carece de
ser. 

```
(voice: Carmen)
```

---

![top](ny.jpg)

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
