## ESM2M-BLING perturbation experiments

Analysis of perturbation experiments with ESM2M.  

The root directory for experiments is here: `/archive/Richard.Slater/Siena/siena_201308_rds-c3-gat-slurm/`  
There are two important configurations there: `MOM5_SIS_BLING_CORE2-gat` and `MOM5_SIS_BLING_CORE2-gat-override-po4`  
The full postprocess path for e.g. no-override experiment is thus: `/archive/Richard.Slater/Siena/siena_201308_rds-c3-gat-slurm/MOM5_SIS_BLING_CORE2-gat/gfdl.ncrc3-intel16-prod-openmp/pp`  

Within each postprocess file directory, there are files for the 4 experiments, including a control (no suffix), a control with general atmospheric tracer (`_gat`), an experiment where the phytoplankton growth rate is doubled for one year (`_double`), and an experiment where the phytoplankton growth rate is zero'd for one year (`_zero`).  

Because of some unconventional file namings, wrapper functions to load the experiment data (around `gfdl_utils`) are available in the `bio-pump-timescales` package, within the `config` package.

The model spin-up is available here : `/archive/Richard.Slater/Siena/siena_201308_rds-c3-gat-slurm/MOM5_SIS_BLING_CORE2-spinup-intel19/gfdl.ncrc3-intel19-prod-openmp/pp`

***
### Details of experimental design

### Derived data
Processed data (e.g. global integrals) can be found in `/work/Graeme.Macgilchrist/projects/bio-pump-timescales/data/processed/`.
