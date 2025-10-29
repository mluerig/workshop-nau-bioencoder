# BioEncoder workshop at Norther Arizona University

<div align="center">
    <img src="assets/banner.jpg" width="50%">
</div>

## Background

BioEncoder is a toolkit for supervised metric learning to i) learn and extract features from images, ii) enhance biological image classification, and iii) identify the features most relevant to classification. Designed for diverse and complex datasets, the package and the available metric losses can handle unbalanced classes and subtle phenotypic differences more effectively than non-metric approaches. The package includes taxon-agnostic data loaders, custom augmentation techniques, hyperparameter tuning through YAML configuration files, and rich model visualizations, providing a comprehensive solution for high-throughput analysis of biological images.

The paper: [https://onlinelibrary.wiley.com/doi/10.1111/ele.14495](https://onlinelibrary.wiley.com/doi/10.1111/ele.14495)


## Quickstart

Comprehensive help files are available in the package repo: [https://github.com/agporto/BioEncoder/tree/main/help](https://github.com/agporto/BioEncoder/tree/main/help).  

1\. Clone the repo, unpack, and go to the directory:
````
git clone https://github.com/mluerig/workshop-nau-bioencoder
## cd workshop-nau-bioencoder-main
````

2\. Install BioEncoder into a virtual environment with CUDA and pytorch: 

Make sure that mamba is installed and initialized. On monsoon the command is `module load mambaforge` 
````
mamba env create -f environment.yml
````

3\. Get the [dataset from the file hoster](https://www.dropbox.com/scl/fi/mxr6606ei5m88piwrtd19/junonia.zip?rlkey=1gzhckdxt9640zac6014gaifh&st=y9vn8iok&dl=0). Unzip and place the folder in `data_raw`.

4\. Activate the environment, and run the notebook - either in vscode or jupyter notebook / lab:

````
mamba activate bioencoder-env
jupyter notebook scripts\01_training_junonia.ipynb
````

Happy (en)coding!
