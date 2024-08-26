# CadastreVision: A Benchmark Dataset for Cadastral Boundary Delineation from Multi-Resolution Earth Observation Images

## Authors
Jeroen Grift,
Claudio Persello,
Mila Koeva 

## Paper
- The related paper is available at: https://www.sciencedirect.com/science/article/pii/S0924271624003150
- The related benchmark dataset is available at: https://phys-techsciences.datastations.nl/dataset.xhtml?persistentId=doi:10.17026/PT/OS3OWX

To cite the paper/benchmark dataset, please use this bib file:
```
@article{cadastrevision,
  title={CadastreVision: A Benchmark Dataset for Cadastral Boundary Delineation from Multi-Resolution Earth Observation Images},
  author={Grift, Jeroen and Persello, Claudio and Grift, Jeroen and Koeva, Mila},
  journal={{ISPRS Journal of Photogrammetry and Remote Sensing},
  volume={217}
  number={}
  pages={91-100}
  year={2024}
}
```

## This repository
In this repository, we publish two types of FME pipelines:
- fme/benchmark_preperation: preprocess the restricted data from CadastreVision (Planetscope and SuperView)
- fme/overlap_calculation: perform the overlap analysis between the cadastral boundaries from the CadastreVision dataset and physical topographic objects from several topographic maps 

## Software requirements
Make sure FME Workbench 2024.0 is installed on your machine. Installation manuals and software documentation are available at: [https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm](https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm 'https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm')


