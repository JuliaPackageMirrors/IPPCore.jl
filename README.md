# IPPCore.jl

A Julia package that provides core library service to all packages that rely on Intel Performance Primitives Library (IPP).

-------------

## Usage

This package provides a few functions for retrieving version information and loading libraries:

```julia
IPPCore.version()         # returns the version information (of type IPPVersion)

IPPCore.loadlib(name)     # load a IPP library, 
```

For ``IPPCore.loadlib``, the input argument is the library name (*e.g.*, ``libippi``, ``libipps``, etc). Please refer to the [table here](https://software.intel.com/en-us/articles/selecting-the-intel-integrated-performance-primitives-intel-ipp-libraries-needed-by-your) to choose a proper library for your codes.

