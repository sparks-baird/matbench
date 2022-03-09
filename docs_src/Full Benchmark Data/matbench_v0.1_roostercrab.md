# matbench_v0.1: RoosterCrab

### Algorithm description: 

Fit CrabNet and RooSt using 300 epochs, assign compounds to clusters based on chemical similarity, and choose to use CrabNet or RooSt for each compound based on whether the containing cluster sees overall better performance with CrabNet or RooSt, respectively.

#### Notes:
A Jupyter notebook is provided which contains additional details about the run of the algorithm.

Raw data download and example notebook available [on the matbench repo](https://github.com/hackingmaterials/matbench/tree/main/benchmarks/matbench_v0.1_roostercrab).

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
{'python': [['crabnet==2.0.3',
             'scikit_learn==1.0.2',
             'matbench==0.5',
             'scipy',
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
 | fold_0 | 0.3465| 0.7806| 0.3790| 4.5950 |
 | fold_1 | 0.3893| 0.9061| 0.3552| 6.5301 |
 | fold_2 | 0.4205| 0.9952| 0.3856| 8.2795 |
 | fold_3 | 0.4628| 1.1408| 0.4746| 10.4711 |
 | fold_4 | 0.4429| 0.9059| 0.4211| 4.8957 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.4124 | 0.4628 | 0.3465 | 0.0410 |
| rmse | 0.9457 | 1.1408 | 0.7806 | 0.1191 |
| mape* | 0.4031 | 0.4746 | 0.3552 | 0.0415 |
| max_error | 6.9543 | 10.4711 | 4.5950 | 2.1958 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'num_clusters': 11}` |
| fold_1 | `{'num_clusters': 15}` |
| fold_2 | `{'num_clusters': 17}` |
| fold_3 | `{'num_clusters': 14}` |
| fold_4 | `{'num_clusters': 18}` |




