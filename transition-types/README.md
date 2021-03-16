# Narakeet transition types

This example shows how to automatically various transition types.

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

To set a transition for an individual scene, add it using the `transition` stage direction. For example, the script below adds a 2-second long crossfade incoming transition to the current scene:


```
![](london.jpg)

(transition: crossfade 2)
```

Note that the transition property combines the previous scene with the current scene, so any transition on the first scene is ignored.

## Available transition options


See <https://www.narakeet.com/docs/format/#transition> for an up-to-date list of supported transition types
