# malariaibm-spatial-Rwanda-561H

[Penn State](https://www.psu.edu/) - [Center for Infectious Disease Dynamics (CIDD)](https://www.huck.psu.edu/institutes-and-centers/center-for-infectious-disease-dynamics) - [Boni Lab](http://mol.ax/)

---

# Overview

This repository contains a frozen snapshot of the source code and intermediary files to accompany the manuscript by Zupko et al., which is currently in preperation. Due to the size of the intermedary data (285 MB, compressed) this repsitory uses [Git Large File Storage](https://git-lfs.github.com/) and may be limited in terms of bandwidth as a result. All studies run by the simuation use YAML files (in Studies) to provide the configurationa nd ASC files (in Data/GIS) for spaital data.

Due to the complex nature of the simuation, [primary living documentation](https://github.com/rjzupkoii/PSU-CIDD-Malaria-Simulation) to build and run the simuation is hosted with the repository that contains active development. The version 4.1.1 code base was used to run the replicates used in manuscript revisions.

---

## Organization

Contents of the Study directory are organized in the following fashion:

| Type | Study Name | Filename |
| --- | --- | --- |
| Status Quo | Status quo with no interventions | Baseline/rwa-pfpr-constant.yml |

## Binary Files

The complied version fo the simulation used for studies is provided in the `Binaries` directory, which was compiled and run in the following environment:

```
LSB Version:    :core-4.1-amd64:core-4.1-noarch:cxx-4.1-amd64:cxx-4.1-noarch:desktop-4.1-amd64:desktop-4.1-noarch:languages-4.1-amd64:languages-4.1-noarch:printing-4.1-amd64:printing-4.1-noarch
Distributor ID: RedHatEnterpriseServer
Description:    Red Hat Enterprise Linux Server release 7.9 (Maipo)
Release:        7.9
Codename:       Maipo
```

---

### Original Repositories
- Malaria Simulation, version 4.1.1: https://github.com/rjzupkoii/PSU-CIDD-Malaria-Simulation
- Burkina Faso analysis and plots: https://github.com/rjzupkoii/PSU-CIDD-Rwanda
- Support scripts and infrastructure: https://github.com/bonilab/PSU-CIDD-MaSim-Support
