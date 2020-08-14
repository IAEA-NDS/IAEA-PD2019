# IAEA Updated Evaluated Photonuclear Data Library (IAEA/PD-2019)
This repository contains the IAEA Photonuclear Data Library (IAEA/PD-2019). 

**Note that the processing of the IAEA/PD-2019 for application library was processed by a "patched version of NJOY2016", which is available under Github branch (feature/pn-iaea) of NJOY2016. The ACE library defaults to isotropic any energy-angle distribution coded in LAW=1, LANG=1 with NA=1, of which a sequence not yet handled in Acer (NJOY2016) for photon-induced file. This occurs for a few exit channels of 153 evaluations in the 219 presents in IAEA-PD2019. As soon as complete patch of NJOY2016 is released, the ACE library will be updated accordingly and this warning removed. However, this impediment bears no impact on the cross-section, residual or emitted particle spectra, or application library derived using other processing systems.**

``iaea-pd2019`` directory contains the original ENDF-6 format data files of 219 isotopes.  

``application-lib`` directory contains;  
- /ace            : Type-1 (ASCII) cross-section file  
- iaeapd19.xs     : xsdir for IAEA/PD-2019  
- /graphs         : Acer check/plot  

``activation-lib`` directory contains;  
- /hendf         : Linearised ENDF  
- /gxs-162       : Groupwise FISPACT-II files with MF1,2,3,8,10,33,40  
- /graphs        : Evalplot check/plot  

The information on the Research Coordination Meeting of CRP can be found at:

https://nds.iaea.org/CRP-photonuclear/index_1RCM.html

https://nds.iaea.org/CRP-photonuclear/index_2RCM.html

https://nds.iaea.org/CRP-photonuclear/index_3RCM.html

## Report
The report on "Processing of the Evaluated Photonuclear Data Library (IAEA/PD-2019)" is available at:

https://nds.iaea.org/publications/nds/iaea-nds-0232/

## Download
You can download the repository from a terminal using:

```
git clone https://github.com/IAEA-NDS/IAEA-PD2019.git
```

The ENDF-6 format data library and application libraries can be retrieved as compressed files (tar.gz) from the IAEA-NDS web site:

https://nds.iaea.org/photonuclear/


## Notifications
Please note that the master file will be managed by IAEA-NDS. Please
let us (NDS.Contact-Point@iaea.org) know if you find any problems.

