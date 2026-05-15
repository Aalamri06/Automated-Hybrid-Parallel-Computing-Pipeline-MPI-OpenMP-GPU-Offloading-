%%writefile README.md
# Automated Hybrid Parallel Computing Pipeline (MPI + OpenMP + GPU Offloading)

## 📌 Project Overview
This repository contains a high-performance, enterprise-grade hybrid parallel system combining distributed memory architecture (**MPI**) with shared memory parallelism (**OpenMP**) and dedicated hardware accelerator offloading (**NVIDIA CUDA/PTX via OpenMP Target**). 

The application configures an exactly balanced **11-process cluster topology** designed to execute distinct computational operations concurrently. It handles arithmetic calculations, multi-threaded string analytics reduction, safe non-blocking stream file I/O operations, complex 2D matrix data scatter/gather transformations, and explicit GPU kernel acceleration.

---

## 🏗️ System Topology & Node Mapping
The program splits processing tasks cleanly among 11 distinct MPI Ranks across three specialized computing paradigms:
