# ExampleLibrary for Processing

Sample library for Processing with **Makefile** for easier development.

Completed libraries may be cloned into your **sketchbook/libraries/** directory, or downloaded from the **.zip** file



Building from source requires Processing's **core.jar** file in the **sketchbook/libraries/** directory.

Use `make` to compile and create a **.jar** file.



## Using Makefile for you own libraries

Edit **Makefile** before running `make`.  Set NAME to the name of your library name on line 25.  Then specify each of your source files after line 27.  Every line (except the last) should have backslash at end:

```
# List all source files here (example)
CLASSES = \
	src/File1.java \
	src/File2.java \
	src/File3.java
```



## Recipes

`make`

Compile all source files and create java archive.

`make clean`

Remove binaries.  Effectively uninstalls library, but keeps source code.

`make docs`

Updates javadoc reference.

`make zip`

Prepare a zip file for publishing.  All of the necessary files as well as source code, examples and reference, are included in the zip.  However **bin** directory and **Makefile** are omitted.

