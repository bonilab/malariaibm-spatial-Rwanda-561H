# malariaibm-spatial-Rwanda-561H

[Penn State](https://www.psu.edu/) - [Center for Infectious Disease Dynamics (CIDD)](https://www.huck.psu.edu/institutes-and-centers/center-for-infectious-disease-dynamics) - [Boni Lab](http://mol.ax/)

---

# Overview

This repository contains a frozen snapshot of the source code and intermediary files to accompany the manuscript by Zupko et al. (In Press) which will appear in *Nature Medicine*. Due to the size of the intermediary data (479 MB, compressed) this repository uses [Git Large File Storage](https://git-lfs.github.com/) and may be limited in terms of bandwidth as a result. All studies run by the simulation use YAML files (in Studies) to provide the configuration and ASC files (in `Data/GIS`) for spatial data.

Due to the complex nature of the simulation, [primary living documentation](https://github.com/rjzupkoii/PSU-CIDD-Malaria-Simulation) to build and run the simulation is hosted with the repository that contains active development. The version 4.1.4 code base was used to run all replicates for the studies presented in the manuscript.

---

## Organization

Contents of the `Study` directory are organized in the following fashion for the primary studies of the manuscript under the `Policy Interventions` sub-directory:

| Type | Study Name | Filename |
| --- | --- | --- |
| AL Replacement | AL replacement with ASAQ | AL Replacement/rwa-replacement-asaq.yml |
| AL Replacement | AL replacement with DHA-PPQ | AL Replacement/rwa-replacement-dhappq.yml |
| Artesunate Extension | Extension of artesunate, four day course | Artesunate Extension/rwa-ae-al-4.yml |
| Artesunate Extension | Extension of artesunate, five day course| Artesunate Extension/rwa-ae-al-5.yml |
| Artesunate Extension | Extension of artesunate, three-day course on days 0, 1, 2; followed by second course on days 7, 8, 9 | Artesunate Extension/rwa-ae-al-3-4-3.yml |
| Baseline | Status quo with no interventions | Baseline/rwa-pfpr-constant.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, AL (75%) and ASAQ (25%) | Multiple First-Line Therapies/rwa-mft-al-asaq-0.25.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, AL (50%) and ASAQ (50%) | Multiple First-Line Therapies/rwa-mft-al-asaq.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, AL (25%) and ASAQ (75%) | Multiple First-Line Therapies/rwa-mft-al-asaq-0.75.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, AL (75%) and DHA-PPQ (25%) | Multiple First-Line Therapies/rwa-mft-al-dhappq-0.25.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, AL (50%) and DHA-PPQ (50%) | Multiple First-Line Therapies/rwa-mft-al-dhappq.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, AL (25%) and DHA-PPQ (75%) | Multiple First-Line Therapies/rwa-mft-al-dhappq-0.75.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, ASAQ (75%) and DHA-PPQ (25%) | Multiple First-Line Therapies/rwa-mft-asaq-dhappq-0.25.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, ASAQ (50%) and DHA-PPQ (50%) | Multiple First-Line Therapies/rwa-mft-asaq-dhappq.yml |
| Multiple First-Line Therapies |  Multiple First-Line Therapies, ASAQ (25%) and DHA-PPQ (75%) | Multiple First-Line Therapies/rwa-mft-asaq-dhappq-0.75.yml |
| Rotation | Therapy rotation / switching, Three years of DHA-PPQ followed by AL (50%) and ASAQ (50%) | Rotation/rwa-rotation-al-3.yml |
| Rotation | Therapy rotation / switching, Three years of DHA-PPQ followed by AL five day course (50%) and ASAQ (50%) | Rotation/rwa-rotation-al-5.yml |
| Sequential Dosing | Sequential course of three-day ACT; AL, four day pause, then by ASAQ | Sequential Dosing/rwa-seq-al-asaq-pause.yml |
| Sequential Dosing | Sequential course of three-day ACT; AL followed by ASAQ | Sequential Dosing/rwa-seq-al-asaq.yml |
| Sequential Dosing | Sequential course of three-day ACT; AL, four day pause, then by DHA-PPQ | Sequential Dosing/rwa-seq-al-dhappq-pause.yml |
| Sequential Dosing | Sequential course of three-day ACT; AL followed by DHA-PPQ | Sequential Dosing/rwa-seq-al-dhappq.yml |
| Sequential Dosing | Sequential course of three-day ACT; ASAQ, four day pause, then by AL | Sequential Dosing/rwa-seq-asaq-al-pause.yml |
| Sequential Dosing | Sequential course of three-day ACT; ASAQ followed by AL | Sequential Dosing/rwa-seq-asaq-al.yml |
| Sequential Dosing | Sequential course of three-day ACT; DHA-PPQ, four day pause, then by AL | Sequential Dosing/rwa-seq-dhappq-al-pause.yml |
| Sequential Dosing | Sequential course of three-day ACT; DHA-PPQ followed by AL | Sequential Dosing/rwa-seq-dhappq-al.yml |
| Triple ACT | AL + AQ | TACT/rwa-tact-alaq.yml |
| Triple ACT | DHAPPQ + MQ | TACT/rwa-tact-dhappqmq.yml |

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
- Malaria Simulation, version 4.1.4: https://github.com/rjzupkoii/PSU-CIDD-Malaria-Simulation
- Rwanda analysis and plots: https://github.com/rjzupkoii/PSU-CIDD-Rwanda
- Support scripts and infrastructure: https://github.com/bonilab/PSU-CIDD-MaSim-Support
