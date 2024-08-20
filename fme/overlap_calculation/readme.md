# Calculate overlap cadastral/topographic objects

To calculate the overlap, 8 FME scripts should be executed consecutively. 

Make sure FME Workbench 2024.0 is installed on your machine. Installation manuals and software documentation are available at: [https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm](https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm 'https://docs.safe.com/fme/html/FME-Form-Documentation/FME-Form/Home.htm')

The following describes the order and the purpose of the scripts (detailed documentation is added inside the scripts):

1. 1_OverlapBRKTopo.fmw: Performs the overlap analysis per tile
2. 2_runOverlapBRKTopo.fmw: Runs the overlap analysis for every tile
3. 3_mergeOverlapBRKTopo.fmw: Merges the output per tile to a single output 
4. 4_classifyOverlapBRKTopo.fmw: Classifies the matched cadastral boundaries to the classes as described in the paper per tile
5. 5_runClassifyOverlapBRKTopo.fmw: Merges the classification per tile to a single output
6. 6_analyseClassesOverlapBRKTopo.fmw: Analyses the length of the cadastral boundaries per class
7. 7_runAnalyseClassesOverlapBRKTopo.fmw: Runs the analysis for all the tiles
8. 8_finalStatsOverlapBRKTopo.fmw: Calculates the length of all matched and not-matched cadastral boundaries


