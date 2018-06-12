# Shrinkpdf
A simple wrapper around Ghostscript to shrink PDFs (as in reduce filesize) under Linux. Inspired by some code I found in an OpenOffice Python script (I think). The script feeds a PDF through Ghostscript, which performs lossy recompression by such methods as downsampling the images to 72dpi. The result should be (but not always is) a much smaller file.


## Usage
Download the script by clicking the filename at the top of the box. Make it executable. If you run it with no arguments, it prints a usage summary. If you run it with a single argument – the name of the pdf to shrink – it writes the result to stdout:

``` ./shrinkpdf.sh in.pdf > out.pdf ```

You can also provide a second filename for the output:

```./shrinkpdf.sh in.pdf out.pdf```

And an output resolution in DPI (default is 72 DPI):
``` ./shrinkpdf.sh in.pdf out.pdf 90 ```
