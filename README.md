# Dataset of N-doped graphene based single atom catalysts (M@C<sub>(4-x)</sub>N<sub>x</sub>)

In our work of [Design Principle of Carbon-Supported Single-Atom Catalysts – Interplay between d-Orbital Periodicity and Local Hybridization](https://pubs.acs.org/doi/full/10.1021/acs.chemmater.3c02549), we 
developed a computational dataset with 140 catalysts and 560 adsorption energies. Based on such dataset, we have established
 a design principle for understanding the catalytic process M@C<sub>(4-x)</sub>N<sub>x</sub>. For promoting the transparency
of our research, we have open sourced all our DFT data in this Github Repo

## Free energy diagram
The free energy diagram of HER and OER processes have been dumped in `./predicted_performance/FreeEnergy`

## Overpotential map
The map of overpotentials of HER and ORR reactions as being shown in our research paper has been demonstrated in `./predicted_performance/overpotential`

## Interactive dataset
The interactive version of the dataset is available as [HER Free Energy](https://jeff-oakley.github.io/SAC_HOER_data/heatmap_HER.html)
and [ORR Free Energy](https://jeff-oakley.github.io/SAC_HOER_data/heatmap_ORR.html)

## Raw DFT data
The raw DFT data, have been preprared and dumped in `./RawData` folder. The final overpotentials for HER and ORR are summarized in `eta.csv` file.

#### Input data files:
* `INCAR`: The INCAR we used for DFT relaxation for both substrate and adsorption model.
* `KPOINTS`: The KPOINTS we selected for DFT relaxation.
* `POTCAR_info`: The POTCAR version we used for generating the raw data. Note that VASP does not allow sharing POTCAR directory.
* `CONTCAR`: The final atomic model we obtained after DFT relaxation.
* `OSZICAR`: The energy profile of DFT relaxation.

#### Script for reproducing the results of our paper:

## Citing
We offer such dataset for promoting the transparency of research. Whenever our repo can be useful for you, 
please consider citing our paper
```
@article{SAC_HEOR,
  title={Design principle of carbon supported single atom catalyst – interplay between d-band periodicity and local hybridization},
  author={He, Zhengda and Wang, Jingyang and Ouyang, Bin},
  journal={Chemistry of Materials},
  html={https://pubs.acs.org/doi/full/10.1021/acs.chemmater.3c02549},
  year={2023}
}
```
