# Video Puppet call-outs example 

This example shows how to add call-outs to highlight important parts of a slide in Video Puppet. 

Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Video Puppet project. The main script file is [`source.md`](script/source.md).

## How it works

Add a circle highlight to a picture by providing `callout` stage direction. property of a scene. Set the circle center using `cx` (horizontal position) and `cy` (vertical position) and the circle radius using `size`. The coordinates are relative to the top-left corner of the original image.


When using complex stage directions, such as `callout`, indent the subproperties by two spaces or a tab (technically, the stage direction block enclosed in brackets is YAML)

```
(callout:
  cx: 313
  cy: 250
  size: 100)

![](image.png)
```

You can also set a rectangular highlight, by specifying `type` to be `rectangle`, then providing the `top`, `left`, `bottom` and `right` coordinates of the rectangle, relative to the top-left corner of the original image.

```yaml
![](image.png)

(callout:
  type: rectangle
  left: 450
  top: 0
  right: 770
  bottom: 130)
```

