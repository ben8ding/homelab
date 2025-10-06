
Parts list:

* CPU: Intel I5-12400 

* Mobo: Asrock Rack Z690D4U-2L2T/G5 

* CPU Cooler: Heatsink Silverstone XE01-LGA1700 

* Ram: 1x Samsung 8GB DDR5 4800 MHZ (M323R1GB4BB0-CQK)

* Boot Drive: Kingston DC2000B 240gb M.2 NVME 

* Storage Drive: 2x Dell EMC 960GB Sata (Micron 7300 Max) 

* Chassis: Inwin RA102 

* PSU: Powerman(?) 215W 80+ Bronze Flex ATX - Included With Chassis



![Semi Assembled](https://github.com/ben8ding/homelab/blob/main/images/MistyIsle/IMG_2170.jpeg?raw=true)


Most of the parts were bought used save for the chassis, PSU, and heatsink. Not sure I'd do it again as my first stick of ram ended up cooking mid OS installation, which has now been replaced by the aforementioned Samsung stick I nabbed from work.

The build itself was a learning process for a lot of things as it's the first time I've worked with a 1U chassis. Now I know why everyone says to just build a 2U chassis. For one, the backplate of the motherboard was taller than the standoffs, and there's currently a slight bend in the motherboard to get it screwed in. Finding an IO shield was also half an adventure, as my vendor for the Inwin chassis had exactly one left in the warehouse, and it ended up shipping to the wrong customer. Fortunately, both of us were in the same region and I was able to meet up to swap the wrong part I had been sent rather than toss it back over mail.

The motherboard itself came with absolutely nothing, not even a screw for the M.2 drive. The standoff itself also used an M3 screw instead of the usual M2. No IO shield either if I decide to transplant it into a 2U chassis either.

And as with all servers, the the little 40x40x38mm fans are screamers. The board wanted them to idle at 10k RPM, and after I snuck into the IPMI they still run at 6K RPM at 20% duty cycle. At 10K RPM I could hear them upstairs from where they live in my Harry Potter closet. I've swapped them with Arctic's S4028-6K 6000 RPM 40mm fans instead, and while it is a reduction in noise, the CPU cooler itself is where most of the noise is coming from. Dynatron makes a similar looking model with a copper heatsink and a proper vapor chamber instead of a skived aluminum block that I suspect will perform better, but maybe not $60 better. For now, the noise is tolerable when the door is closed.

