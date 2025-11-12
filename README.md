# CESM2-project
-seasonality - avoids collapsing of time dimension via `average_time=False`

-take3 - original draft for plotting 21 year ensemble mean anomalies of sea level pressure (PSL) and 2m reference height temperature (TREFHT) 40-90N as a result of progression of anthropogenic aerosol forcing only (AAER), progression of greenhouse gas forcing only (GHG) and all forcings evolving (LE). Aim is to plot correlation (nonlinearity) in the signal between aerosol and greenhouse gas progression by subtracting 'all but' aerosol forcing (xAER) from LE, then subtracting AAER from this.

-If running from scratch, both scripts require .nc files covering AAER, xAER, LE, GHG forcings on both PSL and TREFHT variables from notable time periods:

1920-1939 - baseline,

1965-1985 - representing peak in aerosol emissions in EU/NA,

1994-2014 - current day,

2030-2050 - future scenario per SSP3-7.0 forecast

This will download new .nc files covering averages that can be recalled for reproducability.

.nc files supplied contain 1920-1940 'baseline' subtracted from 3 21 year averages per variable, as well as seasonal components (from code supplied, run already). Can be input to produce figures.

Note: AAER runs contains 20 ensemble members, xAER 10 members, LE 20 members, GHG 15 members.
