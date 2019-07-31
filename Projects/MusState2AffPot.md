#Transforming muscle states into muscle spindle afferent potentials

## Data preparation
### CDS files
- CDS files need to have EMG and muscle lengths
  - If files do not have EMG, do not use file
  - If files do not have muscle lengths, either run with OpenSim, or do not use file
  
### TD files
- Check EMG envelopes
  - Should be fairly smooth
  - If not, reprocess from CDS->TD
- While TD structure is in "big" format, do all postprocessing
  - Make muscle lengths relative to mean
  - Normalize EMG to min-max ~ 0-1
- run splitTD.m to separate the TD files back into 

### Wrapper for running model
- Needs to take TD struct and params
- Single muscle?
- Will assign gamma and cdl variables from EMG and muscle lengths
- Needs to save back into TD format
