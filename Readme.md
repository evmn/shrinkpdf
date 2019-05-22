# Reduce PDF Size

Download the script by clicking the filename at the top of the box. Make it executable. If you run it with no arguments, it prints a usage summary. If you run it with a single argument – the name of the pdf to shrink – it writes the result to stdout:

```sh
./shrinkpdf.sh in.pdf > out.pdf
```

You can also provide a second filename for the output:

```sh
./shrinkpdf.sh in.pdf out.pdf
```

And an output resolution in DPI (default is 72 DPI):

```sh
./shrinkpdf.sh in.pdf out.pdf 90
```

If both the input and the output are regular files, the script checks if the output is actually smaller. If not, it writes a message to stderr and copies the input over the output.

Sorry, Windows users; this one is Linux only. A Windows adaptation of this script can be found on [this blog](http://dcm684.us/wp/2013/10/pdf-shrink/). It's a bit more user-friendly than my barebones version and also supports drag-and-drop.

# Reference

 [Shrinkpdf: shrink PDF files with Ghostscript](http://www.alfredklomp.com/programming/shrinkpdf/)
