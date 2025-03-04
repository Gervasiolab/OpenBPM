# OpenBPMD - evaluating ligand pose stability using metadynamics

### Background 
OpenBPMD is an open source implementation of binding pose metadynamics (BPMD). Based on work by [Clark et al, 2016](https://doi.org/10.1021/acs.jctc.6b00201). Primarily built for reranking docked poses out of a list of candidates generated by a docking program. OpenBPMD biases ligands using metadynamics and evaluates how stable they are during the simulation. Recommended to be used in conjunction with [_grand_](https://github.com/essex-lab/grand) to optimise water networks around the ligand before subjecting it to metadynamics.

### Installation & Usage

The dependencies needed for running the scripts can be installed with conda:

```
conda create -n openbpmd
conda activate openbpmd

conda install -c conda-forge -c omnia openmm
conda install -c conda-forge mdanalysis
conda install -c conda-forge mdtraj
conda install -c conda-forge parmed
```

Once the dependencies have been installed, running OpenBPMD involves simply running one of the Python scripts. Have a look at the ```examples/``` directory for further instructions on how to run and analyse the OpenBPMD results.

### References

1. A. J. Clark, P. Tiwary, K. Borrelli, S. Feng, E. Miller, R. Abel, R. A. Friesner, B. J. Berne, _J. Chem. Theory Comput._ 2016, 12, 6, 2990–2998, DOI:[https://doi.org/10.1021/acs.jctc.6b00201](https://doi.org/10.1021/acs.jctc.6b00201) 
2. D. Lukauskis, M. L. Samways, S. Aureli, B. P. Cossins, R. D. Taylor, F. L. Gervasio, _J. Chem. Inf. Model._ 2022, 62, 23, 6209–6216, DOI:[https://doi.org/10.1021/acs.jctc.6b00201](https://doi.org/10.1021/acs.jcim.2c01142)
