# OpenJPEG PPM/XPM/PCX load

Usually, it is only possible to load tga, png and jpg files into GMod. However, it appears that either FreeImage or OpenJPEG allows you to load different file formats by renaming it to a .jpg (or .png) file and loading it anywhere.

-   PPM
    -   Functions normally, but if you enter an extremely high (something like 8000x8000 wont work) number into the resolution tuple, it will crash quickly.
-   XPM
    -   Functions normally.
-   PCX
    -   Causes an infinite hang on load

See the attached files in this folder.

## Plugins

FreeImage have user installed plugins that are searched for in the root folder of the executable.
They are compiled DLLs.. but they are renamed to have the extension: ".fip" (probably stands for FreeImage Plugin)

I did not get any to load without crashing, but creating an empty file with the ".fip" extension in gmod's root will cause a hard Win32 library loading error on every boot.

The only known FreeImage plugins do not load, and the recent binaries are years old.