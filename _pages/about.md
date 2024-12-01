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

I am currently a Postdoctoral Fellow at the Duke Center for Computational Evolutionary Intelligence ([DCEI](https://cei.pratt.duke.edu/)), supervised by [Prof. Yiran Chen](https://cei.pratt.duke.edu/people/yiran-chen). I received the Ph. D. degree of Microelectronics and Solid-State Electronics in the School of integrated Circuits, Peking University, China, in Jan. 2024, supervised by [Prof. Hailong Jiao](https://www.ece.pku.edu.cn/info/1045/2719.htm) at [PKU-VLSI Lab](http://www.PKU-VLSI.com). I received the Bachelor degree of Microelectronics Science and Engineering from Sun Yat-sen University, Guangzhou, China, in Jul. 2018.  My research interest is energy-efficient AI chips for edge computing. You can find more information through my [CV](https://github.com/zhouchch3/changchunzhou/blob/main/docs/CV.pdf). I am looking for possible research collaboration. If you are interested in me, please feel free to contact me at any time.

<!--My research interest includes neural machine translation and computer vision. I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>).-->

# 📖 Educations
- *2018.09 - 2024.01*, Doctor of Philosophy in Microelectronics and Solid-State Electronics, Peking University, Beijing, China. Thesis Title: Research on On-Chip Neural Network Accelerators for 3D Understanding.
- *2014.09 - 2018.06*, Bachelor of Engineering in Microelectronics Science and Engineering, Sun Yat-sen University, Guangzhou, China.

<!--# 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. -->

# 🎖 Honors and Awards
- 12/2023 **Leo KoGuan Scholarship (1/157, ¥20, 000)**, *Peking University*                                                      
- 12/2023 **Exceptional Award for Academic Innovation**, *Peking University*                                           
- 12/2023 Merit Student, *Peking University*                                                                           
- 12/2022 Award for Scientific Research, *Peking University*                                                                         
- 10/2019 Merit Student, *Peking University*                                                                           
- 10/2016 National Inspirational Scholarship, *Sun Yat-sen University*                                                  
- 10/2015 National Inspirational Scholarship, *Sun Yat-sen University*                                                 
- 10/2015 First Class Scholarship, *Sun Yat-sen University*                                                            


# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ISSCC 2025</div><img src='images/ISSCC.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

Nebula: A 28-nm 109.8 TOPS/W 3D PNN Accelerator Featuring Adaptive Partition, Multi-Skipping, and Block-Wise Aggregation

**<u>C. Zhou</u>**, T. Huang, Y. Ma, Y. Fu, X. Song, S. Qiu, J. Sun, M. Liu, G. Li, Y. He, Y. Yang, and H. Jiao.

*IEEE International Solid-State Circuits Conference (**<font color=blue>ISSCC</font>**) Dig. Tech. Papers* (Accepted)

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCAS-II 2024</div><img src='images/TCAS-II.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Adjustable Multi-Stream Block-Wise Farthest Point Sampling Acceleration in Point Cloud Analysis](https://ieeexplore.ieee.org/document/10430381)

**<u>C. Zhou</u>**\*, Y. Fu*, Y. Ma, E. Han, Y. He, and H. Jiao

*IEEE Transactions on Circuits and Systems II: Express Briefs (**TCAS-II**)*


<details>
<summary>Abstract</summary>
Point cloud is increasingly used in a variety of applications. Farthest Point Sampling (FPS) is typically employed for down-sampling to reduce the size of point cloud and enhance the representational capability by preserving contour points in point cloud analysis. However, due to low parallelism and high computational complexity, high energy consumption and long latency are caused, which becomes a bottleneck of hardware acceleration. In this brief, we propose an adjustable multi-stream block-wise FPS, adjusted by four configurable parameters, according to hardware and accuracy requirements. A unified hardware architecture is designed to implement the adjustable multi-stream block-wise FPS. Furthermore, we present a rapid searching algorithm to select the optimal configuration of the four parameters. Designed in an industrial 28-nm CMOS technology, the proposed hardware architecture achieves a latency of 0.005 ms and a frame energy consumption of 0.09 µJ/frame for 1 k input points at 200 MHz and 0.9 V supply voltage. Compared to the state of the art, the proposed hardware architecture reduces the latency by up to 84.38%, saves the energy by up to 76.19%, and improves the network accuracy by up to 1.05%.

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


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">JIOT 2023</div><img src='images/IOTJ.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Sagitta: An Energy-Efficient Sparse 3D-CNN Accelerator for Real-Time 3D Understanding.](https://ieeexplore.ieee.org/abstract/document/10224248/)

**<u>C. Zhou</u>**, M. Liu, S. Qiu, X. Cao, Y. Fu, Y. He, and H. Jiao.

*IEEE Internet of Things Journal (**JIOT**)*


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


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCSVT 2024</div><img src='images/TCAS-I.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SoftAct: A High-Precision Softmax Architecture for Transformers with Nonlinear Functions Support](https://ieeexplore.ieee.org/document/10495359/)

Y. Fu, **<u>C. Zhou</u>**, T. Huang, E. Han, Y. He, and H. Jiao.

*IEEE Transactions on Circuits and Systems for Video Technology(**TCSVT**)*


<details>
<summary>Abstract</summary>
Transformer-based deep learning networks are revolutionizing our society. The convolution and attention codesigned (CAC) Transformers have demonstrated superior performance compared to the conventional Transformer-based networks. However, CAC Transformer networks contain various nonlinear functions, such as softmax and complex activation functions, which require high precision hardware design yet typically with significant cost in area and power consumption. To address these challenges, SoftAct, a compact and high-precision algorithm-hardware co-designed architecture, is proposed to implement both softmax and nonlinear activation functions in CAC Transformer accelerators. An improved softmax algorithm with penalties is proposed to maintain precision in hardware. A stage-wise full zero detection method is developed to skip redundant computation in softmax. A compact and reconfigurable architecture with a symmetrically designed linear fitting module is proposed to achieve nonlinear functions. The SoftAct architecture is designed in an industrial 28-nm CMOS technology with the MobileViT-xxs network as the benchmark. Compared with the state of the art, SoftAct achieves up to 35.14% network accuracy improvement, 10× maximum frequency, and 809× overall efficiency.

</details>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ISCAS 2024</div><img src='images/ISCAS.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

An Energy-Efficient Configurable Coprocessor Based on 1-D CNN for ECG Anomaly Detection [[pdf](https://github.com/zhouchch3/changchunzhou/blob/main/docs/ISCAS.pdf)]

C. Zhang, Z. Huang, Q. Cheng, **<u>C. Zhou</u>**, and X. Wang

*IEEE International Symposium on Circuits and Systems (**ISCAS**) (Accepted)*


<details>
<summary>Abstract</summary>
Many healthcare devices have been widely used for electrocardiogram (ECG) monitoring. However, most of them have relatively low energy efficiency and lack flexibility. A novel ECG coprocessor is proposed in this paper, which can perform efficient ECG nomaly detection. In order to achieve high sensitivity and positive precision of R-peak detection, an algorithm based on Hilbert transform and adaptive threshold comparison is proposed. Also, a flexible one-dimensional convolutional neural network (1-D CNN) based classification engine is adopted, which can be configured with instructions to process various network models for ifferent applications. Good energy efficiency is achieved by combining filter level parallelism and output channel parallelism within the processing element (PE) array with data reuse strategy. A 1-D CNN for arrhythmia detection is proposed to validate the hardware performance. The proposed ECG coprocessor is implemented using 55 nm CMOS technology, occupying an area of 1.39 mm2. At a clock frequency of 100MHz, the energy efficiency is 215.6 nJ/classification. The comparison results show that this design has advantages in energy overhead and detection performance.

</details>

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TCSVT 2023</div><img src='images/TCSVT.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[CNN Accelerator at the Edge with Adaptive Zero Skipping and Sparsity-Driven Data Flow](https://ieeexplore.ieee.org/abstract/document/10122694/)

M. Liu, **<u>C. Zhou</u>**, S. Qiu, Y. He, and H. Jiao.

*IEEE Transactions on Circuits and Systems for Video Technology(**TCSVT**)*


<details>
<summary>Abstract</summary>
An energy-efficient convolutional neural network (CNN) accelerator is proposed for low-power inference on edge devices. An adaptive zero skipping technique is proposed to dynamically skip the zeros in either activations or weights, depending on which has the higher sparsity. The characteristic of non-zero data aggregation is explored to enhance the effectiveness of adaptive zero skipping in performance boosting. To mitigate the load imbalance issue after zero skipping, a sparsity-driven data flow and low-complexity dynamic task allocation are employed for different convolution layers. Facilitated further by a two-stage distiller, the proposed accelerator achieves 5.42×, 3.41×, and 3.42× performance boosting for VGG16, AlexNet, and Mobilenet-v1, respectively, compared to the baseline. Implemented in a 55-nm low power CMOS technology, the proposed accelerator achieves an effective energy efficiency of 2.41 TOPS/W, 2.35 TOPS/W, and 0.64 TOPS/W for VGG16, AlexNet, and Mobilenet-v1, respectively, at 100 MHz and 1.08 V supply voltage.

</details>

</div>
</div>


# 🍀 Tape Out

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Transformer</div><img src='images/bit_variable_imc.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A bit-variable in-memory computing chip for accelerating transformers at the edge.

12/2025 (Expected), Project Leader

*Fabricated in TSMC 40-nm technology with an expected area of 1 mm×1 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Transformer</div><img src='images/nebula_v2_chip.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

An energy-efficient acceleration chip supporting transformer-based networks.

01/2025 (Expected), Project Leader

*Fabricated in TSMC 28-nm HPC technology with an expected area of 2.0 mm×3 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Point Cloud</div><img src='images/28nm.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

An energy-efficient pipelined and configurable 3D point cloud-based neural network accelerator.

08/2023, Project Leader

*Fabricated in TSMC 28-nm HPC technology with an area of 2.0 mm×1.5 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">3D-CNN</div><img src='images/55nm_micrograph.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A 4.5 TOPS/W sparse 3D-CNN accelerator for real-time 3D understanding

08/2020, Project Leader

*Fabricated in UMC 55-nm low-power CMOS technology with an area of 4.2 mm×3.6 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">1D-CNN</div><img src='images/1DCNN_Chips.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

1D-CNN accelerators for medical analysis

06/2024, Collaboration

*Fabricated in UMC 55-nm and TSMC 65-nm low-power CMOS technology*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2D-CNN</div><img src='images/LIU_28_Chip.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A 2.4 TOPS/W CNN accelerator with adaptive zero skipping and sparsity-driven dataflow

06/2022, Collaboration

*Fabricated in TSMC 28-nm HPC technology with an area of 2.0 mm×1.35 mm*

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2D-CNN</div><img src='images/LIU_55_Chip.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

A 2.0 TOPS/W CNN accelerator skipping invalid activations

10/2019, Collaboration

*Fabricated in UMC 55-nm low-power CMOS technology with an area of 3.4 mm×2.3 mm*

</div>
</div>




# 💻 Skills
- Flow: IC Front-End, Logic Synthesis, FPGA, Neural Network Training
- Tools: Cadence, Vivado, PyTorch, TensorFlow 
- Language: Verilog, SystemVerilog, Python, C, Shell, Makefile

# 💬 About Me
- I am an Easy Going and Self-Motivated Person. Feel Free to Reach out Anytime!
- Interests and Hobbies: Fitness, Taekwondo(Black Belt), and Table Tennis.


<!-- [**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
</div>
</div>

- [Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet](https://github.com), A, B, C, **CVPR 2020**

# 🎖 Honors and Awards
- *2021.10* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 


# 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/)

# 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China. -->
