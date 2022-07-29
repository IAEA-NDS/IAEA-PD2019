# IAEA Updated Evaluated Photonuclear Data Library (IAEA/PD-2019)
This repository contains the IAEA Photonuclear Data Library (IAEA/PD-2019).

``iaea-pd2019`` directory contains the original ENDF-6 format data files of 219 isotopes.
``application-lib`` directory contains:

- /ace            : Type-1 (ASCII) cross-section files
- iaeapd19.xs     : xsdir for IAEA/PD-2019
- /extace         : ace files with additional data

Some directories with `ace` files contain a subdirectory `plots`
with plots in pdf format produced by NJOY2016.

``activation-lib`` directory contains;
- /hendf         : Linearised ENDF
- /gxs-162       : Groupwise FISPACT-II files with MF1,2,3,8,10,33,40
- /graphs        : Evalplot check/plot

The information on the Research Coordination Meeting of CRP can be found at:

<https://nds.iaea.org/CRP-photonuclear/index_1RCM.html>

<https://nds.iaea.org/CRP-photonuclear/index_2RCM.html>

<https://nds.iaea.org/CRP-photonuclear/index_3RCM.html>

## Report

To overcome some limitations of NJOY2016,
the processing has been performed with ACEMAKER, see
[this report][iaeapd19ace] for details.

[iaeapd19ace]: https://github.com/IAEA-NDS/IAEA-PD2019/blob/073a4d47a3d393c238f76fe6e8fdb9af7563358e/application-lib/iaea-nds-852-draft.pdf

The details on how files were processed previously can be found in
the report on "Processing of the Evaluated Photonuclear Data Library (IAEA/PD-2019)" at:

<https://nds.iaea.org/publications/nds/iaea-nds-0232/>

## Download
You can download the repository from a terminal using:

```
git clone https://github.com/IAEA-NDS/IAEA-PD2019.git
```

The ENDF-6 format data library and application libraries can be retrieved as compressed files (tar.gz) from the IAEA-NDS web site:

<https://nds.iaea.org/photonuclear/>


## Notifications
Please note that the master file will be managed by IAEA-NDS. Please
let us (NDS.Contact-Point@iaea.org) know if you find any problems.

