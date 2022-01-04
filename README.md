# Ceres-Solver-Examples


## Environment
|OS|Language|
|:---:|:---:|
|Ubuntu 18.04.6 LTS|C++|  

## 1. Ceres-Solver Installation, CMake, HelloWorld Example
[1. Presentation PDF](https://github.com/Lee-JaeWon/Ceres-Solver-Examples/blob/main/ceres/ceres-solver/helloworld_example/1229.pdf)[ or GitBlog](https://lee-jaewon.github.io/ceres_solver/ceres-solver(1)/)
<br>
[2. Source Code](https://github.com/Lee-JaeWon/Ceres-Solver-Examples/tree/main/ceres/ceres-solver/helloworld_example)

## How to install Ceres Solver
Ubuntu 명령어
```
git clone https://ceres-solver.googlesource.com/ceres-solver

# CMake
sudo apt-get install cmake
# google-glog + gflags
sudo apt-get install libgoogle-glog-dev libgflags-dev
# BLAS & LAPACK
sudo apt-get install libatlas-base-dev
# Eigen3
sudo apt-get install libeigen3-dev
# SuiteSparse and CXSparse (optional)
sudo apt-get install libsuitesparse-dev

mkdir ceres-bin
cd ceres-bin
cmake ../ceres-solver-2.0.0
make -j3
make test
# Optionally install Ceres, it can also be exported using CMake which
# allows Ceres to be used without requiring installation, see the documentation
# for the EXPORT_BUILD_DIR option for more information.
sudo make install
```
ceres-bin 폴더와 ceres-solver폴더가 동일폴더에 존재해야한다.


