My archive of the "J operating system" by Terry Davis

* ```jcd.iso``` was downloaded from https://web.archive.org .
* ```JCD.ISO/``` contains uncompressed the contents of ```jcd.iso```.

## Run JOS in qemu

To run ```jcd.iso``` in qemu, install ```qemu-system-i386```. Start qemu with ```qemu-system-i386 -cdrom jcd.iso -m 100```. In the JOS boot loader screen, press ```s``` for seconday IDE controller, followed by ```0``` for IDE master.

To boot qemu with a hard drive, run it with the following options

```
-drive file=JHD.raw,index=0,format=raw,media=disk -boot d
```

after creating a ```JHD.raw``` HDD image with

```
qemu-img create JHD.raw 500M
```
