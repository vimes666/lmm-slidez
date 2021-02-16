# lmm-slidez

## Slideshow generator for linux mint mate desktop background.

This bash script generates an XML file that can be used as a background slideshow in the linux mint mate desktop. It __recursively__ collects the names of all image files that are present in the input folder. 
The script is able to randomize the order of the images. Also the duration per image, input folder and output file can be set.

### Syntax
    lmm-slidez [-h] [-r] [-v] [-d duration] [-i input-folder] [-o output-file]

        -d seconds          How long each image will be displayed.
        -h                  Show syntax.
        -i input-folder     Specifies the location name where the images are located. Default is /usr/share/backgrounds.
        -o output-file      Specifies the location of the output XML file. Default is /home/username/.backgrounds/slideshow.xml
        -r                  Randomize the sequence of the images. This happens only during the generation of the XML file. 
                            If you want to reorder it again you will have to regenerate the XML file.
        -v                  Print version.

### Installation:
- Place the script in the folder .bin and if you dont have the folder, create it with `mkdir .bin`.
  The dot designates a hidden file so it will only show up in the file manager after typing ctrl-h.
- Make the file executable if necessary `chmod +x .bin/lmm-slidez`.
- Create the folder .backgrounds with `mkdir .backgrounds` if it is not already there.

### Usage:
- In a terminal type `lmm-slidez -r`
  This will generate the slideshow file /home/username/.backgrounds/slideshow.xml from all the images in the linux mint backgrounds folder /usr/share/backgrounds.
  The -r option tells the script to randomize the picture order.
- Right-click the desktop background and click 'change desktop background'.
- Click 'Add...'.
- Select 'All files' on the pulldown button that says 'Images' (above the open button).
- Navigate to /home/username/.backgrounds or enter that name in the location field.
- Select the file slideshow.xml and click open.
- Done.
- If you generate a new slideshow and replace the existing active slideshow, the switch will be instantaneous. If you make one with another name you will have to add it manually as described before.

### Notes:
- Comments, suggestions and bug reports are always appreciated :)
