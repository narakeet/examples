# Video Puppet voice control example

This example shows how to set voices for different scenes in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works

To set the voice for the whole document, use a `voice` property on the top level, such as this:

```yml
size: 720p
voice: William
scenes:
# your scenes
```

To set the voice for an individual scene, make the scene `narration` element a key-value map, then use the `voice` property of that object. Move the contents of the narration into the `text` sub-element:

```yml
scenes:
  - image: london.jpg
    narration:
      text: Passengers will instead be boarding a plane belonging to a Belgian budget airline.
      voice: Elisabeth
```


## Available voices

The following voices are currently available:

* British English
  * William
  * Charles
  * Carol
  * Elisabeth
* American English
  * Mike
  * Bill
  * Sarah
  * Jeff
  * Lisa
* Australian English
  * Kylie
  * Bruce
  * Kate
  * Liam
* German
  * Monika
  * Florian
  * Marlene
  * Helmut
* French 
  * Alain
  * Margot
  * Sophie
  * Jean
* Dutch
  * Maartje
* Swedish
  * Ingrid
* Italian
  * Mario
  * Laura
* Japanese
  * Akira
  * Yuriko
* Korean
  * Chae-Won
  * Min-Ho

