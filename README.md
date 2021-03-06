# lmm-slidez

## Slideshow generator for Linux mint mate desktop background.

This bash script generates an XML file that can be used as a background slideshow in the Linux mint mate desktop. It recursively collects the names of all image files that are present in the input folder. 
The script is able to randomize the order of the images. Also the duration per image, input folder and output file can be set.

### Syntax
    lmm-slidez [-f] [-h] [-r] [-v] [-d duration] [-i input-folder] [-m maxdepth] [-o output-file]

        -d duration         The duration that each image is displayed in seconds.
                            The default is 300.
        -f                  Force overwrite of the output file.
        -h                  Show syntax.
        -i input-folder     Specifies the location name where the images are located. 
                            Default is /usr/share/backgrounds.
        -m maxdepth         Level of recursiveness. 1 - 2147483647. The latter is default.
        -o output-file      Specifies the location of the output XML file. 
                            Default is /home/username/.backgrounds/slideshow.xml
        -r                  Randomize the sequence of the images. This happens only during the 
                            generation of the XML file. 
                            If you want to reorder it again you will have to regenerate the XML file.
        -v                  Print version.

### Installation:
- Place the script in the folder bin and if you don't have the folder, create it with `mkdir bin`.
- Make the file executable if necessary `chmod +x bin/lmm-slidez`.
- Create the folder .backgrounds with `mkdir .backgrounds` if it is not already there.
  The dot designates a hidden file so it will only show up in the file manager after typing ctrl-h.

### Usage:
- In a terminal type `lmm-slidez -r`
  This will generate the slideshow file /home/username/.backgrounds/slideshow.XML from all the images in the Linux mint backgrounds folder /use/share/backgrounds.
  The -r option tells the script to randomize the order of the images.
- Right-click the desktop background and click 'change desktop background'.
- Click 'Add...'.
- Select 'All files' on the pull down button that says 'Images' (above the open button).
- Navigate to /home/username/.backgrounds (press ctrl-h if you don't see .backgrounds).
- Select the file slideshow.xml and click open.
- Done.
- If you generate a new slideshow and replace the existing active slideshow, the switch will be instantaneous. If you make one with another name you will have to add it manually as described above.

### Notes:
- Comments, suggestions and bug reports are always appreciated :)
