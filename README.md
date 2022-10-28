# pbs-torque

This profile configures Snakemake to run on the pbspro version used by elta2 (Institute for molecular bioscience, University of Queensland).

## Setup

### Deploy profile

To deploy this profile, run

    mkdir -p ~/.config/snakemake
    cd ~/.config/snakemake
    cookiecutter https://github.com/GiulioCentorame/pbspro-delta2.git

Then, you can run Snakemake with

    snakemake --profile pbspro-delta2 ...


### Parameters

The following resources are supported by on a per-rule basis:

**node** - set the ppn resource request (defaults to the thread declaration).  
**mem** - set the memory resource request (bytes).  
**walltime** - set the walltime resource (secs).  
