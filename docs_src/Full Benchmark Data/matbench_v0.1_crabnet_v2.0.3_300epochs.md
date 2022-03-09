# matbench_v0.1: CrabNet v2.0.3

### Algorithm description: 

Fit CrabNet using 300 epochs and rest default parameters to serve as a baseline for RoosterCrab.

#### Notes:
A Jupyter notebook is provided which contains additional details about the run of the algorithm.

Raw data download and example notebook available [on the matbench repo](https://github.com/hackingmaterials/matbench/tree/main/benchmarks/matbench_v0.1_crabnet_v2.0.3_300epochs).

### References (in bibtex format): 

```
['@article{Wang2021crabnet,\n'
 ' author = {Wang, Anthony Yu-Tung and Kauwe, Steven K. and Murdock, Ryan J. '
 'and Sparks, Taylor D.},\n'
 ' year = {2021},\n'
 ' title = {Compositionally restricted attention-based network for materials '
 'property predictions},\n'
 ' pages = {77},\n'
 ' volume = {7},\n'
 ' number = {1},\n'
 ' doi = {10.1038/s41524-021-00545-1},\n'
 ' publisher = {{Nature Publishing Group}},\n'
 ' shortjournal = {npj Comput. Mater.},\n'
 ' journal = {npj Computational Materials}\n'
 ' }']
```

### User metadata:

```
{'version': '2.0.3'}
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
{'python': [['crabnet==2.0.3', 'scikit_learn==1.0.2', 'matbench==0.5']]}
```

### Task data:

#### `matbench_expt_gap`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.6455| 1.2865| 0.7696| 7.9511 |
 | fold_1 | 0.7537| 1.4809| 0.7225| 9.2574 |
 | fold_2 | 0.7256| 1.5094| 0.9986| 11.6917 |
 | fold_3 | 0.6725| 1.3704| 0.8278| 10.4711 |
 | fold_4 | 0.6766| 1.3577| 0.9637| 9.7040 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.6948 | 0.7537 | 0.6455 | 0.0392 |
| rmse | 1.4010 | 1.5094 | 1.2865 | 0.0825 |
| mape* | 0.8564 | 0.9986 | 0.7225 | 0.1077 |
| max_error | 9.8151 | 11.6917 | 7.9511 | 1.2450 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'epochs': 300}` |
| fold_1 | `{'epochs': 300}` |
| fold_2 | `{'epochs': 300}` |
| fold_3 | `{'epochs': 300}` |
| fold_4 | `{'epochs': 300}` |




