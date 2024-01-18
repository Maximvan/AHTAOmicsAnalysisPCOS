# Dataset 4 - Methylation profiling by genome tiling array 
The last dataset is Genome-wide DNA methylation analysis on PCOS using Illumina HumanMethylation 450K BeadChips in 30 PCOS patients and 30 healthy controls (GEO accesion number: GSE80468).

In the exploration of Polycystic Ovary Syndrome (PCOS), the Infinium HumanMethylation450k BeadChip platform was employed to analyze methylation profiles from 60 patients, including both PCOS and healthy tissues. Probes with insufficient statistical significance were filtered out using the pfilter function.

Data preprocessing involved reading raw intensity data from IDAT files using the readEPIC function from the wateRmelon package. Quality control, preprocessing, and normalization were then conducted with the minfi package. Dye color adjustment addressed technical biases, and Figure \ref{f5}  illustrates density and color bias adjustments using methylumi objects.

For differential methylation analysis, the limma package was employed to identify positions with distinct methylation patterns between PCOS and control groups.. Finally, gene set analysis was performed on both differentially methylated positions and regions, following the same methodology as described earlier. This comprehensive approach provides insights into the epigenetic differences associated with PCOS.
