# Adobe Fonts Liberator

> Copy Adobe Fonts (OTF) to a folder on your Desktop

[https://github.com/pawalan/adobe-fonts-liberator](https://github.com/pawalan/adobe-fonts-liberator)

### Problem  
Your licensed and activated Adobe Fonts are not accessible for general use in Windows:
1. they are stored (hidden) under `%APPDATA%\Adobe\CoreSync\plugins\livetype\r`
2. the file names are some sort of ID, which is good for Adobe managing the files, yet not human-readable

### Solution  
This script **copies all activated font files to a new directory `Adobe Fonts`** on your Desktop
and renames all of them to their PostScript name. For example, the file `17969` becomes `MinionPro-BoldCnItCapt.otf` (which includes all cues for font variation, weight, etc.).

After that, you can install the fonts to the Windows font store like all other fonts by right-clicking on the file(s)
and selecting `Install` or `Install for all users`. The fonts are then available to all your Windows applications.

### Configuration
The source and destination directory can be configured at the top of the script,
even though this shouldn't really be needed as the path to the Desktop folder is auto-determined from the 
user's environment and the Adobe CC fonts directory is located under a standard path in the user's %APPDATA%.

### Kudos
This script is essentially a PowerShell port of [kalaschik/adobe-fonts-revealer][1] - Grüße und Danke nach Leipzig!


[1]: https://github.com/kalaschnik/adobe-fonts-revealer
