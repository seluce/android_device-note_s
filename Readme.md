Cubot Note S
===========
Device Tree for LineageOS 14.1
------------------

| Device | NOTE S |
| ------ | ------ |
| Chipset | MT6580 |
| Kernel |  Marshmallow 6.0 (3.18.19) |
| Display | 5,5" 1280x720 |
| Battery | 4150MAh |
| Storage |2GB RAM, 16GB storage |
| Camera | 8MP rear / 5MP front |

Bug	tracker
---------------
- [ ] Video recording interchanged color (workarround: any third party camera, like footej)
- [ ] Some app glitches are present (app crashes has been fixed, glitches are left)

Compiling on Ubuntu 20.10
---------------
First add device patches from device tree into Lineage
```
. build/envsetup.sh 

export JACK_SERVER_VM_ARGUMENTS="-Dfile.encoding=UTF-8 -XX:+TieredCompilation -Xmx4096m"

./prebuilts/sdk/tools/jack-admin kill-server

./prebuilts/sdk/tools/jack-admin start-server

export LC_ALL=C

brunch NOTE_S
```

Result
---------------
You can see the result on needrom: [LineageOS14.1 on needrom.com](https://www.needrom.com/download/n-lineageos-14-1)

Credits
---------------
* Rock12 ([Github](https://github.com/rock12))
* pedropereira22 ([Github](https://github.com/pedropereira22))
* ibrahim1973 ([Github](https://github.com/ibrahim1973))
* svoboda18 ([Github](https://github.com/svoboda18))
* Andrey Litvin (4PDA)
