# Controling narration voices

This example shows how to set voices for different scenes in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

VideoPuppet script files can include an optional header, setting global properties. The header starts with the scene separator (`---`) in the first line,
and includes a key-value map separated by colons (technically, it's a YAML block). For example, the following header sets the size and the voice for the whole document:

```yml
---
size: 720p
voice: William
---
```

You can modify individual scenes by including a stage direction. Stage directions are paragraphs enclosed in brackets. For example, the following stage direction sets `Elisabeth` as the voice for the scene:


```md
(voice: Elisabeth)

Passengers booked to fly British Airways to Cairo this week, will 
instead be boarding a plane belonging to a Belgian budget airline.
```

## Available voices

Check out the Video Puppet [Available Voices](https://www.videopuppet.com/docs/voices/) page for an up-to-date list of voices and to try them out.

## Next steps

Check out the [pronunciation](../pronunciation/README.md) example for information on how to add pauses and control pronunciation.
