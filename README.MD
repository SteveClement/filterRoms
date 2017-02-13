## FilterRoms ##

Introduction
-------
These tool is design to help people to filter roms using some official pre-defined patterns. This product has been written for Mac OS and should work on all Unix system. As command line arguments/results may differ between these OS, there is no garantee  to work on Unix system. Please give me your feedback! May also work on Windows using a unix simulator (Cygwin, Git Bash...).

Pre-requisite
-------

- Mac OS / Unix system
- 7z in command line (p7zip on Mac OS)

Usage
-----
Configure the pattern.txt file. You can use the RomSuffixCode.txt to dertermine the patterns you want.

**Warning**: consider all patterns will be treated together (logical AND)

Put your compressed rom files in input directory.

If there is an output directory, please ensure it is empty.

You can now run the following command:

./filterRoms.sh

Output
------
Because of the f*** exclamation mark character, I was not able to uncompressed the desired files. If you have a solution, I would appreciate.

So, the script creates output/7zCommands.txt file. You can open the file, select and copy all and then paste it in the terminal and press Enter. The files should be uncompressed inside output folder.

Limitations
-----------

- Only works with 7z archive for now
- Only uncompress 1st level of hierarchy (does not uncompress archive of archive of archive...)