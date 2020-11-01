# CUDA-labs
CUDA, python3, PyCUDA, matrix multiplication
- In this program matrix multiplication had been developed by using python3, CUDA, PyCUDA in a free version of Google Collab
- The PyCUDA's main feature allows to build kernel on C++, then running one on GPU
- One of the fastest way to multiply matrix is to use numpy.dot(), because its realization builded on C
- In this work I've compared a time running of two ways on gpu with numpy.dot() and with C++ kernel in PyCUDA on the different matrix sizes
- Mean results
  |  N  | CPU time, ms | GPU time, ms | Speedup|
  |:---:|:------------:|:------------:|:------:|
  | 128 |        0.122 |        0.422 |    0.29|
  | 256 |        0.613 |        0.615 |    1.00|
  | 512 |        4.498 |        2.164 |    2.08|
  |1024 |       33.361 |        9.894 |    3.37|
  |2048 |      258.712 |       62.114 |    4.17|
- Conclusion:
  - As we can see, on the tiny matrix sizes CPU calculate better than GPU in several times, but, with the matrix size growing, GPU shows significant increasing, in compare with CPU. This means the most reasonable use of the GPU, instead of CPU, for multiplying high-sizes matrix.
