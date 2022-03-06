# Leaderboard

## Leaderboard: General Purpose Algorithms on `matbench_v0.1`

Find more information about this benchmark on [the benchmark info page](Benchmark%20Info/matbench_v0.1.md)

| Task name | Samples | Algorithm | Verified MAE (unit) or ROCAUC | Notes |
|------------------|---------|-----------|----------------------|-------|
| [matbench_steels](Leaderboards%20Per-Task/matbench_v0.1_matbench_steels.md) | 312 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **53.3729 (MPa)** |  |
| [matbench_jdft2d](Leaderboards%20Per-Task/matbench_v0.1_matbench_jdft2d.md) | 636 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **21.9636 (meV/atom)** |  |
| [matbench_phonons](Leaderboards%20Per-Task/matbench_v0.1_matbench_phonons.md) | 1,265 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **13.6984 (cm^-1)** |  |
| [matbench_expt_gap](Leaderboards%20Per-Task/matbench_v0.1_matbench_expt_gap.md) | 4,604 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.1001 (eV)** |  |
| [matbench_dielectric](Leaderboards%20Per-Task/matbench_v0.1_matbench_dielectric.md) | 4,764 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.1981 (unitless)** |  |
| [matbench_expt_is_metal](Leaderboards%20Per-Task/matbench_v0.1_matbench_expt_is_metal.md) | 4,921 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.9937** |  |
| [matbench_glass](Leaderboards%20Per-Task/matbench_v0.1_matbench_glass.md) | 5,680 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.9690** |  |
| [matbench_log_gvrh](Leaderboards%20Per-Task/matbench_v0.1_matbench_log_gvrh.md) | 10,987 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.0393 (log10(GPa))** |  |
| [matbench_log_kvrh](Leaderboards%20Per-Task/matbench_v0.1_matbench_log_kvrh.md) | 10,987 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.0302 (log10(GPa))** |  |
| [matbench_perovskites](Leaderboards%20Per-Task/matbench_v0.1_matbench_perovskites.md) | 18,928 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.0218 (eV/unit cell)** |  |
| [matbench_mp_gap](Leaderboards%20Per-Task/matbench_v0.1_matbench_mp_gap.md) | 106,113 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.0787 (eV)** |  |
| [matbench_mp_is_metal](Leaderboards%20Per-Task/matbench_v0.1_matbench_mp_is_metal.md) | 106,113 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.9627** |  |
| [matbench_mp_e_form](Leaderboards%20Per-Task/matbench_v0.1_matbench_mp_e_form.md) | 132,752 | [fictitious_compound](Full%20Benchmark%20Data/matbench_v0.1_fictitious_compound_wise.md) | **0.0135 (eV/atom)** |  |



<iframe src="static/scaled_errors.html" class="is-fullwidth" height="700px" width="1000px" frameBorder="0"> </iframe>

Scaled errors for regressions on this leaderboard plot are assessed as the ratio of mean absolute error to mean absolute deviation:

$$
\text{Scaled Error} = \frac{\text{MAE}}{\text{MAD}} = \frac{\sum_i^N | y_i - y_i^{pred} |}{\sum_i^N | y_i - \bar{y} | }
$$


## Overview

[Matbench](https://doi.org/10.1038/s41524-020-00406-3) is an [ImageNet](http://www.image-net.org) for **materials science**; a
**curated set of 13 supervised, pre-cleaned, ready-to-use ML tasks** for benchmarking and fair comparison. The tasks span a wide domain of
inorganic materials science applications including electronic, thermodynamic, mechanical, and thermal properties among crystals, 2D materials,
disordered metals, and more.  

**The [Matbench python package](https://github.com/hackingmaterials/matbench) provides everything needed to use Matbench with your ML algorithm in ~10 lines of code or less.**

![infographic](static/infographic_matbench.png)


## What can Matbench offer?

### This website


- **Leaderboard of results for state-of-the-art materials ML algorithms on standardized test problems**
- Interactively explore and download the tasks on [MPContribs-ML](https://ml.materialsproject.org/browse), a platform hosted by [The Materials Project](https://materialsproject.org). See [Benchmark Info](Benchmark%20Info/matbench_v0.1/) for links to each dataset.
- **Each and every result is backed by a peer-reviewed publication and a jupyter notebook** (similar to Papers With Code) - i.e., how were these results were obtained?
- Glossary of all algorithms' results on the Matbench problems


### The Matbench Python package

- Probe ML algorithms strengths and weaknesses across a wide range of materials property prediction tasks
- Run a full benchmark in ~10 lines of code
- Submit results as a PR to the [Matbench repo](https://github.com/hackingmaterials/matbench) to compare with other algorithms and appear on the leaderboard
- Benchmark both **general purpose** ML models as well as algorithms specialized for particular domains


## Summary of Matbench's Tasks

Matbench's 13 tasks can be broken down into various categories; it includes both the small - less than 10,000 samples - datasets that characterize
experimental materials data as well as larger datasets from computer modelling methods like density functional theory (DFT).


![breakdown](static/datasets_breakdown_inverted.png)


Each task in Matbench consists of a three things:

1. **A set of inputs:** crystal structures or chemical compositions.
2. **A set of outputs:** target properties, such as formation energy.
3. **A test procedure:** a way to get a score for your algorithm


The Matbench Python package provides functions for getting the first two (packaged together for each task as a _dataset_) as well as running 
the test procedure. See the [How to use](How%20To%20Use/) documentation page to get started.



## Citing Matbench

You can find details and results on the benchmark in our paper [Benchmarking materials property prediction methods: the Matbench test set and Automatminer reference algorithm](https://doi.org/10.1038/s41524-020-00406-3). 
Please consider citing this paper if you use Matbench v0.1 for benchmarking, comparison, or prototyping.


You can cite Matbench using this reference:

```
Dunn, A., Wang, Q., Ganose, A., Dopp, D., Jain, A. 
Benchmarking Materials Property Prediction Methods: 
The Matbench Test Set and Automatminer Reference Algorithm. 
npj Computational Materials 6, 138 (2020). 
https://doi.org/10.1038/s41524-020-00406-3
```