# A Scalable Test Problem Generator for Sequential Transfer Optimization

## A Benchmark Suite of Sequential Transfer Optimization Problems (STOPs)

This repository provides the MATLAB implementation of generating a benchmark suite of sequential transfer optimization problems (STOPs). To instantiate an STOP, we need to set up the following six parameters: the target family, the transfer scenario, the optimum optimum, the similarity distribution, the task dimension, and the number of source tasks. Their available realizations are as follows:

* Task families (F): `Sphere`, `Ellipsoid`, `Schwefel`, `Quartic`, `Ackley`, `Rastrigin`, `Griewank`, and `Levy`.
* Transfer scenarios (T): `Ta` and `Te`.
* Optimum coverages (xi): 0, 0.7, 1.
* Similarity distributions (p): `c`, `u`, `i`, `d`.
* Task dimensions (d): positive integers.
* Numbers of source tasks (k): positive integers.

In this work, we name an STOP as F-T-xi-p-d-k, where F denotes the target family, T represents the transfer scenario, xi is the optimum coverage, p represents the similarity distribution, d denotes the task dimension, k is the number of source tasks. According to this naming rule, we specify the following 12 STOPs to form the benchmark suite,


|Problem ID|Problem Specification|
|:-|:-|
|STOP 1|Sphere-Ta-xi0-pc-50-k|
|STOP 2|Ellipsoid-Te-xi0-pu-25-k|
|STOP 3|Schwefel-Ta-xi0-pi-30-k|
|STOP 4|Quartic-Te-xi0-pd-50-k|
|STOP 5|Ackley-Ta-xi1-pi-25-k|
|STOP 6|Rastrigin-Te-xi1-pu-50-k|
|STOP 7|Griewank-Ta-xi0.7-pi-25-k|
|STOP 8|Levy-Te-xi1-pd-30-k|
|STOP 9|Sphere-Ta-xi1-pc-25-k|
|STOP 10|Rastrigin-Te-xi0.7-pc-30-k|
|STOP 11|Ackley-Ta-xi0.7-pc-50-k|
|STOP 12|Ellipsoid-Te-xi1-pc-50-k|

In this repository, we employ evolutionary algorithm (EA) to denmonstrate the generation process of the 12 STOPs, whose scripts can be found at [STOP-EA](https://github.com/XmingHsueh/STOP/blob/main/main_generation_ea.m).

## Citation

If you find this repo useful for your research, please consider to cite:
```latex
@article{xue2023scalable,
  title={A Scalable Test Problem Generator for Sequential Transfer Optimization},
  author={Xue, Xiaoming and Yang, Cuie and Feng, Liang and Zhang, Kai and Song, Linqi and Tan, Kay Chen},
  journal={arXiv preprint arXiv:2304.08503},
  year={2023}
}
```

## Acknowledgments

...
