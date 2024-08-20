# Preprocess restricted data

To prepare the PlanetScope and SuperView data we first have to download the data from Satellietdataportaal. This process is described in download_readme.md

After downloading the data several FME script should be executed. Make sure FME Workbench 2024.0 is installed on your machine. Installation manuals and software documentation is available at: [https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm](https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm 'https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm')


## Preprocess PlanetScope
For PlanetScope data we have to run a single script. ClipPlanetScope.fmw is used to to preprocess the PlanetScope data downloaded from Satellietdataportaal. The script executes the following steps:

1. read sample tiles
2. read country border of NL
3. Read PlanetScope mosaic of NL
4. Clip the mosaic with the country border
5. Clip the result of step 4 per tile 
6. Georeference the result of step 5
7. Resample the result of step 6
8. Write the clipped mosiac per tile to a TIFF file

## Preprocess SuperView
For SuperView the preprocessing is based on two scripts: mosaicSuperView.fmw and runMosaicSuperView.fmw. The first processes the SuperView data per sample tile by using the following steps:
1. read sample tiles
2. Filter on tile name
3. Select the images that are in the tile dir
4. Read the images
5. Mosaic the images
6. Georeference and resample the images
7. Write the result to a TIFF file

runMosaicSuperView.fmw runs mosaicSuperView.fmw for all sample tiles (because running the script with all the 90 sample creates resource issues).


