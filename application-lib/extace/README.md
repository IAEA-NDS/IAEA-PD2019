# Extended application files

The ace files in the subdirectories
contain additional data that can be
used in Monte Carlo simulations.

The directory `with_delayed_neutron_data`
contains the same set of cross sections as
the corresponding files in `application-lib/ace`
but additionally include delayed neutron spectra
from photo-fission.

The directory `with_dosimetry_and_production`
contains the same set of cross sections as the
corresponding files in `application-lib/ace`
but additionally include dosimetry and production
data that can be used as a tally in Monte Carlo
simulations.

At the time of writing (July 2022), the current
MCNP version 6.2 cannot use these files but it
is expected that future versions of MCNP will be
able to use them.
