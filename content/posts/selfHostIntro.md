---
title: "Self-hosting applications using k3s over an Orange Pi cluster"
date: "2023-11-18"
tags: ["emoji"]
ShowToc: false
ShowBreadCrumbs: false
---

# 

This hobby project aims to build a small-scale, highly available, scalable server to host our applications and store our data durably using replication. To achieve the same, we would develop our server using 3 [Orange Pi 5](http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/details/Orange-Pi-5.html) boards and have [k3s](https://k3s.io/) (a lighter version of Kubernetes) run over it. We would be using [Longhorn](https://longhorn.io/) to have data replication. The sample application we would be hosting is [Seafile](https://www.seafile.com/), an open-source file sync and share software.

The hardware we will be needing for this will be as follows:

1. Three or more Orange Pi 5 boards. You can use any other computer that can host a Linux server, but setup may vary based on CPU type (ARM vs x86) and hardware capabilities.
2. An M2 SSD for each board. It’s known that micro-SSDs have high wear and tear; hence, M2 SSDs are preferable. Orange Pi boards need an M2 2242 NVMe SSD, but with an extra stand, we can use full-size SSDs too, as I have done. 
3. Switch
4. A router with internet access to which the switch will connect to.
5. Ethernet cables
6. (optional) M2 screws and bolts for attaching SSDs to a case or stand
7. (Optional) Thermal pads for the processors
8. (Optional) A stand to hold everything in place. You can get this 3D-printed from the STL files shared over my drive folder.
9. (Optional) A fan to cool everything. [Amazon link](https://a.co/d/goxG4lU)
10. (Optional) If you intend to 3D print the shared stand, you would need three 100 mm rods to hold the boards on the stand. [Amazon link](https://a.co/d/0HeK35E)

Once we have everything needed, let’s start setting up a server with the help of the next blogs in this series.