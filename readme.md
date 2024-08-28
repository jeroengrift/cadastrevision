# CadastreVision: A Benchmark Dataset for Cadastral Boundary Delineation from Multi-Resolution Earth Observation Images

## Authors
Jeroen Grift,
Claudio Persello,
Mila Koeva 

## Paper
- The related paper is available at: https://www.sciencedirect.com/science/article/pii/S0924271624003150
- The related benchmark dataset is available at: https://phys-techsciences.datastations.nl/dataset.xhtml?persistentId=doi:10.17026/PT/OS3OWX

Please be aware that the 8cm aerial imagery and the results of the overlap analysis (classfied cadastral reference) has not been published yet (due to upload restrictions). We will share this data as soon as possible

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
- fme/benchmark_preparation: preprocess the restricted data from CadastreVision (Planetscope and SuperView)
- fme/overlap_calculation: perform the overlap analysis between the cadastral boundaries from the CadastreVision dataset and physical topographic objects from several topographic maps

Auxiliary data is published in the data folder and contains:
- data/sample_tiles.gpkg: extents of the 90 sample tiles in GeoPackage format
- data/bestuurlijke_grenzen.gpkg: country border of the Netherlands

The topographic datasets are too large to share via DANS, so they could be downloaded with the following urls:
- data/brk: Please follow the instructions here to download current data: https://app.pdok.nl/kadaster/kadastralekaart/download-viewer/
- data/bgt: Please follow the instructions here to download current data: https://app.pdok.nl/lv/bgt/download-viewer/
- data/brt: Please follow the instructions here to download current data: https://service.pdok.nl/brt/topnl/atom/top10nl.xml
- data/brp: Please follow the instructions here to download current data: https://service.pdok.nl/rvo/brpgewaspercelen/atom/v1_0/basisregistratie_gewaspercelen_brp.xml
- data/bag: Please follow the instructions here to download current data: https://www.kadaster.nl/-/kosteloze-download-bag-2-0-extract

## Software requirements
Make sure FME Workbench 2024.0 is installed on your machine. Installation manuals and software documentation are available at: [https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm](https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm 'https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm')


