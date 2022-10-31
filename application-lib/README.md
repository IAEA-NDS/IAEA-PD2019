# Application files (ACE)

The ace files in the subdirectories
have been produced by ACEMAKER.
For details regarding the processing, consult
[this report][iaeapd19ace].

For each material, several ace files are available
and differ in regard to the inclusion of delayed neutron
data for photo-fission and the inclusion of production
cross-sections. Files that contain production
cross-sections are provided in two forms
(`Prod, MT>1000` and `Prod, MT<1000`).
They include the same data but use different MT number
assignments for production data due to the fact that
MCNP 6.2 cannot handle production MT numbers greater than 999.
See the [next section](#coding-of-production-cross-sections)
for details.

The table below summarizes the available
files and indicates what data are included in the ace files.

|            | No Prod | Prod, MT>1000 | Prod, MT<1000 |
| ---------- | ------- | ------------- | ------------- |
| no delayed | [ZP0N_] | [ZP1N_]       | [ZP2N_]       |
| delayed    | [ZP0N1] | [ZP1N1]       | [ZP2N1]       |

## Coding of production cross sections

In the ace files under the directory [ZP1N_] and [ZP1N1],
long MT numbers for production are used, which are not
yet supported by MCNP 6.2. The associations are described
in the corresponding txt files. For instance, the following
lines from the file `g_26-Fe-56-2631.txt` for Fe-53,
```
   i     MT/MTD     Q [MeV]     T [MeV] LMF  MT    ZAP LFS
 ...
 211   50026053    0.000000   36.000000   6   5  26053   0
 212   51026053    0.000000   38.000000   6   5  26053   1
 ...
```
indicate that the MT number `50026053` is associated with
the production of the isotope Fe-53 (given in the column
`ZAP`) in the ground state (`LFS=0`).
Analogously, MT number `51026053` gives the same product
in a meta-stable level indicated by `LFS=1`.

In the ace files under the directory [ZP2N_] and [ZP2N1],
short MT numbers for production are used, which are supported
by MCNP 6.2. The assocations are described in the corresponding
txt files. Taking the same example as above,
```
   i     MT/MTD     Q [MeV]     T [MeV] LMF  MT    ZAP LFS
 ...
 211        428    0.000000   36.000000   6   5  26053   0
 212        429    0.000000   38.000000   6   5  26053   1
 ...
```
now the MT number associated with the production of Fe-53
in ground state is `428` and for the production of the
meta stable level is `429`.


[ZP0N_]: https://github.com/IAEA-NDS/IAEA-PD2019/tree/dev/application-lib/ZP0N_
[ZP1N_]: https://github.com/IAEA-NDS/IAEA-PD2019/tree/dev/application-lib/ZP1N_
[ZP2N_]: https://github.com/IAEA-NDS/IAEA-PD2019/tree/dev/application-lib/ZP2N_
[ZP0N1]: https://github.com/IAEA-NDS/IAEA-PD2019/tree/dev/application-lib/ZP0N1
[ZP1N1]: https://github.com/IAEA-NDS/IAEA-PD2019/tree/dev/application-lib/ZP1N1
[ZP2N1]: https://github.com/IAEA-NDS/IAEA-PD2019/tree/dev/application-lib/ZP2N1


[iaeapd19ace]: https://github.com/IAEA-NDS/IAEA-PD2019/blob/dev/application-lib/indc-nds-858-draft.pdf
