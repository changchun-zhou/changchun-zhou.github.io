---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am currently a Postdoctoral Fellow at the Duke Center for Computational Evolutionary Intelligence ([DCEI](https://cei.pratt.duke.edu/)), supervised by [Prof. Yiran Chen](https://cei.pratt.duke.edu/people/yiran-chen) and [Prof. Hai "Helen" Li](https://cei.pratt.duke.edu/people/hai-helen-li). I received the Ph.D. degree of Microelectronics and Solid-State Electronics in the School of Integrated Circuits, Peking University, China, in Jan. 2024, supervised by [Prof. Hailong Jiao](https://www.ece.pku.edu.cn/info/1045/2719.htm) at [PKU-VLSI Lab](http://www.PKU-VLSI.com). I received the Bachelor degree of Microelectronics Science and Engineering from Sun Yat-sen University, Guangzhou, China, in Jul. 2018.
{: style="margin-bottom: 2em;"}

My research interest is energy-efficient AI chips for edge computing via cross-layer innovations, spanning from algorithms to architecture and circuit design. My research directions are guided by bottlenecks observed in
real hardware implementations, informing practical cross-layer insights.

**I am on the job market for tenure-track faculty positions in ECE and CS starting in Fall 2027!**


# 🧭 Research Tracks {#research-tracks}

**I. Chips for AI Acceleration** — heterogeneous, tape-out-validated accelerators for mainstream AI workloads (LLMs, diffusion, Transformers, CNNs; for text, image, video, and point cloud). Focus areas: generative-model acceleration · 3D/4D point-cloud analysis & reconstruction · embodied AI and robotics (VLA).

**II. Systems for AI Deployment** — end-to-end serving systems that run AI on customized chip clusters (or FPGAs), accessible via web platforms and mobile apps: hardware-aware algorithms · AI compilers (e.g., MLIR) · schedulers — delivering up to two–three orders-of-magnitude cost and energy advantages over GPU baselines in edge workloads.

**III. AI for Chip Design** — silicon-validated, agent-driven design flows that carry a chip from idea to GDS, through tape-out, to measured silicon and live demos, in a closed loop, now applied in our ongoing tape-outs.


# 🍀 Chip Gallery {#chip-gallery}

<img src="images/chips_platform.jpg?v=20261021" alt="Chip Gallery and Test Platforms" width="92%">


# 📝 Selected Publications {#publications}

*Lead-author work across chips, architectures, and algorithms.* 


<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="background-color:#c8102e;">ISSCC 2027</div><img src='images/ISSCC2027_Fornax.jpg' alt="Fornax ISSCC 2027" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

Fornax: A 16nm 16-Die Diffusion Processor with Fractal Recursion and Bit-Plane Folding for 8K Edge Image Generation

**<u>C. Zhou</u>**, Z. Guo, Z. Xu, E. Dai, Y. Zhong, G. Zhou, J. Zhang, J. Ku, H. Li, and Y. Chen.

*IEEE International Solid-State Circuits Conference (**<font color=red>ISSCC</font>**) Dig. Tech. Papers, Paper 34.6 (Accepted)* <span style="display:inline-block;background-color:#c8102e;color:#fff;font-weight:bold;font-size:.8em;padding:1px 8px;border-radius:3px;">★ Highlight Paper</span>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="background-color:#c8102e;">ISSCC 2027</div><img src='images/ISSCC2027_LYRA.jpg' alt="LYRA ISSCC 2027" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

LYRA: A 3.5nJ/Point Streaming 4D Point-Cloud Transformer Processor with Spatial Registration and Incremental Inference

**<u>C. Zhou</u>**\*, Y. Ma\*, W. Luo, X. Wang, Z. Li, Z. Guo, Y. Jiang, Z. Guo, Z. Gao, Y. Lin, H. He, A. Li, Y. Fu, S. Qiu, C. Zhang, Y. He, G. Li, Y. Yang, and H. Jiao. (**\*Equal Contribution**)

*IEEE International Solid-State Circuits Conference (**<font color=red>ISSCC</font>**) Dig. Tech. Papers, Paper 34.2 (Accepted)* <span style="display:inline-block;background-color:#c8102e;color:#fff;font-weight:bold;font-size:.8em;padding:1px 8px;border-radius:3px;">★ Highlight Paper</span>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">DAC 2026</div><img src='images/DAC2026_FlashFPS.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

FlashFPS: Efficient Farthest Point Sampling for Large-Scale Point Clouds via Pruning and Caching

Y. Fu, H. Ye, C. Guo#, J. Zhang, Q. Wang, Y. Lin, **<u>C. Zhou</u>#**, H. Li, and Y. Chen. (**#Corresponding Author**)

*IEEE/ACM Design Automation Conference (**DAC**) (Accepted)*

<details>
<summary>Abstract</summary>
Point-based Neural Networks (PNNs) have become a key approach for point cloud processing. However, a core operation in these models, Farthest Point Sampling (FPS), often introduces significant inference latency, especially for large-scale processing. Despite existing CUDA- and hardware-level optimizations, FPS remains a major bottleneck due to exhaustive computations across multiple network layers in PNNs, which hinders scalability.Through systematic analysis, we identify three substantial redundancies in FPS, including unnecessary full-cloud computations, redundant late-stage iterations, and predictable inter-layer outputs that make later FPS computations avoidable. To address these, we propose FlashFPS, a hardware-agnostic, plug-and-play framework for FPS acceleration, composed of FPS-Prune and FPS-Cache. FPS-Prune introduces candidate pruning and iteration pruning to reduce redundant computations in FPS while preserving sampling quality, and FPS-Cache eliminates layer-wise redundancy via cache-and-reuse. Integrated into existing CUDA libraries and state-of-the-art PNN accelerators, FlashFPS achieves 5.16× speedup over the standard CUDA baseline on GPU and 2.69× on PNN accelerators, with negligible accuracy loss, enabling efficient and scalable PNN inference.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICLR 2026</div><img src='images/ICLR2026_IncVGGT.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[IncVGGT: Incremental VGGT for Memory-Bounded Long-Range 3D Reconstruction](https://openreview.net/pdf?id=CezA1eLa1Y)

K. Fang, **<u>C. Zhou</u>#**, Y. Fu, H. Li, and Y. Chen. (**#Corresponding Author**)

*International Conference on Learning Representations (**ICLR**) (Accepted)*

<details>
<summary>Abstract</summary>
We present IncVGGT, a training-free incremental variant of VGGT that makes transformer-based 3D reconstruction feasible for long sequences in real-world applications. Vanilla VGGT relies on dense global attention, which causes memory to grow quadratically and requires excessive computation, making it impractical for long-sequence scenarios. Even evolved streaming variants, such as StreamVGGT, still suffer from rapidly growing cache and latency. IncVGGT addresses these challenges from two orthogonal directions: (1) register and fuse overlapping frames into composite views, reducing duplicate tokens, and (2) history-side pruning retains only the top-
k most relevant/maximum slots together with the most recent one, bounding cache growth. This incremental and memory-efficient design minimizes computation and memory occupation across arbitrarily long sequences. Compared to StreamVGGT, IncVGGT sustains arbitrarily long sequences with large efficiency gains (e.g., on 500-frame sequences, 58.5x fewer operators, 9x lower memory, 25.7x less energy, and 4.9x faster inference) while maintaining comparable accuracy. More importantly, unlike existing baselines that directly run out of memory beyond 300 (VGGT)–500 (StreamVGGT) frames, IncVGGT continues to operate smoothly even on 10k-frame inputs under an 80GB GPU, showing that our design truly scales to ultra-long sequences without hitting memory limits. These results highlight IncVGGT’s potential for deployment in resource-constrained edge devices for long-range 3D scenarios.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCAS-I 2026</div><img src='images/TCAS-I-CVR.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[A CMOS Voltage Reference Featuring a Tandem Differential Structure With Two-Stage Stacked Diode-Connected MOSFETs Core](https://ieeexplore.ieee.org/document/11301867)

Q. Zhou, Y. Liu, K. Zeng, X. Zhu, **<u>C. Zhou</u>#** and Q. Hua#. (**#Corresponding Author**)

*IEEE Transactions on Circuits and Systems I: Regular Papers (**TCAS-I**)*

<details>
<summary>Abstract</summary>
In this paper, A CMOS voltage reference (CVR) with two-stage self-biased stacked diode connected MOS transistors (SDMTs) which actively compensates for process, voltage, and temperature (PVT) variations via a tandem differential structure (TDS) is proposed. The SDMTs core biased by new pseudo cascode current mirror guarantees better suppression against supply change and generates two reference voltages. The TDS, composed of two tandem NMOS transistors, serves as an output stage, differentially processing these voltages and compensating the final reference against PVT variations. Thus, the deviation of final reference voltage from PVT change is largely reduced. The proposed CVR is fabricated in a 0.18- μ m CMOS process occupying a total area of 0.0048 mm2 . Measurement results from 7 chips demonstrate that the design can achieve an average temperature coefficient of 67 ppm/° C from −40° C to 140° C without trimming networks. Line sensitivity and power supply rejection ratio are 0.009 %/V with a supply range of 1.3V to 2.5 V and -83 dB at 100 Hz. 1% settling time only takes 0.28ms. The average reference voltage is 294 mV.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">HPCA 2026</div><img src='images/HPCA2026_FractalCloud.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[FractalCloud: A Fractal-Inspired Architecture for Efficient Large-Scale Point Cloud Processing](https://ieeexplore.ieee.org/document/11408589)

Y. Fu, **<u>C. Zhou</u>#**, H. Ye, B. Duan, Q. Huang, C. Wei, C. Guo#, H. Li, and Y. Chen. (**#Corresponding Author**)

*IEEE International Symposium on High-Performance Computer Architecture (**HPCA**)*

<details>
<summary>Abstract</summary>
Three-dimensional (3D) point clouds are increasingly used in applications such as autonomous driving, robotics, and virtual reality (VR). Point-based neural networks (PNNs) have demonstrated strong performance in point cloud analysis, originally targeting small-scale inputs. However, as PNNs evolve to process large-scale point clouds with hundreds of thousands of points, all-to-all computation and global memory access in point cloud processing introduce substantial overhead, causing O(n2) computational complexity and memory traffic where n is the number of points. Existing accelerators, primarily optimized for small-scale workloads, overlook this challenge and scale poorly due to inefficient partitioning and non-parallel architectures. To address these issues, we propose FractalCloud, a fractal-inspired hardware architecture for efficient large-scale 3D point cloud processing. FractalCloud introduces two key optimizations: (1) a co-designed Fractal method for shape-aware and hardware-friendly partitioning, and (2) block-parallel point operations that decompose and parallelize all point operations. A dedicated hardware design with on-chip fractal and flexible parallelism further enables fully parallel processing within limited memory resources. Implemented in 28 nm technology as a chip layout with a core area of 1.5 mm2, FractalCloud achieves 21.7× speedup and 27× energy reduction over state-of-the-art accelerators while maintaining network accuracy, demonstrating its scalability and efficiency for PNN inference.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge" style="background-color:#c8102e;">ISSCC 2025</div><img src='images/ISSCC_Nebula.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Nebula: A 28-nm 109.8 TOPS/W 3D PNN Accelerator Featuring Adaptive Partition, Multi-Skipping, and Block-Wise Aggregation](https://ieeexplore.ieee.org/document/10904703)

**<u>C. Zhou</u>**, T. Huang, Y. Ma, Y. Fu, X. Song, S. Qiu, J. Sun, M. Liu, G. Li, Y. He, Y. Yang, and H. Jiao.

*IEEE International Solid-State Circuits Conference (**<font color=red>ISSCC</font>**) Dig. Tech. Papers*

<details>
<summary>Abstract</summary>
Three-dimensional (3D) point clouds are increasingly deployed across various emerging fields, such as autonomous driving, robots, drones, and virtual reality (VR) [1]–[6]. Point-based point-cloud neural networks (PNNs) [3]–[6] have demonstrated superior performance in point-cloud analysis, compared to both sparse 3D convolution-based networks [7], [8] and graph-based convolutional neural networks [9], [10]. Due to the high computational complexity, low parallelism, and frequent irregular external memory accesses, deploying PNNs in hardware is a great challenge. PNN hardware accelerators have been developed [11]–[20]. However, three key challenges remain unsolved in these accelerators, as illustrated in Fig. 23.4.1. 1) The inherent farthest point sampling (FPS) features serial computation and suffers from quadratic growth in inference latency with rising point counts. The existing uniform block-wise FPS techniques [13], [21] fail to achieve a well-balanced block segmentation, due to a typically non-uniform point distribution. 2) A large amount of redundant operations exist for both discarded points (DPs) and retained points (RPs) in FPS. These operations exist in the sampling operations of RPs ① as well as grouping ② convolution ③, and aggregation ④ for DPs, introducing unnecessary energy and latency costs. 3) The irregular memory accesses in the aggregation operation cause significant latency penalties. Channel-wise aggregation in [11] relieves irregularity, yet is unsuitable for large-scale point clouds, as the external memory access of features and the neighbor index table (NIT) is quadratically increased due to the iterative loading of features or the NIT.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">arXiv 2025</div><img src='images/arXiv25_NeuralSymbolicHW.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Automating Hardware Design and Verification from Architectural Papers via a Neural-Symbolic Graph Framework](https://arxiv.org/abs/2511.06067)

H. Yang, X. Zhao, Y. Liu, Z. Zou, K. Lyu, **<u>C. Zhou</u>#**, Y. Zhu, and J. Hao. (**#Corresponding Author**)

*arXiv preprint arXiv:2511.06067*

<details>
<summary>Abstract</summary>
The reproduction of hardware architectures from academic papers remains a significant challenge due to the lack of publicly available source code and the complexity of hardware description languages (HDLs). To this end, we propose ArchCraft, a Framework that converts abstract architectural descriptions from academic papers into synthesizable Verilog projects with register-transfer level (RTL) verification. ArchCraft introduces a structured workflow, which uses formal graphs to capture the Architectural Blueprint and symbols to define the Functional Specification, translating unstructured academic papers into verifiable, hardware-aware designs. The framework then generates RTL and testbench (TB) code decoupled via these symbols to facilitate verification and debugging, ultimately reporting the circuit's Power, Area, and Performance (PPA). Moreover, we propose the first benchmark, ArchSynthBench, for synthesizing hardware from architectural descriptions, with a complete set of evaluation indicators, 50 project-level circuits, and around 600 circuit blocks. We systematically assess ArchCraft on ArchSynthBench, where the experiment results demonstrate the superiority of our proposed method, surpassing direct generation methods and the VerilogCoder framework in both paper understanding and code completion. Furthermore, evaluation and physical implementation of the generated executable RTL code show that these implementations meet all timing constraints without violations, and their performance metrics are consistent with those reported in the original papers.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICCAD 2023</div><img src='images/ICCAD.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[An Energy-Efficient 3D Point Cloud Neural Network Accelerator With Efficient Filter Pruning, MLP Fusion, and Dual-Stream Sampling](https://ieeexplore.ieee.org/document/10323704)

**<u>C. Zhou</u>**, Y. Fu, M. Liu, S. Qiu, G. Li, Y. He, and H. Jiao.

*IEEE/ACM International Conference On Computer Aided Design (**ICCAD**)*


<details>
<summary>Abstract</summary>
Three-dimensional (3D) point cloud has been employed in a wide range of applications recently. As a powerful weapon for point cloud analysis, point-based point cloud neural networks (PNNs) have demonstrated superior performance with less computation complexity and parameters, compared to sparse 3D convolution-based networks and graph-based convolutional neural networks. However, point-based PNNs still suffer from high computational redundancy, large off-chip memory access, and low parallelism in hardware implementation, thereby hindering the applications on edge devices. In this paper, to address these challenges, an energy-efficient 3D point cloud neural network accelerator is proposed for on-chip edge computing. An efficient filter pruning scheme is used to skip the redundant convolution of pruned filters and zero-value feature channels. A block-wise multi-layer perceptron (MLP) fusion method is proposed to increase the on-chip reuse of features, thereby reducing off-chip memory access. A dual-stream blocking technique is proposed for higher parallelism while maintaining inference accuracy. Implemented in an industrial 28-nm CMOS technology, the proposed accelerator achieves an effective energy efficiency of 12.65 TOPS/W and 0.13 mJ/frame energy consumption for PointNeXt-S at 100 MHz, 0.9 V supply voltage, and 8-bit data width. Compared to the state-of-the-art point cloud neural network accelerators, the proposed accelerator enhances the energy efficiency by up to 66.6× and reduces the energy consumption per frame by up to 70.2×. 

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">IOT Journal 2023</div><img src='images/IOTJ.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Sagitta: An Energy-Efficient Sparse 3D-CNN Accelerator for Real-Time 3D Understanding.](https://ieeexplore.ieee.org/abstract/document/10224248/)

**<u>C. Zhou</u>**, M. Liu, S. Qiu, X. Cao, Y. Fu, Y. He, and H. Jiao.

*IEEE Internet of Things Journal (**IOT Journal**)*


<details>
<summary>Abstract</summary>
Three-dimensional (3D) understanding or inference has received increasing attention, where 3D convolutional neural networks (3D-CNNs) have demonstrated superior performance compared to two-dimensional CNNs (2D-CNNs), since 3D-CNNs learn features from all three dimensions. However, 3D-CNNs suffer from intensive computation and data movement. In this paper, Sagitta, an energy-efficient low-latency on-chip 3D-CNN accelerator, is proposed for edge devices. Locality and small differential value dropout are leveraged to increase the sparsity of activations. A full-zero-skipping convolutional microarchitecture is proposed to fully utilize the sparsity of weights and activations. A hierarchical load-balancing scheme is also introduced to increase the hardware utilization. Specialized architecture and computation flow are proposed to enhance the effectiveness of the proposed techniques. Fabricated in a 55-nm CMOS technology, Sagitta achieves 3.8 TOPS/W for C3D at a latency of 0.1 s and 4.5 TOPS/W for 3D U-Net at a latency of 0.9 s at 100 MHz and 0.91 V supply voltage. Compared to the state-of-the-art 3D-CNN and 2D-CNN accelerators, Sagitta enhances the energy efficiency by up to 379.6× and 11×, respectively.

</details>

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">DAC 2021</div><img src='images/DAC.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[An Energy-Efficient Low-Latency 3D-CNN Accelerator Leveraging Temporal Locality, Full Zero-Skipping, and Hierarchical Load Balance](https://ieeexplore.ieee.org/document/9586299)

**<u>C. Zhou</u>**, M. Liu, S. Qiu, Y. He, and H. Jiao.

*IEEE/ACM Design Automation Conference (**DAC**)*


<details>
<summary>Abstract</summary>
Three-dimensional convolutional neural network (3D-CNN) has demonstrated outstanding classification performance in video recognition compared to two-dimensional CNN (2D-CNN), since 3D-CNN not only learns the spatial features of each frame, but also learns the temporal features across all frames. However, 3D-CNN suffers from intensive computation and data movement. To solve these issues, an energy-efficient low-latency 3D-CNN accelerator is proposed. Temporal locality and small differential value dropout are used to increase the sparsity of activation. Furthermore, to fully utilize the sparsity of weight and activation, a full zero-skipping convolutional microarchitecture is proposed. A hierarchical load-balancing scheme is also introduced to improve resource utilization. With the proposed techniques, a 3D-CNN accelerator is designed in a 55-nm low-power CMOS technology, bringing in up to 9.89x speedup compared to the baseline implementation. Benchmarked with C3D, the proposed accelerator achieves an energy efficiency of 4.66 TOPS/W at 100 MHz and 1.08 V supply voltage.

</details>

</div>
</div>


# 📚 Full Publication List {#full-list}

**<u>C. Zhou</u>**: me · #: corresponding author · \*: equal contribution

**Lead-Author (First or Corresponding Author)**

- **[1]** `ISSCC 2027` Fornax: A 16nm 16-Die Diffusion Processor with Fractal Recursion and Bit-Plane Folding for 8K Edge Image Generation  
  **<u>C. Zhou</u>**, Z. Guo, Z. Xu, E. Dai, Y. Zhong, G. Zhou, J. Zhang, J. Ku, H. Li, and Y. Chen.  
  *IEEE International Solid-State Circuits Conference (**<font color=red>ISSCC</font>**) Dig. Tech. Papers, Paper 34.6 (Accepted)* <span style="display:inline-block;background-color:#c8102e;color:#fff;font-weight:bold;font-size:.8em;padding:1px 8px;border-radius:3px;">★ Highlight Paper</span>
- **[2]** `ISSCC 2027` LYRA: A 3.5nJ/Point Streaming 4D Point-Cloud Transformer Processor with Spatial Registration and Incremental Inference  
  **<u>C. Zhou</u>**\*, Y. Ma\*, W. Luo, X. Wang, Z. Li, Z. Guo, Y. Jiang, Z. Guo, Z. Gao, Y. Lin, H. He, A. Li, Y. Fu, S. Qiu, C. Zhang, Y. He, G. Li, Y. Yang, and H. Jiao.  
  *IEEE International Solid-State Circuits Conference (**<font color=red>ISSCC</font>**) Dig. Tech. Papers, Paper 34.2 (Accepted)* <span style="display:inline-block;background-color:#c8102e;color:#fff;font-weight:bold;font-size:.8em;padding:1px 8px;border-radius:3px;">★ Highlight Paper</span>
- **[3]** `DAC 2026` FlashFPS: Efficient Farthest Point Sampling for Large-Scale Point Clouds via Pruning and Caching  
  Y. Fu, H. Ye, C. Guo#, J. Zhang, Q. Wang, Y. Lin, **<u>C. Zhou</u>#**, H. Li, and Y. Chen.  
  *IEEE/ACM Design Automation Conference (**DAC**) (Accepted)*
- **[4]** `ICLR 2026` [IncVGGT: Incremental VGGT for Memory-Bounded Long-Range 3D Reconstruction](https://openreview.net/pdf?id=CezA1eLa1Y)  
  K. Fang, **<u>C. Zhou</u>#**, Y. Fu, H. Li, and Y. Chen.  
  *International Conference on Learning Representations (**ICLR**) (Accepted)*
- **[5]** `ISCAS 2026` A Unified Function Processor with Integer Arithmetic Based on Piecewise Chebyshev Polynomial Approximation  
  X. Zheng, Z. Guo, and **<u>C. Zhou</u>#**.  
  *IEEE International Symposium on Circuits and Systems (**ISCAS**) (Accepted)*
- **[6]** `TCAS-I 2026` [A CMOS Voltage Reference Featuring a Tandem Differential Structure With Two-Stage Stacked Diode-Connected MOSFETs Core](https://ieeexplore.ieee.org/document/11301867)  
  Q. Zhou, Y. Liu, K. Zeng, X. Zhu, **<u>C. Zhou</u>#** and Q. Hua#.  
  *IEEE Transactions on Circuits and Systems I: Regular Papers (**TCAS-I**)*
- **[7]** `HPCA 2026` [FractalCloud: A Fractal-Inspired Architecture for Efficient Large-Scale Point Cloud Processing](https://ieeexplore.ieee.org/document/11408589)  
  Y. Fu, **<u>C. Zhou</u>#**, H. Ye, B. Duan, Q. Huang, C. Wei, C. Guo#, H. Li, and Y. Chen.  
  *IEEE International Symposium on High-Performance Computer Architecture (**HPCA**)*
- **[8]** `ISSCC 2025` [Nebula: A 28-nm 109.8 TOPS/W 3D PNN Accelerator Featuring Adaptive Partition, Multi-Skipping, and Block-Wise Aggregation](https://ieeexplore.ieee.org/document/10904703)  
  **<u>C. Zhou</u>**, T. Huang, Y. Ma, Y. Fu, X. Song, S. Qiu, J. Sun, M. Liu, G. Li, Y. He, Y. Yang, and H. Jiao.  
  *IEEE International Solid-State Circuits Conference (**<font color=red>ISSCC</font>**) Dig. Tech. Papers*
- **[9]** `arXiv 2025` [Automating Hardware Design and Verification from Architectural Papers via a Neural-Symbolic Graph Framework](https://arxiv.org/abs/2511.06067)  
  H. Yang, X. Zhao, Y. Liu, Z. Zou, K. Lyu, **<u>C. Zhou</u>#**, Y. Zhu, and J. Hao.  
  *arXiv preprint arXiv:2511.06067*
- **[10]** `TCAS-II 2024` [Adjustable Multi-Stream Block-Wise Farthest Point Sampling Acceleration in Point Cloud Analysis](https://ieeexplore.ieee.org/document/10430381)  
  **<u>C. Zhou</u>**\*, Y. Fu\*, Y. Ma, E. Han, Y. He, and H. Jiao.  
  *IEEE Transactions on Circuits and Systems II: Express Briefs (**TCAS-II**)*
- **[11]** `ICCAD 2023` [An Energy-Efficient 3D Point Cloud Neural Network Accelerator With Efficient Filter Pruning, MLP Fusion, and Dual-Stream Sampling](https://ieeexplore.ieee.org/document/10323704)  
  **<u>C. Zhou</u>**, Y. Fu, M. Liu, S. Qiu, G. Li, Y. He, and H. Jiao.  
  *IEEE/ACM International Conference On Computer Aided Design (**ICCAD**)*
- **[12]** `IOT Journal 2023` [Sagitta: An Energy-Efficient Sparse 3D-CNN Accelerator for Real-Time 3D Understanding](https://ieeexplore.ieee.org/abstract/document/10224248/)  
  **<u>C. Zhou</u>**, M. Liu, S. Qiu, X. Cao, Y. Fu, Y. He, and H. Jiao.  
  *IEEE Internet of Things Journal (**IOT Journal**)*
- **[13]** `DAC 2021` [An Energy-Efficient Low-Latency 3D-CNN Accelerator Leveraging Temporal Locality, Full Zero-Skipping, and Hierarchical Load Balance](https://ieeexplore.ieee.org/document/9586299)  
  **<u>C. Zhou</u>**, M. Liu, S. Qiu, Y. He, and H. Jiao.  
  *IEEE/ACM Design Automation Conference (**DAC**)*

**Co-Author**

- **[14]** `ISCA 2026` EVA: Recasting LLM Decoding into GEMM via an Efficient Vector Quantization Architecture  
  B. Duan, C. Guo, C. Wei, H. Shan, Y. Fu, X. Chen, Y. Xu, Z. Zhang, **<u>C. Zhou</u>**, H. Li, and Y. Chen.  
  *ACM International Symposium on Computer Architecture (**ISCA**) (Accepted)*
- **[15]** `HPCA 2026` [NP-CAM: Efficient and Scalable DNA Classification using a NoC-Partitioned CAM Architecture](https://ieeexplore.ieee.org/document/11408550)  
  B. F. Morris III, T. Molom-Ochir, **<u>C. Zhou</u>**, Y. Chen, A. Jones, and H. Li.  
  *IEEE International Symposium on High-Performance Computer Architecture (**HPCA**)*
- **[16]** `HPCA 2026` [Focus: A Streaming Concentration Architecture for Efficient Vision-Language Models](https://ieeexplore.ieee.org/document/11408525)  
  C. Wei, C. Guo, J. Zhang, H. Shan, Y. Xu, Z. Zhang, Y. Liu, Q. Wang, **<u>C. Zhou</u>**, H. Li, and Y. Chen.  
  *IEEE International Symposium on High-Performance Computer Architecture (**HPCA**)*
- **[17]** `JSSC 2026` [PANDA: A Reconfigurable Seizure Prediction and Detection Neural Network Accelerator for Epilepsy Monitoring](https://ieeexplore.ieee.org/document/11570998/)  
  S. Qiu, X. Song, X. Song, **<u>C. Zhou</u>**, X. Song, J. Yang, W. Wang, Y. Yang, and H. Jiao.  
  *IEEE Journal of Solid-State Circuits (**JSSC**)*
- **[18]** `ISCA 2025` [Ecco: Improving Memory Bandwidth and Capacity for LLMs via Entropy-Aware Cache Compression](https://dl.acm.org/doi/10.1145/3695053.3731024)  
  F. Cheng, C. Guo, C. Wei, J. Zhang, **<u>C. Zhou</u>**, E. Hanson, J. Zhang, X. Liu, H. Li, and Y. Chen.  
  *ACM International Symposium on Computer Architecture (**ISCA**)*
- **[19]** `TIM 2025` [A Two-Stage Prediction + Detection Framework for Real-Time Epileptic Seizure Monitoring](https://ieeexplore.ieee.org/document/10950403/)  
  S. Qiu, W. Wang, **<u>C. Zhou</u>**, X. Song, J. Yang, and H. Jiao.  
  *IEEE Transactions on Instrumentation and Measurement  (**TIM**)*
- **[20]** `Symp. VLSI 2025` [PANDA: A 3.178 TOPS/W Reconfigurable Seizure Prediction ANd Detection Neural Network Accelerator for Epilepsy Monitoring](https://ieeexplore.ieee.org/document/11075036/)  
  S. Qiu, X. Song, X. Song, **<u>C. Zhou</u>**, X. Song, J. Yang, W. Wang, Y. Yang, and H. Jiao.  
  *IEEE Symposium on VLSI Technology and Circuits (**Symp. VLSI**)*
- **[21]** `TBioCAS 2025` [An Energy-Efficient Configurable 1-D CNN-Based Multi-Lead ECG Classification Coprocessor for Wearable Cardiac Monitoring Devices](https://ieeexplore.ieee.org/abstract/document/10844856)  
  C. Zhang, Z. Huang, **<u>C. Zhou</u>**, A. Qie, and X. Wang.  
  *IEEE Transactions on Biomedical Circuits and Systems (**TBioCAS**)*
- **[22]** `BSPC 2025` [Automatic epileptic seizure detection with an ultra lightweight 3D-CNN model](https://www.sciencedirect.com/science/article/pii/S1746809425007712)  
  C. Xie, S. Qiu, **<u>C. Zhou</u>**, X. Song, J. Yang, J. Huang, W. Wang, and H. Jiao.  
  *Biomedical Signal Processing and Control (**BSPC**)*
- **[23]** `ISCAS 2024` [An Energy-Efficient Configurable Coprocessor Based on 1-D CNN for ECG Anomaly Detection](https://ieeexplore.ieee.org/abstract/document/10557838)  
  C. Zhang, Z. Huang, Q. Cheng, **<u>C. Zhou</u>**, and X. Wang.  
  *IEEE International Symposium on Circuits and Systems (**ISCAS**)*
- **[24]** `TCSVT 2024` [SoftAct: A High-Precision Softmax Architecture for Transformers with Nonlinear Functions Support](https://ieeexplore.ieee.org/document/10495359/)  
  Y. Fu, **<u>C. Zhou</u>**, T. Huang, E. Han, Y. He, and H. Jiao.  
  *IEEE Transactions on Circuits and Systems for Video Technology(**TCSVT**)*
- **[25]** `TCSVT 2023` [CNN Accelerator at the Edge with Adaptive Zero Skipping and Sparsity-Driven Data Flow](https://ieeexplore.ieee.org/abstract/document/10122694/)  
  M. Liu, **<u>C. Zhou</u>**, S. Qiu, Y. He, and H. Jiao.  
  *IEEE Transactions on Circuits and Systems for Video Technology(**TCSVT**)*

# 👥 Research Mentoring {#mentoring}

<div style="columns: 2 300px; column-gap: 2em;" markdown="1">

- **Zhenhua Xu** (Master) — Efficient ML
- **Yibo Huang** (Undergrad) — IC Design
- **Chongxiang Zhao** (Undergrad) — IC Design
- **Yuntian Liu** (Master) — Arch & IC Design
- **Fengqi Yu** (Master) — IC Design
- **[Ziyi Guo](https://elana-ehsan.github.io/)** (Ph.D.) — IC Design
- **[Yunyang Lu](https://wihxlyy.github.io/)** (Master) — Arch & IC Design
- **Yiming Zhou** (Master) — IC Design
- **[Zhouzhuo Guo](https://zhouzhuoguo.github.io/)** (Ph.D.) — IC Design
- **Keyu Fang** (Ph.D.) — Efficient ML
- **Vito Wang** (Undergrad) — IC Design
- **[Endong Dai](https://endong-dai.github.io/)** (Master) — IC Design
- **Tai Yu** (Ph.D.) — IC Design
- **Junzhao Huang** (Master) — Efficient ML
- **[Yueyang Zhong](https://and-landy.github.io/)** (Undergrad) — Systems
- **Haotian Chen** (Master) — IC Design
- **Binglin Cheng** (Master) — IC Design
- **Ziqian Gao** (Master) — Systems
- **Kaiwen Tang** (Master) — IC Design
- **Chengyuan Zhang** (Undergrad) — IC Design

</div>

# 📖 Education {#education}
- *2018.09 - 2024.01*, Doctor of Philosophy in Microelectronics and Solid-State Electronics, Peking University, Beijing, China. Thesis Title: Research on On-Chip Neural Network Accelerators for 3D Understanding.
- *2014.09 - 2018.06*, Bachelor of Engineering in Microelectronics Science and Engineering, Sun Yat-sen University, Guangzhou, China.


# 🎖 Honors and Awards {#honors}
- 11/2026 ISSCC 2027 Session Highlight, two papers (*LYRA* and *Fornax*)
- 02/2026 Best Paper Nomination, *IEEE HPCA 2026*
- 12/2023 Leo KoGuan Scholarship (1/157, ¥20,000), *Peking University*                                                      
- 12/2023 Exceptional Award for Academic Innovation, *Peking University*                                                                                                                  
- 12/2022 Award for Scientific Research, *Peking University*                                                                                                                                  
- 05/2021 Best Presentation Award, *IEEE CASS Shanghai and Shenzhen Joint Workshop (SSJW 2021)*

# 👔 Academic Service {#service}
- **Technical Program Committee:**
  - ACM/IEEE International Symposium on Computer Architecture (**ISCA**) 2027
  - IEEE International Symposium on High-Performance Computer Architecture (**HPCA**) 2027
  - Design Automation Conference (**DAC**) 2026
- **Conference Reviewer:**
  - IEEE/CVF Conference on Computer Vision and Pattern Recognition (**CVPR**) 2027
  - International Conference on Learning Representations (**ICLR**) 2027
  - IEEE International Symposium on Circuits and Systems (**ISCAS**) 2027
  - IEEE International Symposium on Circuits and Systems (**ISCAS**) 2026
- **Journal Reviewer:**
  - IEEE Transactions on Very Large Scale Integration Systems (**TVLSI**)
  - IEEE Transactions on Circuits and Systems I: Regular Papers (**TCAS-I**)
  - IEEE Journal on Emerging and Selected Topics in Circuits and Systems (**JETCAS**)
  - IEEE Internet of Things Journal (**IoT-J**)
  - IEEE Journal of Biomedical and Health Informatics (**JBHI**)

<div style="width:67%; margin:0 auto;">
<script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=_BR7QekQGZnFn3itv4-ySG-lm-FuV_MoJjqvcMQ5LXo&cl=ffffff&w=a"></script>
</div>

