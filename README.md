
# Introduction

Trajectory inference (TI) provides important insights in understanding cell development and biological process. However, the integration of transcriptomic profiles and spatial locations to organize spatiotemporal cell orders is currently remaining challenges. Here we introduce spaTrack, which effectively constructs cell trajectories from an optimal-transport matrix at single cell resolution, taking into account both profile of gene expression and distance cost of cell transition in a spatial context. 

spaTrack has the potential to capture fine local details of trajectory within a single tissue section of spatial transcriptomics (ST) data, as well as reconstruct cell dynamics across multiple tissue sections in a time series. To capture potential dynamic drivers, spaTrack models the fate of a cell as a function of expression profile along the time points driven by transcription factors, which facilitates the identification of key molecular regulators that govern cellular trajectories.

<div style="display: flex;">   <div style="flex-basis: 50%; padding-right: 10px;">     <img src="https://github.com/yzf072/spaTrack_tutorials/raw/main/docs/source/_static/TI.png" alt="Image 1" style="width: 100%;">     <p style="text-align: center;">Infer cell trajectory</p>   </div>   <div style="flex-basis: 50%; padding-left: 10px;">     <img src="https://github.com/yzf072/spaTrack_tutorials/raw/main/docs/source/_static/transfer.png" alt="Image 2" style="width: 100%;">     <p style="text-align: center;">Visualize cell transfer</p>   </div> </div>

# Highlighted features

**spaTrack**

* reconstructs fine local trajectories from ST data. 
* integrates spatial transition matrix of multiple samples to generate complete trajectories.
* traces cell trajectory across multiple tissue sections via direct mapping without integrating data. 
* captures the driven factors of differentiation.
* could be extensively applied on both ST data and scRNA-seq data.
* requires lower computing memory and loads than RNA-velocity methods, making it a fast and effective option for TI study.

# Installation

```shell
pip install spaTrack
```

# Turorials

We provide the following five tutorials as reference cases to illustrate the application of spaTrack in inferring cell trajectories on ST data of single slices with a single starting point and multiple starting points, as well as ST data of multiple time slices, and scRNA-seq data.

1. [Apply spaTrack to infer a trajectory on spatial transcriptomic data from axolotl brain regeneration after injury.](https://spatrack-tutorials.readthedocs.io/en/latest/notebooks/01.ST_data_of_axolotl_brain_regeneration_after_injury.html)

2. [Apply spaTrack to infer a trajectory on spatial transcriptomic data from 
    Intrahepatic cholangiocarcinoma cancer with multiple starting points.](https://spatrack-tutorials.readthedocs.io/en/latest/notebooks/02.ST_data_of_Intrahepatic_cholangiocarcinoma_cancer.html)

3. [Apply spaTrack to infer a trajectory on spatial transcriptomic data from multiple time slices of axolotl brain regeneration.](https://spatrack-tutorials.readthedocs.io/en/latest/notebooks/03.ST_data_of_axolotl_brain_slides_with_multiple_times.html)

4. [Apply spaTrack to infer cell transitions across multiple time points in spatial transcriptomic data from the mouse midbrain.](https://spatrack-tutorials.readthedocs.io/en/latest/notebooks/04.ST_data_of_mouse%20midbrain_with_multiple_times.html)

5. [Apply spaTrack to infer cell  trajectory in  scRNA-seq data from 
    hematopoietic stem cells development with multiple directions.](https://spatrack-tutorials.readthedocs.io/en/latest/notebooks/05.scRNAseq_data_of_HSC.html)



