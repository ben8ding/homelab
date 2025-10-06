Hello all! I've just got Proxmox loaded up on my first server build so I thought I would post my build experience in case other people had any interest in the parts and wanted to know of any silly quirks they might encounter.

Parts list:

* CPU: Intel I5-12400 

* Mobo: Asrock Rack Z690D4U-2L2T/G5 

* CPU Cooler: Heatsink Silverstone XE01-LGA1700 

* Ram: 1x Samsung 8GB DDR5 4800 MHZ (M323R1GB4BB0-CQK)

* Boot Drive: Micron 7450 Pro 480GB M.2 NVME 

* Storage Drive: 2x Dell EMC 960GB Sata (Micron 7300 Max) 

* Chassis: Inwin RA102 

* PSU: Powerman(?) 215W 80+ Bronze Flex ATX - Included With Chassis



![Semi Assembled](https://github.com/ben8ding/homelab/blob/main/images/MistyIsle/IMG_2170.jpeg?raw=true)


Most of the parts were bought used save for the chassis, PSU, and heatsink. Not sure I'd do it again as my first stick of ram ended up cooking mid OS installation, which has now been replaced by the aforementioned Samsung stick I nabbed from work.

The build itself was a learning process for a lot of things as it's the first time I've worked with a 1U chassis. Now I know why everyone says to just build a 2U chassis. For one, the backplate of the motherboard was taller than the standoffs, and there's currently a slight bend in the motherboard to get it screwed in. Finding an IO shield was also half an adventure, as my vendor for the Inwin chassis had exactly one left in the warehouse, and it ended up shipping to the wrong customer. Fortunately, both of us were in the same region and I was able to meet up to swap the wrong part I had been sent rather than toss it back over mail.

The motherboard itself came with absolutely nothing, not even a screw for the M.2 drive. The standoff itself also used an M3 screw instead of the usual M2. No IO shield either if I decide to transplant it into a 2U chassis either.

And as with all servers, the the little 40x40x38mm fans are screamers. The board wanted them to idle at 10k RPM, and after I snuck into the IPMI they still run at 6K RPM at 20% duty cycle. At 10K RPM I could hear them upstairs from where they live in my Harry Potter closet, but now they're mostly background noise.

Overall, I had a lot of fun hunting parts and learning as I assembled. The hardware is always more fun than software for me, so I've been dragging my feet on setting up Proxmox. The plan is to just use it as a small media server, but the CPU should have enough grunt to do other virtualization tasks and with a bit of extra ram I can probably fit a minecraft server on it too.

Thanks for reading, and I'll do my best to answer any questions!
