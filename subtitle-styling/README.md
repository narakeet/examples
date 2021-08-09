# Styling subtitles

This example shows how to control overlay subtitle styling, to set a different font size or color.

## Try it out

Upload the [`script`](script) directory to a Narakeet project. The main script file is [`source.md`](script/source.md).

## How it works

You can control overlay property styling by providing a set of properties in the `subtitle` header value, setting the mode to `overlay`, then using the `color`, `background` or `outline` properties to set the styling, and `scale` or `size` properties to control the font size. See the [subtitles header](https://www.narakeet.com/docs/format/#subtitles) format documentation for more information.

**Important note**: the header section is specified as YAML, which uses `#` for a comment. If you want to specify a hex value with any of the color properties, make sure you enclose it into quotes, to prevent YAML ignoring it as a comment. 


