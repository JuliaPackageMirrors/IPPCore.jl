# IPPCore.jl

A Julia package that provides core library service to all packages that rely on Intel Performance Primitives Library (IPP).

-------------

## Usage

This package provides a few functions for retrieving version information and loading libraries:

```julia
using IPPCore

ippversion()            # returns the version information (of type IppVersion)

ippstatus_string(s)     # get the message string for a status code

ippcputype()            # get an integer code that indicates the CPU type

ippcpudescr(i)          # get the CPU description given an integer code
ippcpudescr()           # get the CPU description (for the CPU of the host)

ippcpufreq()            # estimate the CPU frequence (in MHz). 
                        # The estimated value may depend on the CPU workload.
```

For ``IPPCore.loadlib``, the input argument is the library name (*e.g.*, ``libippi``, ``libipps``, etc). Please refer to the [table here](https://software.intel.com/en-us/articles/selecting-the-intel-integrated-performance-primitives-intel-ipp-libraries-needed-by-your) to choose a proper library for your codes.

