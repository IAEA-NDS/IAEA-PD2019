# IAEA Updated Evaluated Photonuclear Data Library (IAEA/PD-2019.2)
This repository contains the IAEA Photonuclear Data Library (IAEA/PD-2019).
Please note that in order to retrieve ENDF and ACE files from this repository,
you need [git-annex][git-annex]. Alternatively, you can download the files
from the IAEA website, see the [Download section](#download) of this page.

[git-annex]: https://git-annex.branchable.com/

The `iaea-pd2019` directory contains the original ENDF-6 format data files of 219 isotopes.
The `application-lib` directory contains `ace` files and plots.
For details on the processed files, see [application-lib/README.md][app-lib-readme].

There is also an activation library part in `activation-lib` which contains
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

[iaeapd19ace]: https://github.com/IAEA-NDS/IAEA-PD2019/blob/dev/application-lib/indc-nds-858-draft.pdf

The details on how files were processed previously can be found in
the report on "Processing of the Evaluated Photonuclear Data Library (IAEA/PD-2019)" at:

<https://nds.iaea.org/publications/nds/iaea-nds-0232/>

## Download
You can download the repository from a terminal using:

```
git clone https://github.com/IAEA-NDS/IAEA-PD2019.git
```
In order to retrieve afterwards all large files (ENDF, ACE, etc.),
run from the root directory of this repository
```
git annex get .
```

The ENDF-6 format data library and application libraries can also be retrieved as compressed files (tar.gz) from the IAEA-NDS web site:

<https://nds.iaea.org/photonuclear/>


## Notifications
Please note that the master file will be managed by IAEA-NDS. Please
let us (NDS.Contact-Point@iaea.org) know if you find any problems.

[app-lib-readme]: https://github.com/IAEA-NDS/IAEA-PD2019/tree/dev/application-lib/README.md
