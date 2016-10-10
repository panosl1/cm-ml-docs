# Installing the Machine Learning RPMs


As of Bright Cluster Manager 7.3 a number of Machine/Deep Learning librariy and framework RPM packages have been included.  Bright makes it faster and easier for organizations to gain actionable insights from rich, complex data using the latest, state-of-the-art libraries with minimal effort during installation.

Currently the following RPMs are available:

Package name | Description
------------ | -------------
cm-ml-distdeps | Meta-package containing library dependencies available from the base Linux distribution repositories as well as the EPEL repository
cm-ml-pythondeps | Pre-packaged Python dependencies for Bright's RPM packages
caffe | A deep learning framework made with expression, speed, and modularity in mind.
torch7 | A library in C++ for developing Open Source speech and machine learning applications. 
theano | Theano is a Python library that allows you to define, optimize, and evaluate mathematical expressions involving multi-dimensional arrays efficiently. 
tensorflow | TensorFlow is an Open Source Software Library for Machine Intelligence
cudnn | A GPU-accelerated library of primitives for deep neural networks.
cub |  Reusable software components for CUDA
nccl | (pronounced "Nickel") A stand-alone library of standard collective communication routines, such as all-gather, reduce, broadcast, etc., that have been optimized to achieve high bandwidth over PCIe. 
mlpython | MLPython is a library for organizing machine learning research.

The following package will be added in the future:

Package name | Description
------------ | -------------
caffeonspark | CaffeOnSpark brings deep learning to Hadoop and Spark clusters. By combining salient features from deep learning framework Caffe and big-data frameworks Apache Spark and Apache Hadoop, CaffeOnSpark enables distributed deep learning on a cluster of GPU and CPU servers.
cntk | The Computational Network Toolkit by Microsoft Research, is a unified deep-learning toolkit 
bidmach | BIDMach is a very fast machine learning library.

## Requirements

The folowing requirements must be met before installing the Machine Learning packages

* RHEL, Centos or Scientic Linux 7.x
* Access to the Linux distribution's online YUM repositories as well the EPEL repository
* 2 GB of free space for the RPMs that are installed on the headnode and an additional 400 MB for each software image that will be used for running Machine Laraning pipelines
* (Recommended) Maxwell or more recent NVIDIA GPUs with compute capability 3.5 or later

## Installation

### For the compute nodes

The only RPM that needs to be installed on the headnode is cm-ml-distdeps. This is is a meta-package the instructs YUM to install the necessary system libraries as well as the development packages e.g. blas-devel.





