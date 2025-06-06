# findrops

A low-level utility to detect active Raster Operations Pipelines (ROPs) on NVIDIA GPUs using direct `ioctl` calls. With the RTX 5090 release, some GPUs were missing ROPs.
No CUDA or NVML dependencies required.

---

## 🔧 How to Build

Download the source code: 

`wget https://raw.githubusercontent.com/low-pe/find-rops/main/findrops.cpp`

Compile it using g++: 

`g++ -o findrops findrops.cpp`

Run the tool (you may need sudo for access to /dev/nvidia*): 

`./findrops`

Easy one-liner to do all the steps:
`wget -q https://raw.githubusercontent.com/low-pe/find-rops/main/findrops.cpp && g++ -o findrops findrops.cpp && ./findrops`
