# markpdf - Watermark PDF files using image or text

A tiny command line tool to watermark PDF files using image or text. 
With simple options to configure position, opacity, rotation, stretch etc.

Highlights -

- Very simple and easy to use 
- Extreamly fast!
- Stretching watermark image to height or weight proportionately 
- Options to adjust position, opacity, rotation of image
- Free and open source

## Install

It's just a single binary file, no external dependencies. 
Just download the appropriate version of [executable from latest release](https://github.com/ajaxray/markpdf/releases) for your OS. Then rename and give it execute permission.
```bash
mv markpdf_linux-amd64 markpdf  
sudo chmod +x markpdf
```

If you want to install it globally (run from any directory of your system), put it in your systems $PATH directory.
```bash
sudo mv markpdf /usr/local/bin/markpdf
```
Done! 

## How to use

### Image watermarking

Command options are shown in both, shorthand and full name.

```bash
# watermark with all default options (on top left corner with 50% opacity)
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf"

# watermark at center
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" --center
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" -c

# watermark at right top with 20px offset from edge and full opaque
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" --offset-x=-20 --offset-y=20 --opacity=1.0
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" -x -20 -y 20 -o 1.0

# watermark at left bottom with 100px offset and 45 degree rotation
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" --offset-x=100 --offset-y=-100 --angle=45
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" -x 100 -y -100 -a 45

# stretch full with of page at page middle
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" --scale-width-center
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" -W
# Note the capital "W" 

# stretch full with of page at page bottom
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" --scale-width --offset-y=-10
markpdf "path/to/source.pdf" "img/logo.png" "path/to/output.pdf" -wy -10
```

### Image watermarking

> Note : Text watermarking is not completed yet.

## Roadmap

✅ Draw image on every page of PDF
✅ Configure Opacity option
✅ Configure watermark position by X and Y offset
✅ Allow negative values to for offset to adjust from opposite direction
✅️ Easy option for positioning at center
✅ Configure rotation angle
✅ Options to Stretch watermark to width or height, proportionately
✅ Options to Stretch watermark to width or height at the middle of page
◻️ Render text on every page
◻️ Configure text color, style and font
◻️ Configure text opacity
◻️ Configure text rotation angle
◻️ Text placement by offset 
◻️ Put text at page center

### Contribute

If you fix a bug or want to add/improve a feature, 
and it's alligned with the focus (merging with ease) of this tool, 
I will be glad to accept your PR. :) 

### Thanks

This tool was made using the beautiful [Unidoc](https://unidoc.io/) library. Thanks and ❤️ to **Unidoc**.

---
> "This is the Book about which there is no doubt, a guidance for those conscious of Allah" - [Al-Quran](http://quran.com)


