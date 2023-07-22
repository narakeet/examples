# Tiktok-style Subtitled Videos

This example shows how to produce TikTok-style videos with subtitles included over the video, in the middle of the video frame.


Check out the outcome in [`result.mp4`](result.mp4).

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`video.txt`](script/video.txt).

## How it works

To burn subtitles onto a video, add a `subtitle` header, and set the `mode` property to `overlay`. 

You can set the font to any TTF file, using the `font` property of the `subtitle` header.

TikTok videos usually have large subtitles in the middle of the screen. To achieve that, use the `position` property of the `subtitle` header and set it to `middle`.

Finally, to quickly show jut a few words at a time in large letters, set the font size using the `size` property. Sizes of 30-40 usually work well with standard TikTok video frame sizes. Then use the `break` property to control roughly how many characters to include in each subtitle (controlling the word break). 


Here is the full header example, setting the size to standard TikTok video frame, and setting the font position, size and choosing a custom font file.

```yml
size: 1080x1920
subtitles:
  mode: overlay
  break: 25
  size: 40
  font: CarterOne-Regular.ttf
  position: middle
```


