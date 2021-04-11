# CUDA-memory-transfer-issues
Issues and mentioned solutions in the "CUDA streams best practices and common pitfalls presentation"

Symptoms

— Memory copies do not overlap

— Host spends excessive time in memory copy API

— Cuda reports “Pageable” memory (Cuda 5.5+)

Solutions

— Use asynchronous memory copies

— Use pinned memory for host memory: cudaMallocHost or cudaHostRegister
