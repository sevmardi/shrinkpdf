# Shrinkpdf
A simple wrapper around Ghostscript to shrink PDFs (as in reduce filesize) under Linux. Inspired by some code I found in an OpenOffice Python script (I think). The script feeds a PDF through Ghostscript, which performs lossy recompression by such methods as downsampling the images to 72dpi. The result should be (but not always is) a much smaller file.


