SpelunkyWadUtility v1.2
=======================

Unpacks and repacks the .wad&amp;.wix file pairs from the game [Spelunky by Mossmouth](http://spelunkyworld.com/)

Tested on Python 2.7 and Python 3.3. Older versions **might** work but YMMV.
Update your Python if you're having problems.

Usage
=====

* Copy the **.py** files to the directory with the **.wad** file you want to mess with.
  * This could be "..\Spelunky\Data\Textures" for an example for textures.
* To unpack, run **unpack.py**.
* To repack modified files, dump them in the **repack** subdirectory as is. **Don't** make any extra directories there.
* Run **repack.py**, which will rebuild the **.wad** file.

Notes
=====

* If you made a booboo, there are backups made on the first unpack named something like **.wad.orig**.
* You can run the included convenience script **restore_original.py** to move them over the current **.wad**.
* In case of game updates that change the **.wad** file you've modified, I'd suggest doing this:
  * Make sure you got at least version 1.1 of my scripts
  * Run **restore_original.py** script to get rid of the old .origs.
  * Go on Steam and "Verify integrity of game cache" or get the new files some other way, if you downloaded from GOG for an example.
  * Run **repack.py** to repack your modifications over the now updated **.wad**