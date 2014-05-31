# IPPCore.jl

A Julia package that provides core library service to all packages that rely on Intel Performance Primitives Library (IPP).

-------------

## Usage

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
