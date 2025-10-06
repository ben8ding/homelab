Man these hot swap rack mount chassis are expensive.

Components: 

* CPU: AMD 7600

* Mobo: Gigabyte MC13-LE1

* CPU Cooler: Dynatron A47 2U Cooler

* Ram: Kingston KSM48E40BS8KI-16HA 16GB DDR5 ECC UDIMM

* Boot Drive: Micron 7450 Pro 480GB M.2 NVME 

* Storage Drives: 2x Western Digital Red Plus 4tb WD40EFPX 

* HBA: Inspur 9300-8i LSI SAS3008

* Chassis: Silverstone RM21-304

* PSU: FSP400-70AGGBM(M)

![Figure 1](https://github.com/ben8ding/homelab/blob/main/images/CinderCove/IMG_3532.jpeg?raw=true)

I actually originally intended to use a Kingston DC2000B 240GB drive as my boot drive, but unlike the Asrock motherboard, I bought this MC13-LE1 new which came with a heatsink. The DC2000B I ordered, however, came with an integrated heatsink already and I didn't feel like tearing it off so I just swapped the drives. The 7450 Pro was also overheating in the 1U chassis without a heatsink so I'd say this smacks two birds with one stone.

![Figure 2](https://github.com/ben8ding/homelab/blob/main/images/CinderCove/IMG_3533.jpeg?raw=true)

The chassis has a neat feature where the fan bracket can be removed to mount the fans. You can technically fit 25mm thick fans, but they press right against the PWM pins on the backplane.

The other change I made mid build was the PSU. Pictured in the image above is a Seasonic SSP-650RS, which while has plenty of power for a front to back ATX PSU, has way too many cables I don't need and is 20mm longer. This combined with the extra cables made management a huge pain, and I decided to grab a shorter FSP unit from Digikey that matched my use case better. 

![Figure 3](https://github.com/ben8ding/homelab/blob/main/images/CinderCove/IMG_3561.jpeg?raw=true)

The FSP unit is actually quite nice, it's actually fully modular, I just ended up using all the cables anyways. Some of the higher wattage models will even have 8 Pin PCIE cables.
I'm not actually sure the HBA fan is necessary here, as it is a 2U chassis. But since I'm using slim fans instead I decided to play it safe.

My experience with the motherboard itself has been positive, save for a small hiccup with the ram stick in the wrong slot. The BMC also has a couple extra features such as bios post code logging. (Asrock BMC has the post code on the board itself). I didn't have any issues with the board not having an onboard video output.

OS setup: Proxmox with virtualized Truenas and the HBA passed through.
