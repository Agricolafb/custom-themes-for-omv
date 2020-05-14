Change the look of your OpenMediaVault web gui by inserting a custom css theme into your OMV install via command line. By creating a theme-custom.css file you will override certain values in the default css files in OpenMediaVault. Here are the steps.

1. Open your command line tool of choice and login to your OMV server and enter the following commands.
2. $ cd /var/www/openmediavault/css
3. $ sudo nano theme-custom.css
4. Copy the contents of the desired theme and paste them into the theme-custom.css file.
5. Press "Control-x", then "y", then the "return" key.
6. Refresh your OMV web page.
Enjoy.

Notes on a Custom Logo: To place an identifying name or logo in the top bar of the left menu requires a 160x35px file appropriately named (see line 79-80 for my file name. You can use whatever filename you like, it just needs to match the name in the theme-custom.css file.) and needs to reside in /var/www/openmediavault/images. Using Inkscape create an appropriately named .svg and .png image:
1. Open Inkscape and create a blank palatte 160x35px.
2. Choose Font name and font size=32. You may need to adjust the font size to fit your palatte.
3. Once you have typed the text you want, in order to have the font appear correctly across multiple browsers and devices, you have to select the whole text and...
4. In the Path menu select "Object to Path".
5. In the Object menu select "Group".
6. In the Path menu select "Union".
7. Press save and give the file an appropriate name.
8. Save as PNG and give the file an appropriate name. I am guessing the .png version is used as a backup for non-.svg supported situations. 
9. Place the two images in /var/www/openmediavault/images.
Enjoy.
