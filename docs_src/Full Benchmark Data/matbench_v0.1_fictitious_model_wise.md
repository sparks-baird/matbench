# matbench_v0.1: fictitious_model

### Algorithm description: 

Fictitious model ensemble where (intentionally p-hacked) optimal weights were found based on ~130k SOBOL-sampled weight combinations of the various models for each of the task/fold combinations. Also referred to as a weighted ensemble average.

#### Notes:
No notes.

Raw data download and example notebook available [on the matbench repo](https://github.com/hackingmaterials/matbench/tree/main/benchmarks/matbench_v0.1_fictitious_model_wise).

### References (in bibtex format): 

```
('@article{Dunn2020,\n'
 '  doi = {10.1038/s41524-020-00406-3},\n'
 '  url = {https://doi.org/10.1038/s41524-020-00406-3},\n'
 '  year = {2020},\n'
 '  month = sep,\n'
 '  publisher = {Springer Science and Business Media {LLC}},\n'
 '  volume = {6},\n'
 '  number = {1},\n'
 '  author = {Alexander Dunn and Qi Wang and Alex Ganose and Daniel Dopp and '
 'Anubhav Jain},\n'
 '  title = {Benchmarking materials property prediction methods: the Matbench '
 'test set and Automatminer reference algorithm},\n'
 '  journal = {npj Computational Materials}\n'
 '}')
```

### User metadata:

```
{}
```

### Metadata:

| tasks recorded | 13/13 |
|----------------|-------------------------------------|
| complete? | ✓ | 
| composition complete? | ✓ | 
| structure complete? | ✓ | 
| regression complete? | ✓ | 
| classification complete? | ✓ | 

### Software Requirements

```
{'python': ['scikit-learn==0.24.1', 'numpy==1.20.1', 'matbench==0.1.0']}
```

### Task data:

#### `matbench_dielectric`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.1736| 0.6474| 0.0587| 14.0358 |
 | fold_1 | 0.2564| 1.0394| 0.0836| 19.4483 |
 | fold_2 | 0.3997| 2.9327| 0.0801| 59.0262 |
 | fold_3 | 0.2760| 2.2449| 0.0551| 52.4163 |
 | fold_4 | 0.2931| 1.5846| 0.0887| 28.0063 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.2798 | 0.3997 | 0.1736 | 0.0726 |
| rmse | 1.6898 | 2.9327 | 0.6474 | 0.8214 |
| mape* | 0.0733 | 0.0887 | 0.0551 | 0.0136 |
| max_error | 34.5866 | 59.0262 | 14.0358 | 17.9443 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.20575117871423193, 'matbench_v0.1_alignn': 0.36503077350276164, 'matbench_v0.1_automatminer_expressv2020': 0.03693776452273196, 'matbench_v0.1_modnet_v0.1.10': 0.3922802832...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.15967213462626922, 'matbench_v0.1_alignn': 0.019957298927968287, 'matbench_v0.1_automatminer_expressv2020': 0.22950980783361521, 'matbench_v0.1_modnet_v0.1.10': 0.590860758...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.26752136323219017, 'matbench_v0.1_alignn': 0.00022466871513461952, 'matbench_v0.1_automatminer_expressv2020': 0.32256934842943974, 'matbench_v0.1_modnet_v0.1.10': 0.4096846...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.07708241986797697, 'matbench_v0.1_alignn': 0.22901497809874913, 'matbench_v0.1_automatminer_expressv2020': 0.08756035007079653, 'matbench_v0.1_modnet_v0.1.10': 0.6063422519...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.40492091223579596, 'matbench_v0.1_alignn': 0.01928753160915624, 'matbench_v0.1_automatminer_expressv2020': 0.21645513538860056, 'matbench_v0.1_modnet_v0.1.10': 0.3593364207...` |




#### `matbench_expt_gap`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.3135| 0.6275| 0.3085| 5.1756 |
 | fold_1 | 0.3282| 0.6640| 0.2527| 6.7164 |
 | fold_2 | 0.3390| 0.7782| 0.3133| 8.8678 |
 | fold_3 | 0.3086| 0.6647| 0.2919| 5.4599 |
 | fold_4 | 0.3199| 0.6526| 0.3583| 5.6826 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.3218 | 0.3390 | 0.3086 | 0.0108 |
| rmse | 0.6774 | 0.7782 | 0.6275 | 0.0522 |
| mape* | 0.3049 | 0.3583 | 0.2527 | 0.0341 |
| max_error | 6.3805 | 8.8678 | 5.1756 | 1.3480 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.25328331229913154, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.19279284485612228, 'matbench_v0.1_modnet_v0.1.10': 0.5539238428447462, 'target'...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.5107847473559838, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.1463424463386866, 'matbench_v0.1_modnet_v0.1.10': 0.3428728063053297, 'target': ...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.6865386216198438, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.12547388312292732, 'matbench_v0.1_modnet_v0.1.10': 0.18798749525722885, 'target'...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.4973765410211031, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.07069597545395823, 'matbench_v0.1_modnet_v0.1.10': 0.43192748352493865, 'target'...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.24897538653903542, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.14684490360565391, 'matbench_v0.1_modnet_v0.1.10': 0.6041797098553107, 'target'...` |




#### `matbench_expt_is_metal`

###### Fold scores

| fold | accuracy | balanced_accuracy | f1 | rocauc |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.9218| 0.9218| 0.9205| 0.9218 |
 | fold_1 | 0.9157| 0.9156| 0.9145| 0.9156 |
 | fold_2 | 0.9207| 0.9207| 0.9193| 0.9207 |
 | fold_3 | 0.9228| 0.9228| 0.9223| 0.9228 |
 | fold_4 | 0.9238| 0.9238| 0.9235| 0.9238 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| accuracy | 0.9210 | 0.9238 | 0.9157 | 0.0028 |
| balanced_accuracy | 0.9209 | 0.9238 | 0.9156 | 0.0028 |
| f1 | 0.9200 | 0.9235 | 0.9145 | 0.0031 |
| rocauc | 0.9209 | 0.9238 | 0.9156 | 0.0028 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999994636097223, 'matbench_v0.1_modnet_v0.1.10': 5.363902777989782e-07, 'target': 0.0}` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999975241578845, 'matbench_v0.1_modnet_v0.1.10': 2.4758421155135045e-06, 'target': 0.0}` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999913986660386, 'matbench_v0.1_modnet_v0.1.10': 8.601333961434646e-06, 'target': 0.0}` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999938365545721, 'matbench_v0.1_modnet_v0.1.10': 6.16344542788228e-06, 'target': 0.0}` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999802552040563, 'matbench_v0.1_modnet_v0.1.10': 1.974479594366695e-05, 'target': 0.0}` |




#### `matbench_glass`

###### Fold scores

| fold | accuracy | balanced_accuracy | f1 | rocauc |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.8283| 0.8441| 0.8697| 0.8441 |
 | fold_1 | 0.8125| 0.8383| 0.8548| 0.8383 |
 | fold_2 | 0.8574| 0.8546| 0.8956| 0.8546 |
 | fold_3 | 0.9173| 0.8742| 0.9437| 0.8742 |
 | fold_4 | 0.9375| 0.8921| 0.9579| 0.8921 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| accuracy | 0.8706 | 0.9375 | 0.8125 | 0.0490 |
| balanced_accuracy | 0.8607 | 0.8921 | 0.8383 | 0.0199 |
| f1 | 0.9043 | 0.9579 | 0.8548 | 0.0404 |
| rocauc | 0.8607 | 0.8921 | 0.8383 | 0.0199 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999959766363284, 'matbench_v0.1_modnet_v0.1.10': 4.023363671606479e-06, 'target': 0.0}` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999933773656292, 'matbench_v0.1_modnet_v0.1.10': 6.622634370803024e-06, 'target': 0.0}` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999955134857657, 'matbench_v0.1_modnet_v0.1.10': 4.486514234348761e-06, 'target': 0.0}` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999873715803423, 'matbench_v0.1_modnet_v0.1.10': 1.2628419657670107e-05, 'target': 0.0}` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.9999923643049671, 'matbench_v0.1_modnet_v0.1.10': 7.635695032953968e-06, 'target': 0.0}` |




#### `matbench_jdft2d`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 25.6817| 45.6908| 20.8585| 201.4303 |
 | fold_1 | 27.7426| 63.3403| 0.2270| 367.3741 |
 | fold_2 | 50.8337| 147.0971| 0.5943| 846.5039 |
 | fold_3 | 24.9264| 50.6733| 0.2358| 302.0936 |
 | fold_4 | 37.7280| 151.3688| 0.4895| 1533.5975 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 33.3825 | 50.8337 | 24.9264 | 9.8594 |
| rmse | 91.6341 | 151.3688 | 45.6908 | 47.3993 |
| mape* | 4.4810 | 20.8585 | 0.2270 | 8.1900 |
| max_error | 650.1999 | 1533.5975 | 201.4303 | 494.2650 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.15342414366645282, 'matbench_v0.1_alignn': 0.03181279451221846, 'matbench_v0.1_automatminer_expressv2020': 0.446224463518545, 'matbench_v0.1_modnet_v0.1.10': 0.368538598302...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.01712548352219769, 'matbench_v0.1_alignn': 0.0008425195852314279, 'matbench_v0.1_automatminer_expressv2020': 0.028448329464033657, 'matbench_v0.1_modnet_v0.1.10': 0.9535836...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.0005454254242677881, 'matbench_v0.1_alignn': 0.18050122343170372, 'matbench_v0.1_automatminer_expressv2020': 0.02001052727974478, 'matbench_v0.1_modnet_v0.1.10': 0.79894282...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.17966803253404068, 'matbench_v0.1_alignn': 0.1828427612410428, 'matbench_v0.1_automatminer_expressv2020': 0.2321150227627915, 'matbench_v0.1_modnet_v0.1.10': 0.405374183462...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.0004628740793511039, 'matbench_v0.1_alignn': 0.25457773015822455, 'matbench_v0.1_automatminer_expressv2020': 0.13933131094614346, 'matbench_v0.1_modnet_v0.1.10': 0.60562808...` |




#### `matbench_log_gvrh`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0671| 0.1030| 0.0533| 0.9089 |
 | fold_1 | 0.0685| 0.1081| 0.0551| 1.1515 |
 | fold_2 | 0.0676| 0.1055| 0.0543| 0.8141 |
 | fold_3 | 0.0676| 0.1046| 0.0528| 0.8935 |
 | fold_4 | 0.0669| 0.1052| 0.0525| 0.7486 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0675 | 0.0685 | 0.0669 | 0.0006 |
| rmse | 0.1053 | 0.1081 | 0.1030 | 0.0017 |
| mape* | 0.0536 | 0.0551 | 0.0525 | 0.0010 |
| max_error | 0.9033 | 1.1515 | 0.7486 | 0.1368 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.0005469296890628186, 'matbench_v0.1_alignn': 0.5790363091121159, 'matbench_v0.1_automatminer_expressv2020': 0.016475670548405624, 'matbench_v0.1_modnet_v0.1.10': 0.40394109...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.0008720753148568775, 'matbench_v0.1_alignn': 0.5398068953552143, 'matbench_v0.1_automatminer_expressv2020': 0.00293608420564664, 'matbench_v0.1_modnet_v0.1.10': 0.456384945...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.00397918306233581, 'matbench_v0.1_alignn': 0.5905921519766839, 'matbench_v0.1_automatminer_expressv2020': 0.0013491061186301629, 'matbench_v0.1_modnet_v0.1.10': 0.404079558...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.0036578251362713926, 'matbench_v0.1_alignn': 0.5745243458793965, 'matbench_v0.1_automatminer_expressv2020': 0.0007068555241777903, 'matbench_v0.1_modnet_v0.1.10': 0.4211109...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.004858865465360498, 'matbench_v0.1_alignn': 0.510039374033992, 'matbench_v0.1_automatminer_expressv2020': 0.0015554463592616025, 'matbench_v0.1_modnet_v0.1.10': 0.483546314...` |




#### `matbench_log_kvrh`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0505| 0.0987| 0.0335| 1.5820 |
 | fold_1 | 0.0522| 0.1061| 0.0343| 1.3186 |
 | fold_2 | 0.0477| 0.0922| 0.0318| 1.1371 |
 | fold_3 | 0.0554| 0.1091| 0.0400| 1.0836 |
 | fold_4 | 0.0514| 0.1001| 0.0345| 1.3635 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0514 | 0.0554 | 0.0477 | 0.0025 |
| rmse | 0.1012 | 0.1091 | 0.0922 | 0.0059 |
| mape* | 0.0348 | 0.0400 | 0.0318 | 0.0027 |
| max_error | 1.2970 | 1.5820 | 1.0836 | 0.1773 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.0021430310672584164, 'matbench_v0.1_alignn': 0.44012112653432134, 'matbench_v0.1_automatminer_expressv2020': 0.037587235031681716, 'matbench_v0.1_modnet_v0.1.10': 0.5201486...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.011125181281904034, 'matbench_v0.1_alignn': 0.4454571849332936, 'matbench_v0.1_automatminer_expressv2020': 0.04526796006356993, 'matbench_v0.1_modnet_v0.1.10': 0.4981496737...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.035214279444113504, 'matbench_v0.1_alignn': 0.4542466438434961, 'matbench_v0.1_automatminer_expressv2020': 0.002799658586453697, 'matbench_v0.1_modnet_v0.1.10': 0.507739418...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.001317193865459212, 'matbench_v0.1_alignn': 0.3612906935102406, 'matbench_v0.1_automatminer_expressv2020': 0.12549697847265245, 'matbench_v0.1_modnet_v0.1.10': 0.5118951341...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.0013550637888710693, 'matbench_v0.1_alignn': 0.3972992478093793, 'matbench_v0.1_automatminer_expressv2020': 0.1239877770792496, 'matbench_v0.1_modnet_v0.1.10': 0.4773579113...` |




#### `matbench_mp_e_form`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0217| 0.0631| 0.1491| 3.5983 |
 | fold_1 | 0.0220| 0.0533| 0.1330| 2.8653 |
 | fold_2 | 0.0210| 0.0496| 0.1395| 2.0082 |
 | fold_3 | 0.0219| 0.0543| 0.1831| 1.6367 |
 | fold_4 | 0.0211| 0.0500| 0.2482| 1.3868 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0215 | 0.0220 | 0.0210 | 0.0004 |
| rmse | 0.0541 | 0.0631 | 0.0496 | 0.0049 |
| mape* | 0.1706 | 0.2482 | 0.1330 | 0.0425 |
| max_error | 2.2991 | 3.5983 | 1.3868 | 0.8203 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.008499291160418577, 'matbench_v0.1_alignn': 0.9032029811240486, 'matbench_v0.1_automatminer_expressv2020': 0.007458152631024239, 'matbench_v0.1_modnet_v0.1.10': 0.080839575...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.004977249815968251, 'matbench_v0.1_alignn': 0.9004650742942951, 'matbench_v0.1_automatminer_expressv2020': 0.002291709303718508, 'matbench_v0.1_modnet_v0.1.10': 0.092265966...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.017394782923472796, 'matbench_v0.1_alignn': 0.9120658902185469, 'matbench_v0.1_automatminer_expressv2020': 0.0015317067352738955, 'matbench_v0.1_modnet_v0.1.10': 0.06900762...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.008004151413010018, 'matbench_v0.1_alignn': 0.9272266729313643, 'matbench_v0.1_automatminer_expressv2020': 0.006611717219836468, 'matbench_v0.1_modnet_v0.1.10': 0.058157458...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.006685517382035754, 'matbench_v0.1_alignn': 0.9329780645736975, 'matbench_v0.1_automatminer_expressv2020': 0.01291754489989797, 'matbench_v0.1_modnet_v0.1.10': 0.0474188731...` |




#### `matbench_mp_gap`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.1770| 0.4025| 2.4955| 6.1745 |
 | fold_1 | 0.1774| 0.4018| 2.5452| 6.3716 |
 | fold_2 | 0.1802| 0.4059| 4.1836| 5.5312 |
 | fold_3 | 0.1756| 0.4091| 5.2175| 6.0348 |
 | fold_4 | 0.1803| 0.4188| 4.8511| 5.2131 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.1781 | 0.1803 | 0.1756 | 0.0018 |
| rmse | 0.4076 | 0.4188 | 0.4018 | 0.0062 |
| mape* | 3.8586 | 5.2175 | 2.4955 | 1.1420 |
| max_error | 5.8650 | 6.3716 | 5.2131 | 0.4284 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.03134890898326961, 'matbench_v0.1_alignn': 0.7111209827754947, 'matbench_v0.1_automatminer_expressv2020': 0.005786178299136875, 'matbench_v0.1_modnet_v0.1.10': 0.2517439299...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.0407591733831172, 'matbench_v0.1_alignn': 0.6975505799075838, 'matbench_v0.1_automatminer_expressv2020': 0.003201954717881077, 'matbench_v0.1_modnet_v0.1.10': 0.25848829199...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.036284616969791905, 'matbench_v0.1_alignn': 0.6942018172396998, 'matbench_v0.1_automatminer_expressv2020': 0.00041732299008234003, 'matbench_v0.1_modnet_v0.1.10': 0.2690962...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.03522104460336443, 'matbench_v0.1_alignn': 0.8009824659470643, 'matbench_v0.1_automatminer_expressv2020': 0.002089889799254658, 'matbench_v0.1_modnet_v0.1.10': 0.1617065996...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.04105720156963323, 'matbench_v0.1_alignn': 0.7549700155809074, 'matbench_v0.1_automatminer_expressv2020': 0.0048447390836097535, 'matbench_v0.1_modnet_v0.1.10': 0.199128043...` |




#### `matbench_mp_is_metal`

###### Fold scores

| fold | accuracy | balanced_accuracy | f1 | rocauc |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.9173| 0.9156| 0.9047| 0.9156 |
 | fold_1 | 0.9135| 0.9117| 0.9003| 0.9117 |
 | fold_2 | 0.9146| 0.9125| 0.9013| 0.9125 |
 | fold_3 | 0.9146| 0.9108| 0.8998| 0.9108 |
 | fold_4 | 0.9147| 0.9123| 0.9012| 0.9123 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| accuracy | 0.9149 | 0.9173 | 0.9135 | 0.0013 |
| balanced_accuracy | 0.9126 | 0.9156 | 0.9108 | 0.0016 |
| f1 | 0.9015 | 0.9047 | 0.8998 | 0.0017 |
| rocauc | 0.9126 | 0.9156 | 0.9108 | 0.0016 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.9953164044264534, 'matbench_v0.1_automatminer_expressv2020': 0.003963882720028548, 'matbench_v0.1_modnet_v0.1.10': 0.0007197128535180265, 'targ...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.93404698679432, 'matbench_v0.1_automatminer_expressv2020': 0.06591254576545874, 'matbench_v0.1_modnet_v0.1.10': 4.0467440221240175e-05, 'target...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.935298137056003, 'matbench_v0.1_automatminer_expressv2020': 0.06459068443951696, 'matbench_v0.1_modnet_v0.1.10': 0.00011117850448007413, 'targe...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 3.765834317927802e-05, 'matbench_v0.1_automatminer_expressv2020': 0.9998516565467143, 'matbench_v0.1_modnet_v0.1.10': 0.00011068511010648864, 'ta...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.0, 'matbench_v0.1_alignn': 0.9606082727476839, 'matbench_v0.1_automatminer_expressv2020': 0.03919544417457493, 'matbench_v0.1_modnet_v0.1.10': 0.00019628307774114157, 'targ...` |




#### `matbench_perovskites`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0300| 0.0583| 0.0307| 0.8302 |
 | fold_1 | 0.0332| 0.0644| 0.0338| 0.9146 |
 | fold_2 | 0.0295| 0.0519| 0.0296| 0.8127 |
 | fold_3 | 0.0302| 0.0545| 0.0298| 0.7940 |
 | fold_4 | 0.0305| 0.0569| 0.0283| 0.8359 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0307 | 0.0332 | 0.0295 | 0.0013 |
| rmse | 0.0572 | 0.0644 | 0.0519 | 0.0042 |
| mape* | 0.0305 | 0.0338 | 0.0283 | 0.0018 |
| max_error | 0.8375 | 0.9146 | 0.7940 | 0.0412 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.009547584180147844, 'matbench_v0.1_alignn': 0.9848694217426553, 'matbench_v0.1_automatminer_expressv2020': 0.0016440523111006303, 'matbench_v0.1_modnet_v0.1.10': 0.00393894...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.01535995631615898, 'matbench_v0.1_alignn': 0.9490765455180638, 'matbench_v0.1_automatminer_expressv2020': 0.02139321931280439, 'matbench_v0.1_modnet_v0.1.10': 0.01417027885...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.004227415890322362, 'matbench_v0.1_alignn': 0.9472138966649386, 'matbench_v0.1_automatminer_expressv2020': 0.027487021706203058, 'matbench_v0.1_modnet_v0.1.10': 0.021071665...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.0011844250315664847, 'matbench_v0.1_alignn': 0.9684742126005914, 'matbench_v0.1_automatminer_expressv2020': 0.029884743936693152, 'matbench_v0.1_modnet_v0.1.10': 0.00045661...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.005623378454120186, 'matbench_v0.1_alignn': 0.9059313272448253, 'matbench_v0.1_automatminer_expressv2020': 0.011448435884939327, 'matbench_v0.1_modnet_v0.1.10': 0.076996858...` |




#### `matbench_phonons`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 31.6557| 65.3053| 0.0564| 629.1442 |
 | fold_1 | 26.9097| 45.6052| 0.0542| 353.3826 |
 | fold_2 | 28.6332| 51.7256| 0.0536| 294.6454 |
 | fold_3 | 28.1886| 61.4775| 0.0549| 513.0511 |
 | fold_4 | 23.9047| 44.1742| 0.0447| 449.6660 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 27.8584 | 31.6557 | 23.9047 | 2.5164 |
| rmse | 53.6576 | 65.3053 | 44.1742 | 8.4300 |
| mape* | 0.0527 | 0.0564 | 0.0447 | 0.0041 |
| max_error | 447.9778 | 629.1442 | 294.6454 | 117.9133 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.0018203153633914477, 'matbench_v0.1_alignn': 0.6486914675578309, 'matbench_v0.1_automatminer_expressv2020': 0.08593035173170938, 'matbench_v0.1_modnet_v0.1.10': 0.263557865...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 5.294311262819687e-05, 'matbench_v0.1_alignn': 0.7044278252813406, 'matbench_v0.1_automatminer_expressv2020': 0.11910972769429452, 'matbench_v0.1_modnet_v0.1.10': 0.176409503...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.003740616371621964, 'matbench_v0.1_alignn': 0.7214054796467301, 'matbench_v0.1_automatminer_expressv2020': 0.008481957920670979, 'matbench_v0.1_modnet_v0.1.10': 0.266371946...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.08617214017244104, 'matbench_v0.1_alignn': 0.7045203684732354, 'matbench_v0.1_automatminer_expressv2020': 0.0006473946247970298, 'matbench_v0.1_modnet_v0.1.10': 0.208660096...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.0061383217259627495, 'matbench_v0.1_alignn': 0.6551412667140507, 'matbench_v0.1_automatminer_expressv2020': 0.053142546033970374, 'matbench_v0.1_modnet_v0.1.10': 0.28557786...` |




#### `matbench_steels`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 100.9349| 168.5655| 0.0653| 846.0036 |
 | fold_1 | 70.6172| 96.7591| 0.0512| 382.8586 |
 | fold_2 | 80.5541| 119.5353| 0.0581| 419.7060 |
 | fold_3 | 82.7723| 130.3167| 0.0616| 653.9549 |
 | fold_4 | 82.6796| 125.2501| 0.0627| 382.7175 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 83.5116 | 100.9349 | 70.6172 | 9.7961 |
| rmse | 128.0854 | 168.5655 | 96.7591 | 23.2641 |
| mape* | 0.0598 | 0.0653 | 0.0512 | 0.0049 |
| max_error | 537.0481 | 846.0036 | 382.7175 | 184.6522 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{'matbench_v0.1_CrabNet': 0.39234828151308304, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.41596749600021377, 'matbench_v0.1_modnet_v0.1.10': 0.1916842224867032, 'target'...` |
| fold_1 | `{'matbench_v0.1_CrabNet': 0.3889308341485257, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.2748090726773708, 'matbench_v0.1_modnet_v0.1.10': 0.3362600931741035, 'target': ...` |
| fold_2 | `{'matbench_v0.1_CrabNet': 0.026986533299291782, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.7075583926926007, 'matbench_v0.1_modnet_v0.1.10': 0.26545507400810747, 'target...` |
| fold_3 | `{'matbench_v0.1_CrabNet': 0.11192047688071322, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 0.22618555757912648, 'matbench_v0.1_modnet_v0.1.10': 0.6618939655401603, 'target'...` |
| fold_4 | `{'matbench_v0.1_CrabNet': 0.6529073222418661, 'matbench_v0.1_alignn': 0.0, 'matbench_v0.1_automatminer_expressv2020': 8.321664685660583e-05, 'matbench_v0.1_modnet_v0.1.10': 0.34700946111127734, 'targe...` |




