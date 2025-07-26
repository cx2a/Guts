
[How GPU Computing Works](https://www.nvidia.com/en-us/on-demand/session/gtcspring21-s31151/) and [How CUDA Programming Works](https://www.nvidia.com/en-us/on-demand/session/gtcspring22-s41487/)

The course [Programming Massively Parallel Processors](https://www.youtube.com/playlist?list=PLRRuQYjFhpmubuwx-w8X964ofVkW1T8O4)

![50 Years' Processor Trend](./res/50-years-processor-trend.png) from [image in microprocessor-trend-data repository](https://github.com/karlrupp/microprocessor-trend-data/blob/master/50yrs/50-years-processor-trend.png)

Numerical rows of [V100 Datasheet](https://images.nvidia.com/content/technologies/volta/pdf/volta-v100-datasheet-update-us-1165301-r5.pdf) from the official [NVIDIA Tesla V100](https://www.nvidia.com/en-gb/data-center/tesla-v100/) page

```
                             |   V100 PCIe    |    100 SXM2    |   V100S PCle
=============================+================+================+================
NVIDIA Tensor Cores          |                       640
NVIDIA CUDA Cores            |                      5,120
Double Precision Performance |    7 TFLOPS    |    8 TFLOPS    |  . .2 TFLOPS
Single Precision Performance |   14 TFLOPS    |  15.7 TFLOPS   |  16.4 TFLOPS
Tensor Performance           |   12 TFLOPS    |   125 TFLOPS   |   130 TFLOPS
GPU Memory                   |        32 GB /16 GB HBM2        |   32 GB HBM2
Memory Bandwidth             |           900 GB/sec            |  1134 GB/sec
Interconnect Bandwidth       |   32 GB/sec    |   300 GB/sec   |   32 GB/sec
Max Power Comsumption        |     250 W      |     300 W      |     250 W
=============================+================+================+================
```

Numerical rows of [A100 Datasheet](https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/a100/pdf/nvidia-a100-datasheet-nvidia-us-2188504-web.pdf) from the official [NVIDIA A100](https://www.nvidia.com/en-gb/data-center/a100/) page

```
                               |     A100 80GB PCIe    |     A100 80GB SXM
===============================+=======================+=======================
FP64                           |                   9.7 TFLOPS
FP64 Tensor Core               |                  19.5 TFLOPS
FP32                           |                  19.5 TFLOPS
Tensor Float 32 (TF32)         |            156 TFLOPS / 312 TFLOPS*
BFLOAT16 Tensor Core           |            312 TFLOPS / 624 TFLOPS*
FP16 Tensor Core               |            312 TFLOPS / 624 TFLOPS*
INT8 Tensor Core               |             624 TOPS / 1248 TOPS*
Multi-Instance GPU             |              Up to 7 MIGs @ 10GB
GPU Memory Bandwidth           |       1,935GB/s       |       2,039GB/s
Max Thermal Design Power (TDP) |          300W         |        400W***
Interconnect                   |  NVIDIA NVLink Bridge |    NVLink: 600GB/s
                               | for 2 GPUs: 600GB/s** |   PCIe Gen4: 64GB/s
                               |   PCIe Gen4: 64GB/s   |
===============================+=======================+=======================
* With sparsity
** SXM4 GPUs via HGX A100 server boards; PCIe GPUs via NVLink Bridge for up to two GPUs
*** 400W TDP for standard configuration. HGX A100-80GB CTS (Custom Thermal Solution) SKU can support TDPs up to 500W
```

![V100 Memory Hierarchy](./res/V100-memory-hierarchy.png) from [Dissecting the NVIDIA Volta GPU Architecture via Microbenchmarking](https://arxiv.org/abs/1804.06826)
