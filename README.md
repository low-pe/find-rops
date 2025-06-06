# findrops

A low-level utility to detect active Raster Operations Pipelines (ROPs) on NVIDIA GPUs using direct `ioctl` calls. With the RTX 5090 release, some GPUs were missing ROPs.
No CUDA or NVML dependencies required.

---

## 🔧 How to Build

Download the source code: 

`wget https://raw.githubusercontent.com/yourusername/findrops/main/findrops.cpp`

Compile it using g++: 

`g++ -o findrops findrops.cpp`

Run the tool (you may need sudo for access to /dev/nvidia*): 

`./findrops`
