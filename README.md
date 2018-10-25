<!--   Distributed under the Boost Software License, Version 1.0. (See accompanying -->
<!--   file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt)        -->

# hpxMP: An OpenMP runtime implemented using HPX

hpxMP is a portabl, scalable and flexible application programming interface using OpenMP specification 
that supports multi-platform shared memory multiprocessing programming in C/ C++.

A recorded video introduction of hpxMP can be found
 [here](https://www.youtube.com/watch?v=ajDGWPDrcxU&index=12&list=PL7vEgTL3FalbVFwzkXLHpBRKlcJNULW1g).

The [CircleCI](https://circleci.com/gh/STEllAR-GROUP/hpxMP) contiguous
integration service tracks the current build status for the master branch:
[![CircleCI](https://circleci.com/gh/STEllAR-GROUP/hpxMP.svg?style=svg)](https://circleci.com/gh/STEllAR-GROUP/hpxMP).

# Code summary

The intel and gcc openMP runtime calls are implemented in intel_hpxMP.cpp/ gcc_hpxMP.cpp.
The OMPT support is implemented in ompt_hpx_general.cpp
The bulk of the work is donein hpx_runtime.cpp.
All of the structs/classes of interest are defined in hpx_runtime.h.

Tests are under folder tests/, which are performing automatic tests fot this program. 
Some of the tests are adapted from examples under folder examples/omp/tests/src which were written by Jeremy Kemp.

This is a different hpx_runtime than the one defined in the hpx implementation, and will eventually
need to be replaced.

# Installation

Please refer to [Install Instruction](doc/install.md) for detailed instruction on how to install hpxMP.

# Usecases

Please refer to [Use Examples](doc/usecases.md) for simple use examples.

# DONEs and TODOs

Please refer to [dones and todos](doc/done-todo.md) for information about
what has been implemented in hpxMP and what needs to be done.

# Feature

Please refer to doc/feature

# Specification

Please refer to doc/specification


