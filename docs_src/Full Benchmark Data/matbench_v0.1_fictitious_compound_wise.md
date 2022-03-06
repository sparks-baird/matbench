# matbench_v0.1: fictitious_compound

### Algorithm description: 

Fictitious compound ensemble where the best prediction from each of the models on a compound-wise basis was taken.

#### Notes:
No notes.

Raw data download and example notebook available [on the matbench repo](https://github.com/hackingmaterials/matbench/tree/main/benchmarks/matbench_v0.1_fictitious_compound_wise).

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
 | fold_0 | 0.0991| 0.5482| 0.0281| 13.6699 |
 | fold_1 | 0.1590| 0.9421| 0.0430| 19.2249 |
 | fold_2 | 0.3185| 2.8847| 0.0484| 58.7285 |
 | fold_3 | 0.2157| 2.1932| 0.0330| 51.3719 |
 | fold_4 | 0.1985| 1.5144| 0.0481| 27.8634 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.1981 | 0.3185 | 0.0991 | 0.0723 |
| rmse | 1.6165 | 2.8847 | 0.5482 | 0.8423 |
| mape* | 0.0401 | 0.0484 | 0.0281 | 0.0082 |
| max_error | 34.1717 | 58.7285 | 13.6699 | 17.7899 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_expt_gap`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0951| 0.2945| 0.1159| 4.5021 |
 | fold_1 | 0.1009| 0.3217| 0.1049| 6.3544 |
 | fold_2 | 0.1144| 0.4185| 0.1328| 7.8869 |
 | fold_3 | 0.0926| 0.2750| 0.1130| 4.2857 |
 | fold_4 | 0.0977| 0.3129| 0.1525| 3.9071 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.1001 | 0.1144 | 0.0926 | 0.0076 |
| rmse | 0.3245 | 0.4185 | 0.2750 | 0.0497 |
| mape* | 0.1238 | 0.1525 | 0.1049 | 0.0170 |
| max_error | 5.3872 | 7.8869 | 3.9071 | 1.5081 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_expt_is_metal`

###### Fold scores

| fold | accuracy | balanced_accuracy | f1 | rocauc |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.9919| 0.9919| 0.9918| 0.9919 |
 | fold_1 | 0.9929| 0.9929| 0.9928| 0.9929 |
 | fold_2 | 0.9970| 0.9969| 0.9969| 0.9969 |
 | fold_3 | 0.9929| 0.9929| 0.9928| 0.9929 |
 | fold_4 | 0.9939| 0.9939| 0.9939| 0.9939 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| accuracy | 0.9937 | 0.9970 | 0.9919 | 0.0017 |
| balanced_accuracy | 0.9937 | 0.9969 | 0.9919 | 0.0017 |
| f1 | 0.9937 | 0.9969 | 0.9918 | 0.0018 |
| rocauc | 0.9937 | 0.9969 | 0.9919 | 0.0017 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_glass`

###### Fold scores

| fold | accuracy | balanced_accuracy | f1 | rocauc |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.9798| 0.9758| 0.9857| 0.9758 |
 | fold_1 | 0.9868| 0.9799| 0.9908| 0.9799 |
 | fold_2 | 0.9762| 0.9680| 0.9833| 0.9680 |
 | fold_3 | 0.9771| 0.9623| 0.9841| 0.9623 |
 | fold_4 | 0.9762| 0.9590| 0.9835| 0.9590 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| accuracy | 0.9792 | 0.9868 | 0.9762 | 0.0040 |
| balanced_accuracy | 0.9690 | 0.9799 | 0.9590 | 0.0079 |
| f1 | 0.9855 | 0.9908 | 0.9833 | 0.0028 |
| rocauc | 0.9690 | 0.9799 | 0.9590 | 0.0079 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_jdft2d`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 12.9983| 26.1572| 18.6985| 121.9589 |
 | fold_1 | 16.9571| 49.9781| 0.1214| 364.1909 |
 | fold_2 | 38.9201| 136.4774| 0.4100| 845.7528 |
 | fold_3 | 14.0195| 38.0753| 0.1062| 275.8517 |
 | fold_4 | 26.9229| 145.8185| 0.3647| 1519.7424 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 21.9636 | 38.9201 | 12.9983 | 9.8048 |
| rmse | 79.3013 | 145.8185 | 26.1572 | 51.1417 |
| mape* | 3.9402 | 18.6985 | 0.1062 | 7.3802 |
| max_error | 625.4994 | 1519.7424 | 121.9589 | 508.3839 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_log_gvrh`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0381| 0.0721| 0.0313| 0.8695 |
 | fold_1 | 0.0402| 0.0770| 0.0328| 1.0887 |
 | fold_2 | 0.0386| 0.0769| 0.0326| 0.7799 |
 | fold_3 | 0.0396| 0.0755| 0.0317| 0.8718 |
 | fold_4 | 0.0401| 0.0771| 0.0320| 0.6013 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0393 | 0.0402 | 0.0381 | 0.0008 |
| rmse | 0.0757 | 0.0771 | 0.0721 | 0.0019 |
| mape* | 0.0321 | 0.0328 | 0.0313 | 0.0005 |
| max_error | 0.8422 | 1.0887 | 0.6013 | 0.1577 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_log_kvrh`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0290| 0.0749| 0.0199| 1.4823 |
 | fold_1 | 0.0312| 0.0830| 0.0212| 1.2273 |
 | fold_2 | 0.0280| 0.0691| 0.0193| 1.0919 |
 | fold_3 | 0.0334| 0.0846| 0.0255| 1.0491 |
 | fold_4 | 0.0293| 0.0750| 0.0200| 1.3125 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0302 | 0.0334 | 0.0280 | 0.0019 |
| rmse | 0.0773 | 0.0846 | 0.0691 | 0.0057 |
| mape* | 0.0212 | 0.0255 | 0.0193 | 0.0023 |
| max_error | 1.2326 | 1.4823 | 1.0491 | 0.1563 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_mp_e_form`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0133| 0.0429| 0.0961| 3.5487 |
 | fold_1 | 0.0139| 0.0393| 0.0839| 2.3544 |
 | fold_2 | 0.0133| 0.0346| 0.0833| 1.4278 |
 | fold_3 | 0.0138| 0.0373| 0.1080| 1.2195 |
 | fold_4 | 0.0132| 0.0347| 0.1057| 1.0446 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0135 | 0.0139 | 0.0132 | 0.0003 |
| rmse | 0.0378 | 0.0429 | 0.0346 | 0.0031 |
| mape* | 0.0954 | 0.1080 | 0.0833 | 0.0104 |
| max_error | 1.9190 | 3.5487 | 1.0446 | 0.9317 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_mp_gap`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0794| 0.2179| 0.9938| 4.9652 |
 | fold_1 | 0.0776| 0.2125| 1.1647| 4.9121 |
 | fold_2 | 0.0776| 0.2063| 2.5293| 4.1238 |
 | fold_3 | 0.0776| 0.2014| 2.9035| 4.9277 |
 | fold_4 | 0.0812| 0.2210| 2.2283| 4.0632 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0787 | 0.0812 | 0.0776 | 0.0014 |
| rmse | 0.2118 | 0.2210 | 0.2014 | 0.0072 |
| mape* | 1.9639 | 2.9035 | 0.9938 | 0.7553 |
| max_error | 4.5984 | 4.9652 | 4.0632 | 0.4131 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_mp_is_metal`

###### Fold scores

| fold | accuracy | balanced_accuracy | f1 | rocauc |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.9683| 0.9662| 0.9630| 0.9662 |
 | fold_1 | 0.9614| 0.9589| 0.9549| 0.9589 |
 | fold_2 | 0.9710| 0.9666| 0.9655| 0.9666 |
 | fold_3 | 0.9641| 0.9616| 0.9581| 0.9616 |
 | fold_4 | 0.9633| 0.9603| 0.9570| 0.9603 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| accuracy | 0.9656 | 0.9710 | 0.9614 | 0.0035 |
| balanced_accuracy | 0.9627 | 0.9666 | 0.9589 | 0.0031 |
| f1 | 0.9597 | 0.9655 | 0.9549 | 0.0039 |
| rocauc | 0.9627 | 0.9666 | 0.9589 | 0.0031 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_perovskites`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 0.0226| 0.0455| 0.0230| 0.7848 |
 | fold_1 | 0.0234| 0.0478| 0.0237| 0.7967 |
 | fold_2 | 0.0208| 0.0358| 0.0211| 0.6265 |
 | fold_3 | 0.0211| 0.0379| 0.0221| 0.5825 |
 | fold_4 | 0.0214| 0.0408| 0.0201| 0.7664 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 0.0218 | 0.0234 | 0.0208 | 0.0010 |
| rmse | 0.0416 | 0.0478 | 0.0358 | 0.0045 |
| mape* | 0.0220 | 0.0237 | 0.0201 | 0.0013 |
| max_error | 0.7114 | 0.7967 | 0.5825 | 0.0889 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_phonons`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 13.9451| 31.5923| 0.0250| 394.6285 |
 | fold_1 | 13.4878| 28.3736| 0.0260| 277.0146 |
 | fold_2 | 14.8111| 33.7098| 0.0261| 226.4931 |
 | fold_3 | 14.1058| 32.4059| 0.0273| 252.1160 |
 | fold_4 | 12.1421| 21.0252| 0.0241| 190.2821 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 13.6984 | 14.8111 | 12.1421 | 0.8867 |
| rmse | 29.4214 | 33.7098 | 21.0252 | 4.5520 |
| mape* | 0.0257 | 0.0273 | 0.0241 | 0.0011 |
| max_error | 268.1069 | 394.6285 | 190.2821 | 69.4711 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




#### `matbench_steels`

###### Fold scores

| fold | mae | rmse | mape* | max_error |
|------ |------ |------ |------ |------ |
 | fold_0 | 65.0725| 119.1001| 0.0403| 553.2987 |
 | fold_1 | 46.6963| 71.5273| 0.0348| 350.5612 |
 | fold_2 | 54.3692| 91.1689| 0.0365| 370.1786 |
 | fold_3 | 50.6138| 76.2675| 0.0362| 295.1635 |
 | fold_4 | 50.1129| 85.8563| 0.0391| 356.5724 |


###### Fold score stats

| metric | mean | max | min | std |
|--------|------|-----|-----|-----|
| mae | 53.3729 | 65.0725 | 46.6963 | 6.3355 |
| rmse | 88.7840 | 119.1001 | 71.5273 | 16.6600 |
| mape* | 0.0374 | 0.0403 | 0.0348 | 0.0020 |
| max_error | 385.1549 | 553.2987 | 295.1635 | 87.8735 |


###### Fold parameters

| fold | params dict|
|------|------------|
| fold_0 | `{}` |
| fold_1 | `{}` |
| fold_2 | `{}` |
| fold_3 | `{}` |
| fold_4 | `{}` |




