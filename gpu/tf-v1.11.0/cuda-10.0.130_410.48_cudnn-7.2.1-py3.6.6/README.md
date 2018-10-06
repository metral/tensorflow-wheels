Tensorflow v1.11.0 | NVIDIA-410.57 | CUDA-10.0.130 | cuDNN-7.3.0
=================

* Compiled from source to **only** support GPU usage
* No CPU / ATX\* support is enabled:
  * This is needed to get around [errors in TF](https://github.com/tensorflow/tensorflow/issues/19584) when using older CPUs, or
  * When GPU support is the only mode desired.

## Installation

1. [Download Wheel - 101M](https://drive.google.com/uc?id=1Onh5CROEDfxLFdq6tQCX1ctLLVFyF_I6&export=download)
(hosted on gdrive due to 100GB github file size limit)
md5: d230909e99920924e4b41e5138f0efd4

2. `pip install tensorflow-1.11.0-cp36-cp36m-linux_x86_64.whl`

## Component Versions

| Component | Version |
| :-------------: | :-------------: |
| Distro   | `Ubuntu 18.04.1`   |
| Kernel   |  `4.18.5 x86_64`   |
| GPU / Compute Capcity     |  `Nvidia GeForce GTX 1080 TI` - `6.1`  |
| Tensorflow   |  `v1.11.0`   |
| NVIDIA   |  `410.57`   |
| CUDA   |  `10.0.130_410.48`   |
| cuDNN   |  `7.3.0.29`   |
| NCCL   |  `2.3.5`   |
| GCC   |  `Ubuntu 6.4.0-17ubuntu1`   |
| Python   |  `3.6.6`   |
| Bazel   |  `0.16.1`   |
| Tested against NVIDIA Driver Runtime   |  `410.57`   |

## Bazel Compilation Parameters

```
export TF_NEED_CUDA=0
export TF_NEED_GCP=1
export TF_CUDA_COMPUTE_CAPABILITIES=6.1
export TF_NEED_HDFS=1
export TF_NEED_OPENCL=0
export TF_NEED_JEMALLOC=1
export TF_ENABLE_XLA=0
export TF_NEED_VERBS=0
export TF_CUDA_CLANG=0
export TF_DOWNLOAD_CLANG=0
export TF_NEED_MKL=0
export TF_DOWNLOAD_MKL=0
export TF_NEED_MPI=0
export TF_NEED_S3=1
export TF_NEED_KAFKA=1
export TF_NEED_GDR=0
export TF_NEED_OPENCL_SYCL=0
export TF_SET_ANDROID_WORKSPACE=0
export TF_NEED_AWS=0
export TF_NEED_NGRAPH=0

export TF_CUDA_VERSION="10.0.130_410.48"
export TF_CUDNN_VERSION="7.2.1"
export TF_NEED_CUDA=1
export TF_NEED_TENSORRT=0
export TF_NCCL_VERSION=2.3
```

## Environment Packages
```
$ conda list -n base

# packages in environment at /conda:
#
# Name                    Version                   Build  Channel
asn1crypto                0.24.0                py36_1003    conda-forge
bazel                     0.16.1                        0    conda-forge
blas                      1.1                    openblas    conda-forge
bzip2                     1.0.6                h470a237_2    conda-forge
ca-certificates           2018.8.24            ha4d7672_0    conda-forge
certifi                   2018.8.24             py36_1001    conda-forge
cffi                      1.11.5           py36h5e8e0c9_1    conda-forge
chardet                   3.0.4                 py36_1003    conda-forge
conda                     4.5.11                   py36_0    conda-forge
conda-env                 2.6.0                         1
cryptography              2.3.1            py36hdffb7b8_0    conda-forge
cryptography-vectors      2.3.1                 py36_1000    conda-forge
h5py                      2.8.0                     <pip>
idna                      2.7                   py36_1002    conda-forge
Keras-Applications        1.0.6                     <pip>
Keras-Preprocessing       1.0.5                     <pip>
libedit                   3.1.20170329         h6b74fdf_2
libffi                    3.2.1                hd88cf55_4
libgcc-ng                 8.2.0                hdf63c60_1
libgfortran               3.0.0                         1    conda-forge
libstdcxx-ng              8.2.0                hdf63c60_1
ncurses                   6.1                  hf484d3e_0
numpy                     1.15.2          py36_blas_openblashd3ea46f_1  [blas_openblas]  conda-forge
openblas                  0.2.20                        8    conda-forge
openjdk                   8.0.152              h46b5887_1
openssl                   1.0.2p               h470a237_0    conda-forge
pip                       18.0                  py36_1001    conda-forge
pycosat                   0.6.3            py36h470a237_1    conda-forge
pycparser                 2.19                       py_0    conda-forge
pyopenssl                 18.0.0                   py36_0    conda-forge
pysocks                   1.6.8                 py36_1002    conda-forge
python                    3.6.6                h5001a0f_0    conda-forge
readline                  7.0                  h7b6447c_5
requests                  2.19.1                   py36_1    conda-forge
ruamel_yaml               0.15.71          py36h470a237_0    conda-forge
setuptools                40.4.3                   py36_0    conda-forge
six                       1.11.0                py36_1001    conda-forge
sqlite                    3.24.0               h84994c4_0
tk                        8.6.8                hbc83047_0
urllib3                   1.23                     py36_1    conda-forge
wheel                     0.32.1                   py36_0    conda-forge
xz                        5.2.4                h14c3975_4
yaml                      0.1.7                had09818_2
zlib                      1.2.11               ha838bed_2
```
