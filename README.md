# HEV ORF1 Molecular Dynamics whole atoms

The repository contains the samples input files and the Molecular Dynamics (MD) configuration files to run the simulations.

## Samples

The samples directory is composed of 3 subdirectories:

- WT: Wild Types samples.
- insertions: the samples with insertions in the Hyper Variable Region.
- duplications: the samples with duplications in the Hyper Variable Region.

Each subdirectory contains for each sample:

- the HEV ORF1 structure PDB file predicted from Alphafold2, the hydrogens of those PDB files were removed.
- the PRMTOP, topology files.
- the CRD, coordinates files.

## Configuration

The configuration directory, is composed of the AMBER configurations files requisite for the different stages of the MD:

- config_minimize-energy.in: the systems energy minimization.
- config_heating.in: the system heating step.
- config_MD-30M.in: the production configuration files to perform 30 millions of cycles steps.
