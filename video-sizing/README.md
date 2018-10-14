# Video Puppet video sizing example 

This example shows how to automatically resize video clips to fit the output format in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.yml`](script/source.yml).

## How it works

Add a `size` to the `video` property of your scene, and set it to one of the following three values:

* `fit`: video will be rescaled without keeping the proportions
* `contain`: video will be completely visible, and padded if necessary with black bars to fit the output frame
* `cover`: (default) video will be scaled so it completely covers the output frame, and cropped if necessary to keep the proportions

```yaml
scenes:
  - video: 
      file: birds.mp4
      size: contain

```
