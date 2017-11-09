# Kernel Tuner (Ben van Werkhoven)

[Kernel Tuner](https://github.com/benvanwerkhoven/kernel_tuner) simplifies the software development of optimized and auto-tuned GPU programs, by enabling Python-based unit testing of GPU code and making it easy to develop scripts for auto-tuning GPU kernels. Kernel Tuner provides a comprehensive solution for auto-tuning GPU programs, supporting auto-tuning of user-defined parameters in both host and device code, supporting output verification of all benchmarked kernels during tuning, as well as many optimization strategies to speed up the tuning process.

## Things that we will work on:

- Simplify installation procedure by using the 'extras' feature, such that optional dependencies such as PyCuda and PyOpenCL can be installed along with Kernel Tuner. The installation guide and readme will be updated accordingly.

- Improve user-friendliness by doing more checks on the inputs, in particular the tunable parameters and kernel arguments

- Reorganize the test suite of Kernel Tuner to match the file structure of the source code, the two have diverged a bit over time. Also we may look at ways to use the examples as integration tests and automate their execution.
We will also fully migrate the tests from nosetests to pytest and use more pytest features.

- Several piecies of the documentation can be expanded into full tutorials and should be converted into jupyter notebooks, this includes the [matrix multiply tutorial](http://benvanwerkhoven.github.io/kernel_tuner/matrix.html) the [output verification tutorial](http://benvanwerkhoven.github.io/kernel_tuner/correctness.html) and the [tuning host code tutorial](http://benvanwerkhoven.github.io/kernel_tuner/hostcode.html).

- Several smaller changes that expand the functionality of the tuner, see the [Kernel Tuner's roadmap](https://github.com/benvanwerkhoven/kernel_tuner/blob/master/roadmap.md)

There are also a couple of larger things to work on, but I doubt we will get to that in this sprint.
