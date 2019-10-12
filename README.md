# Archive of the "J operating system" by Terry

* ```jos.iso``` was downloaded from http://web.archive.org/.
' ```JOS.ISO/``` contains the contents of ```jos.iso``` (– an Android RAR app was able to extract the files of the ISO image).

## Run JOS in qemu

To run ```jos.iso``` in qemu, install: ```qemu-system-i386```.

Start qemu with ```qemu-system-i386 -cdrom jcd.iso -m 100```.

* In the JOS boot loader screen, press ```s``` for seconday IDE controller, followed by ```0``` for IDE master.

## TODO

* I don't know howto decode the files in ```JOS.ISO/```. I have tried the ```TOSZ.CPP``` unzip utility that comes with TempleOS without much success. - If you have an idea howto uncompress these files, please let me know.

## Contact

* https://github.com/koppi

