dm.
==============================
A dark theme for [rEFInd](http://www.rodsbooks.com/refind/) based on [Dream Machine](https://github.com/Lindstream/dm-refind-theme).
----
**Screenshot**
![M](https://github.com/TheRealGramdalf/dm-remastered/blob/master/screenshot.png)

Recolored in purple - using gimp. If you want to make your own version, it is a bit tedious, but [this link](https://daviesmediadesign.com/quickly-change-colors-in-a-photo-with-this-gimp-tool-article-version/) should make it a breeze. Also open to requests, if I have time - just make an issue.

Installation
----
```
$root: cp -r ~/dm /boot/efi/EFI/refind/themes
$root: nvim + /boot/efi/EFI/refind/refind.conf # Opens nvim and puts the cursor on the last line
$root: # Append "include themes/dm/theme.conf" to `refind.conf`
```
__NOTES:__

Obviously [rEFInd](http://www.rodsbooks.com/refind/) is needed to use this. Install with your package manager `refind-efi`. You many need to run `refind-install` afterwards.

If the `refind` bootloader doesn't show up on boot even after running `refind-install`. Run `efibootmgr` (to see the current boot order), then set the order so it is loaded first, for example: `efibootmgr -o 0002,0003,0001`. You may first need to clear the boot order: `efibootmgr -O` OR delete a specific entry: `efibootmgr -A 0002`

----  
Attributions
----

**Font:** [Dento font](http://fontmeme.com/freefonts/34867/dento.font)

**Icons:** [Lightness for burg](http://sworiginal.deviantart.com/art/Lightness-for-burg-181461810) & [refind-ambience](https://github.com/lukechilds/refind-ambience).

**Reddit:** [rEFInd](http://www.rodsbooks.com/refind/)

----
