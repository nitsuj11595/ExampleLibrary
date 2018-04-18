# ExampleLibrary for Processing

Sample library for Processing with *Makefile* for easier development.

Library may be cloned into your **sketchbook/libraries/** directory, or downloaded from the **.zip** file



Building from source requires Processing's **core.jar** file in the **sketchbook/libraries/** directory.

Use `make` to compile and create a **.jar** file.



## Using Makefile for you own libraries

Edit *Makefile* before running `make`.  Set NAME to the name of you library name on line 24.  Then specify each of you source files after line 27.  Every line (except the last) should have backslash at end:

```
# List all source files here (example)
CLASSES = \
	src/File1.java \
	src/File2.java \
	src/File3.java
```



## Recipes

`make`

Compile all files and create java archive.

`make clean`

Remove binaries

`make docs`

Update javadoc reference.

`make zip`

Prepare a zip file for publishing.



A completed library may be turned into a zip file for publishing with `make zip`

