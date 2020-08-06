# IAEA Updated Evaluated Photonuclear Data Library (IAEA/PD-2019)
This repository contains the IAEA Updated Evaluated Photonuclear Data Library (IAEA/PD-2019). 

```diff
- Note that for the time being the ACE library defaults to isotropic any energy-angle distribution coded in law=1, lang=1 with na=1, a sequence not yet handled in Acer for photon induced file. This occurs for a few exit channels of 153 evaluations in the 219 presents in IAEA-PD2019. As soon as a patch for NJOY-2016 is released the ACE library will be updated and this warning removed. However, this impediment bears no impact on the cross-section, residual or emitted particle spectra, or application library derived using other processing systems.@@
```

``iaea-pd2019.0`` directory contains the original ENDF-6 format data files fro 219 isotopes.  

``application-lib`` directory contains  
- /ace            type-1 (ASCII) cross-section file  
- iaeapd19.xs     xsdir for iaeapd19  
- /graphs         Acer check/plot  

``activation-lib`` directory contains  
- /hendf       linearised endf  
- /gxs-162      Groupie 162 gprs files with MF1,2,3,8,10,33,40  
- /graphs       Evalplot check/plot  

The information on the Research Coordination Meeting of CRP can be
found:

https://nds.iaea.org/CRP-photonuclear/index_1RCM.html

https://nds.iaea.org/CRP-photonuclear/index_2RCM.html

https://nds.iaea.org/CRP-photonuclear/index_3RCM.html

## Report
The report on "Processing of the Updated Evaluated
Photonuclear Data Library (IAEA-PD2019)" is available here:

https://nds.iaea.org/publications/nds/iaea-nds-0232/

## Download
You can download the repository from a terminal using:

```
git clone https://github.com/IAEA-NDS/IAEA-PD2019.git
```

The compressed tar files are available on the IAEA-NDS web site:

https://nds.iaea.org/photonuclear/


## Notifications
Please note that the master file will be managed by IAEA-NDS. Please
let us (NDS.Contact-Point@iaea.org) know if you find any problems.



