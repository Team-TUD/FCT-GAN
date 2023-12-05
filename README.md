# FCT_GAN
This code is for paper `FCT-GAN: Enhancing Table Synthesis via Fourier Transform`, which is published in CIKM 2023.

## Structure
- *Real_Datasets* Location of training data

- *Fake_Datasets* Location of generated data

- *model* Location of FCT-GAN model. The generator and discriminator structure definition is under `model/synthesizier/fctgan_synthesizer.py`. The main training logic is also within this file.

## Environment

The code is tested in following package version
```
numpy==1.21.0
torch==1.9.1
pandas==1.2.4
sklearn==0.24.1
dython==0.6.4.post1
scipy==1.4.1
```

## Dataset

We upload the `Adult` dataset as an example, we are not the owner of this dataset, please check its original [link](https://archive.ics.uci.edu/dataset/2/adult) for more information.

## Example
`Experiment_Script_Adult.ipynb` is a demo notebook. Under `Real_Datasets`, there are three csv files: `Adult.csv`, `Adult_corr.csv` and `Adult_type.csv`. They are corresponding to three column permutation orders of `Adult` dataset. The ML utility and Statistical similarity evaluations are also in the demo notebook.

To cite this paper, use the following bibtex for now:
```
@inproceedings{10.1145/3583780.3615202,
author = {Zhao, Zilong and Birke, Robert and Chen, Lydia Y.},
title = {FCT-GAN: Enhancing Global Correlation of Table Synthesis via Fourier Transform},
year = {2023},
isbn = {9798400701245},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3583780.3615202},
doi = {10.1145/3583780.3615202},
booktitle = {Proceedings of the 32nd ACM International Conference on Information and Knowledge Management},
pages = {4450–4454},
numpages = {5},
keywords = {tabular data, gan, fourier transform},
location = {Birmingham, United Kingdom},
series = {CIKM '23}
}


```