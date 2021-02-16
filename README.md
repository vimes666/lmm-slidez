# lmm-slidez

## Slideshow generator for linux mint mate desktop background.

This bash script generates an XML file that can be used as a background slideshow in the linux mint mate desktop. It __recursively__ collects the names of all image files that are present in the input folder. 
The script is able to randomize the order of the images. 

### Installation:
- Place the script in the folder .bin (if you dont have the folder, create it with `mkdir .bin`).
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

### Notes:
- If you add, remove or change images in the image folder, you will have to run lmm-slidez again to see the result in the slideshow.
- The random image order is estabished at the moment lmm-slidez runs. To get a new random order, you will have to run lmm-slidez again.
- Comments and suggestions are always appreciated :)

