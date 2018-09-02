Tensorflow v1.10.1 - CUDA 9.1 - cuDNN 7.1
=================

* Compiled from source to **only** support GPU usage
* No CPU / ATX\* support is enabled:
  * This is needed to get around [errors in TF](https://github.com/tensorflow/tensorflow/issues/19584) when using older CPUs, or
  * When GPU support is the only mode desired.

## Installation

`pip install tensorflow-1.10.1-cp36-cp36m-linux_x86_64.whl`

## Component Versions

| Component | Version |
| :-------------: | :-------------: |
| Distro   | `Ubuntu 18.04.1`   |
| Kernel   |  `4.18.5 x86_64`   |
| GPU / Compute Capcity     |  `Nvidia GeForce GTX 1080 TI` - `6.1`  |
| Tensorflow   |  `v1.10.1`   |
| CUDA   |  `9.1.85_387.26`   |
| cuDNN   |  `7.1.3`   |
| NCCL   |  `2.2.13`   |
| GCC   |  `Ubuntu 6.4.0-17ubuntu1`   |
| Python   |  `3.6.5`   |
| Bazel   |  `0.15.0`   |
| Tested against NVIDIA Driver Runtime   |  `390.87`   |

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

export TF_CUDA_VERSION="9.1.85_387.26"
export TF_CUDNN_VERSION="7.1.3"
export TF_NEED_CUDA=1
export TF_NEED_TENSORRT=0
export TF_NCCL_VERSION=2.2
```
