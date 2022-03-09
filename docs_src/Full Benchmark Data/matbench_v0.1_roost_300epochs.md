# matbench_v0.1: RooSt

### Algorithm description: 

Fit RooSt using 300 epochs and rest default parameters to serve as a baseline for RoosterCrab.

#### Notes:
A Jupyter notebook is provided which contains additional details about the run of the algorithm.

Raw data download and example notebook available [on the matbench repo](https://github.com/hackingmaterials/matbench/tree/main/benchmarks/matbench_v0.1_roost_300epochs).

### References (in bibtex format): 

```
['@article{goodallPredictingMaterialsProperties2020b, title = {Predicting '
 'Materials Properties without Crystal Structure: Deep Representation Learning '
 'from Stoichiometry}, shorttitle = {Predicting Materials Properties without '
 'Crystal Structure}, author = {Goodall, Rhys E. A. and Lee, Alpha A.}, year = '
 '{2020}, month = dec, journal = {Nat Commun}, volume = {11}, number = {1}, '
 'pages = {6280}, issn = {2041-1723}, doi = {10.1038/s41467-020-19964-7}, '
 'abstract = {Machine learning has the potential to accelerate materials '
 'discovery by accurately predicting materials properties at a low '
 'computational cost. However, the model inputs remain a key stumbling block. '
 'Current methods typically use descriptors constructed from knowledge of '
 'either the full crystal structure~\textemdash ~therefore only applicable to '
 'materials with already characterised structures~\textemdash ~or '
 'structure-agnostic fixed-length representations hand-engineered from the '
 'stoichiometry. We develop a machine learning approach that takes only the '
 'stoichiometry as input and automatically learns appropriate and '
 'systematically improvable descriptors from data. Our key insight is to treat '
 'the stoichiometric formula as a dense weighted graph between elements. '
 'Compared to the state of the art for structure-agnostic methods, our '
 'approach achieves lower errors with less data.}, langid = {english}}']
```

### User metadata:

```
{}
```

### Metadata:

| tasks recorded | 1/13 |
|----------------|-------------------------------------|
| complete? | ✗ | 
| composition complete? | ✗ | 
| structure complete? | ✗ | 
| regression complete? | ✗ | 
| classification complete? | ✗ | 

### Software Requirements

```
{'python': [['scipy',
             'tqdm',
             'torch',
             'numpy',
             'pymatgen',
             'torch_scatter',
             'pandas',
             'scikit_learn',
             'pytest',
             'tensorboard']]}
```

### Task data:

#### `matbench_expt_gap`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.3489| 0.7867| 0.3758| 4.5950 |
 | fold_1 | 0.3941| 0.9233| 0.3559| 6.5301 |
 | fold_2 | 0.4200| 0.9970| 0.3866| 8.2795 |
 | fold_3 | 0.4465| 1.0256| 0.4666| 7.5853 |
 | fold_4 | 0.4429| 0.9059| 0.4211| 4.8957 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.4105 | 0.4465 | 0.3489 | 0.0360 |
| rmse | 0.9277 | 1.0256 | 0.7867 | 0.0834 |
| mape* | 0.4012 | 0.4666 | 0.3559 | 0.0389 |
| max_error | 6.3771 | 8.2795 | 4.5950 | 1.4473 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'epochs': 300}` |
| fold_1 | `{'epochs': 300}` |
| fold_2 | `{'epochs': 300}` |
| fold_3 | `{'epochs': 300}` |
| fold_4 | `{'epochs': 300}` |




