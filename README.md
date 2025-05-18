Archive of the J Operating System by [Terry A. Davis](https://en.wikipedia.org/wiki/Terry_A._Davis):
* ```jcd.iso``` was downloaded from https://web.archive.org ,
* ```JCD.ISO/``` contains uncompressed the contents of ```jcd.iso```.

### Run JOS in qemu

To run ```jcd.iso``` in QEMU, install ```qemu-system-i386```.

Next, start QEMU with ```qemu-system-i386 -cdrom jcd.iso -m 100```. In the JOS boot loader screen, press ```s``` for seconday IDE controller, followed by ```0``` for IDE master:
![2025-05-18 08-35-09](https://github.com/user-attachments/assets/d82f6d29-160c-409e-ab17-58a159a7dd6e)

To boot qemu with a hard drive, run it with the following options:
```
-drive file=JHD.raw,index=0,format=raw,media=disk -boot d
```
after creating a ```JHD.raw``` HDD image with:
```
qemu-img create JHD.raw 500M
```

