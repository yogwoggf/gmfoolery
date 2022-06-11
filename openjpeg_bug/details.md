# OpenJPEG PPM/XPM/PCX load

Usually, it is only possible to load tga, png and jpg files into GMod. However, it appears that either FreeImage or OpenJPEG allows you to load different file formats by renaming it to a .jpg (or .png) file and loading it anywhere.

-   PPM
    -   Functions normally, but if you enter an extremely high (something like 8000x8000 wont work) number into the resolution tuple, it will crash quickly.
-   XPM
    -   Functions normally.
-   PCX
    -   Causes an infinite hang on load

See the attached files in this folder.
