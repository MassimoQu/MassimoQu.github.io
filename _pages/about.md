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

# 🥋 About me

I am a researcher and current Research Assistant at <a href="http://www.svm.tsinghua.edu.cn/"> the School of Vehicle and Mobility</a>, <a href="https://www.tsinghua.edu.cn/">Tsinghua University</a>, under the mentorship of Prof. <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Xinyu Zhang</a> and Prof. <a href="https://www.tsinghua.edu.cn/info/1166/93890.htm">Jun Li</a>. I earned my B.Eng in Computer Science and Technology from <a href="https://www.cumtb.edu.cn/">China University of Mining and Technology (CUMTB)</a> in 2023, where I was guided by Prof. <a href="https://ai.cumtb.edu.cn/info/1053/1134.htm">Jiajing Li</a>. Further enhancing my research credentials, I participated in joint training with <a href="https://www.tsinghua.edu.cn/">Tsinghua University</a> from 2023 to 2024.

My research focuses on 3D computer vision and its application to spatial intelligence in autonomous systems, centered on the core challenge of data consistency (or alignment). Previously, my work focused on the foundational challenge of Spatio-Temporal Alignment for the V2X sensing systems. Recently, I'm actively explore the potential of Large Foundation Model (LFM) and Multi-Modal Large Language Models (MLLM) for this field.

I am actively seeking exploring MPhil/PhD programs to further my research on Large Model technologies and their applications in autonomous systems——any opportunities or referrals would be greatly appreciated! Please feel free to reach out!

# 🦄 Research

### tl;dr

- 3D computer vision: Registration/Calibration, Perception, SLAM.
- Autonomous Driving: Scene Understanding for V2X; End-to-End Driving.
- Application of MLLMs & VLA: Cooperative Perception, Scene Understanding, End-to-End Driving, Robot Manipulation.

### Overview

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.95em;">
The following overview frames my research from a specific perspective on 3D computer vision and its application to spatial intelligence in autonomous systems. This categorization is based on my personal understanding of the field's trajectory and may differ from conventional views. I welcome any discussion, differing perspectives, or collaboration!
</div>

My research vision is to enable autonomous systems, such as self-driving vehicles, with robust Spatial Intelligence. Within this broad domain, I focus on the data consistency or the data alignment problem arising from heterogeneous data inputs (e.g., images, point clouds).

I define this "alignment" as the process of mapping heterogeneous data to a common frame of reference, targeting consistency with real-world geometry or semantics. The varying characteristics of different data types (e.g., density, modality) create significant challenges in the accuracy of this mapping. Historically, this problem has evolved from manual methods to analytical, feature-based approaches, and now to data-driven deep learning models.

In this evolution, the boundary between data alignment and data fusion is blurring. However, I argue that the importance of alignment is not diminishing; it is merely taking new forms, being absorbed and integrated from upstream modules into downstream components. This observation leads to my ultimate research goal: to develop a new paradigm for data and feature alignment, moving beyond the current scattered, case-by-case solutions. I believe the problem of spatial data/feature consistency is critical enough to demand its own unified framework. My research aims to build this framework, exploring these issues extensively, and I broadly categorize my contributions into two main areas: Explicit Alignment and Implicit Alignment.

#### 1. Explicit Alignment

Explicit Alignment refers to classical, often upstream, tasks where alignment is the direct and primary objective. The most typical examples are sensor spatio-temporal calibration and data registration. A early portion of my published work, such as our Camera-LiDARs Calibration research (T-IM 2023), falls into this category.

My primary focus is on the new challenges that arise as autonomous systems evolve from single-agent intelligence to multi-agent cooperative systems (e.g., V2X in intelligent transportation). My representative publications (IROS 2024, T-ITS 2025, and our IoT-J survey) all investigate the unique data consistency problems in these emerging multi-agent scenarios. 

Another major class of explicit alignment is map-based localization, including SLAM, which is fundamentally a geometric matching and alignment task. I have also contributed to this area (T-ASE 2024).

#### 2. Implicit Alignment

Implicit Alignment is a concept based on my personal observations of current trends. I have observed that while multi-agent cooperative perception models are affected by data alignment accuracy, many new methods demonstrate robustness to alignment errors. This seems to reduce the pressure on upstream alignment, but I argue that these models are absorbing part of the alignment task, performing compensatory alignment within their intermediate feature layers. This reflects a subtle but significant shift in functional responsibility in the era of end-to-end models. My work under review (CoSTr) explores this path by optimizing alignment at the sparse feature level.

Furthermore, this concept of implicit alignment can be observed at even later stages, which I am currently investigating along three lines:

* MLLM-based Scene Understanding: I have observed surprising and promising capabilities of large models in handling alignment, as seen in the experiments of my ongoing paper (WAMoE3D). This will be a major focus of my future work.

* Pose-Free 3D Foundation Model: The development of pose-free 3D foundation models(like VGGT) offers new insights into how systems can learn to align data without explicit pose information, which is also what I'm currently investigating.

* End-to-End Driving: I am exploring how tasks further downstream, such as end-to-end driving or planning (UniMM-V2X), react to the quality of upstream data alignment, which helps quantify the impact of both explicit and implicit alignment on final system performance.

# 🔥 News
- *2025.08*: &nbsp;🎉🎉 Our paper "V2X-Reg++: A Real-time Global Registration Method for Multi-End Sensing System in Urban Intersections" has been accepted by IEEE T-ITS (JCR Q1, IF:8.4).
- *2025.05*: &nbsp;🎉🎉 Our survey paper "Cooperative Visual-LiDAR Extrinsic Calibration Technology for Intersection Vehicle-Infrastructure: A review" was accepted by IEEE IoT-J (JCR Q1, IF:8.9).
- *2024.08*: &nbsp;🎉🎉 Our paper "GF-SLAM: A Novel Hybrid Localization Method Incorporating Global and Arc Features" was accepted by IEEE T-ASE (JCR Q1, IF=5.9).
- *2024.06*: &nbsp;🎉🎉 Our paper "V2I-Calib: A Novel Calibration Approach for Collaborative Vehicle and Infrastructure LiDAR Systems" was orally presented at IROS 2024(flagship conferences in Robotics). 
- *2023.11*: &nbsp;🎉🎉 Our paper "Automated Extrinsic Calibration  of Multi-Cameras and LiDAR" has been accepted by IEEE T-IM (JCR Q1, IF:6.4).

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">T-ITS 2025</div><img src='images/TITS-V2ICALIB++.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> V2X-Reg++: A Real-time Global Registration Method for Multi-End Sensing System in Urban Intersections </p>
<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.9em;"> <strong>Qianxin Qu</strong>*, Xinyu Zhang*, Yijin Xiong†*, Chen Xia, Ziqiang Song, Qian Peng, Kang Liu, Jun Li </div>

<!-- **Qianxin Qu**\*, Xinyu Zhang\*, Yijin Xiong†, Chen Xia, Ziqiang Song, Qian Peng, Kang Liu, Jun Li -->

Accepted by IEEE Transactions on Intelligent Transportation Systems(T-ITS, CAS Q1 top, JCR Q1, IF:8.4)


<a href="https://arxiv.org/abs/2410.11008"><img src="https://img.shields.io/badge/arXiv-2410.11008-b31b1b?logo=arxiv" alt="arXiv" /></a>  <a href="https://github.com/MassimoQu/v2i-calib"><img src="https://img.shields.io/github/stars/MassimoQu/v2i-calib?style=social" alt="" /> </a> 

*tl;dr:* We argue that current spatial alignment methods, which require an initial pose, are impractical for real-world V2X cooperative perception. To address this limitation, we propose an online global registration algorithm that uses perception priors to align heterogeneous sensors in real-time.

</div>
</div>




<div class='paper-box'><div class='paper-box-image'><div><div class="badge">IROS 2024 oral</div><img src='images/IROS2024_V2I-CALIB.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> V2I-Calib: A Novel Calibration Approach for Collaborative Vehicle and Infrastructure LiDAR Systems </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.9em;"><strong>Qianxin Qu</strong>*, Yijin Xiong* , Guipeng Zhang , Xin Wu , Xiaohan Gao , Xin Gao , Hanyu Li , Shichun Guo , Guoying Zhang†</div>

<!-- **Qianxin Qu**\*, Yijin Xiong\* , Guipeng Zhang , Xin Wu , Xiaohan Gao , Xin Gao , Hanyu Li , Shichun Guo , Guoying Zhang† -->

IEEE/RSJ International Conference on Intelligent Robots and Systems(IROS), 2024


<a href="https://ieeexplore.ieee.org/abstract/document/10802098"><img src="https://img.shields.io/badge/IROS25-Paper-blue?logo=paper"/> </a>  <a href="https://github.com/MassimoQu/v2i-calib"><img src="https://img.shields.io/github/stars/MassimoQu/v2i-calib?style=social" alt="" /> </a>  <a href="https://mp.weixin.qq.com/s?search_click_id=2428615448500534455-1727774148445-8298043828&__biz=MzkyMDY0OTc1NA==&mid=2247504642&idx=1&sn=5e8e8f523c59fc69bf997fa4d99b8897&chksm=c0cebdfa1d2adf1bb12c4a4806f62e77c9e81423bee9d0726d95003f5c9f57a08b1b22944373&scene=7&subscene=10000&sessionid=1727767087&clicktime=1727774148&enterid=1727774148&ascene=65&fasttmpl_type=0&fasttmpl_fullversion=7404782-en_US-zip&fasttmpl_flag=0&realreporttime=1727774148463&devicetype=android-34&version=28003337&nettype=3gnet&abtest_cookie=AAACAA%3D%3D&lang=en&countrycode=IT&exportkey=n_ChQIAhIQOf1YI7b%2BnFnQn0bb%2Fz%2B%2B4xLfAQIE97dBBAEAAAAAAK6AKbESUMEAAAAOpnltbLcz9gKNyK89dVj0PhCrrft%2BplkV1nNAvevodERZfCUl1%2Fb4M2DDiZD%2FbFVoZegjV4q%2FDtLGSxD356hm284NbUCDDnGQLomN2VVb7NDh9nFtDUxc1HK49ZQ8Hu8Tt25eKvwfVm2Wo%2BD1OCMS%2FexqYgoqy7MI%2Bn9cGyonbnsPt5sBU9cTjqu0L5GwQ1XE9nVqSDWJXBOrEAPh2oxNMo0%2FPD8JlPaXFIl5fO%2F6m45NUNx05YrM6xkf0LuFo0f%2BY9rwabhb3Dw%3D&pass_ticket=d19o4MvXBDDn6peTtEFxPIxAp6v3oFFS%2FUdTdsUkXZPfGJXKz%2FFaO%2FmHzyq%2FcRAy&wx_header=3"><img src="https://img.shields.io/badge/Chinese_Blog-09B83E?logo=wechat&logoColor=white&label="> </a> 

*tl;dr:* We re-examine the evolution of sensor calibration in V2I scenarios, highlighting the shift in demand from static, one-time calibration to dynamic, continuous alignment. We then propose an online, global registration of cross-source point cloud for algorithm for V2I.

</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">IoT-J 2025</div><img src='images/arxiv2024_survey.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> Cooperative Visual-LiDAR Extrinsic Calibration Technology for Intersection Vehicle-Infrastructure: A review  </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.25em;"> Yijin Xiong, Xinyu Zhang†, Xin Gao, <strong>Qianxin Qu</strong>, Chun Duan, Renjie Wang, Jing Liu, Jun Li </div>

<!-- <div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
Note: The author order on the initial submission was (Xinyu Zhang, Yijin Xiong†, <strong>Qianxin Qu</strong>, Renjie Wang, Xin Gao, Jing Liu, Shichun Guo, Jun Li). The list was finalized post-acceptance due to 场外因素. 

Contributions of Authors: This work is initially led by <a href="https://scholar.google.com/citations?user=myxo9mQAAAAJ">Dr. Yijin Xiong</a>, she identified a gap in V2X calibration literature while summarizing traditional methods. Yet Renjie Wang who was the first guy executing leaved this project because he couldn't find enough literature. I then took the project and innovatively decouple "spatial alignment" from downstream cooperative perception tasks, allowing us to expand the conceptual scope of V2X calibration and build out the main chapter on this novel topic. The paper received minor revision evaluation from IoT-J but I was deranked due to not participating the revision.
</div> -->

<div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
Note: This survey was initiated by <a href="https://scholar.google.com/citations?user=myxo9mQAAAAJ">Dr. Yijin Xiong</a> under the auspices of <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Prof. Xinyu Zhang</a>. My primary contribution was developing the main chapter on V2X calibration and its novel thesis: "spatial alignment" from downstream cooperative perception can be regarded as implicit calibration. The final author order (from 3rd on ArXiv submission) was adjusted post-acceptance.
</div>


IEEE Internet of Things Journal, 2025 (IoT-J, CAS Q1 top, JCR Q1, IF:8.9, Student First Author)

<a href="https://arxiv.org/abs/2405.10132"><img src="https://img.shields.io/badge/arXiv-2405.10132-b31b1b?logo=arxiv" alt="arXiv" /></a> <a href="https://ieeexplore.ieee.org/abstract/document/10993426/"><img src="https://img.shields.io/badge/IEEE-Paper-blue?logo=ieee"></a> 

*tl;dr:* This survey systematically organizes the evolution of sensor calibration from single-vehicle to cooperative intelligence.

</div>
</div>




<div class='paper-box'><div class='paper-box-image'><div><div class="badge">T-IM 2023</div><img src='images/TIM2023.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> Automated Extrinsic Calibration of Multi-Cameras and LiDAR </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.25em;">Xinyu Zhang, Yijin Xiong†, <strong>Qianxin Qu</strong>, Shifan Zhu, Shichun Guo, Dafeng Jin, Guoying Zhang, Haibing Ren, Jun Li</div>

<!-- Xinyu Zhang, Yijin Xiong†, **Qianxin Qu**, Shifan Zhu, Shichun Guo, Dafeng Jin, Guoying Zhang, Haibing Ren, Jun Li -->

<div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
Note: This research was initiated by <a href="https://scholar.google.com/citations?user=myxo9mQAAAAJ">Dr. Yijin Xiong</a> under the auspices of <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Prof. Xinyu Zhang</a>. It served as my undergraduate thesis and I was responsible for algorithm implementation, improvement, and coordinating this real-world experiment.
</div>

IEEE Transactions on Instrumentation and Measurement, 2023 (T-IM, CAS Q2 top, JCR Q1, IF:5.9, Student First Author)

<a href="assets/TechnicalReport_AutomaticOnlineCalibrationTechnologyBasedonMonocularCameraand3DLiDAR.pdf"><img src="https://img.shields.io/badge/CN-TechnicalReport-purple"/></a> <a href="https://ieeexplore.ieee.org/document/10352967"><img src="https://img.shields.io/badge/IEEE-Paper-blue?logo=paper"/></a> <a href="https://github.com/TH-Lion/Line-based-Automatic-Calibration-of-LiDAR-and-Cameras"><img src="https://img.shields.io/github/stars/TH-Lion/Line-based-Automatic-Calibration-of-LiDAR-and-Cameras?style=social" alt="" /> </a>  

*tl;dr:* We propose an online, line-feature-based method to address extrinsic parameter drift in Camera-LiDAR systems during operation. Its real-world effectiveness was validated with industry partners (<a href="https://mad.meituan.com/">Meituan</a>, <a href="https://www.mogoauto.cn/">MOGOX</a>, and <a href="https://www.saicmotor.com/">SAIC Motor</a>,).

</div>
</div>




<div class='paper-box'><div class='paper-box-image'><div><div class="badge">T-ASE 2024</div><img src='images/TASE2024_GFSLAM.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> GF-SLAM: A Novel Hybrid Localization Method Incorporating Global and Arc Features </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.25em;">
Yijin Xiong, Xinyu Zhang†, Wenju Gao, Jing Liu, <strong>Qianxin Qu</strong>, Shichun Guo, Yang Shen, Jun Li
</div>

<!-- Yijin Xiong, Xinyu Zhang†, Wenju Gao, Yuchao Wang, Jing Liu, **Qianxin Qu**, Shichun Guo, Yang Shen, Jun Li -->

<div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
*Note: This research was initiated by <a href="https://scholar.google.com/citations?user=myxo9mQAAAAJ">Dr. Yijin Xiong</a> under the auspices of <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Prof. Xinyu Zhang</a>. I was responsible for algorithm implementation and coordinating its real-world experiment.*
</div>

IEEE Transactions on Automation Science and Engineering, 2024(T-ASE, CAS Q2 top, JCR Q1, IF=6.4)

<a href="https://ieeexplore.ieee.org/abstract/document/10691946"><img src="https://img.shields.io/badge/IEEE-Paper-blue?logo=paper"/></a> 

*tl;dr:* To address cumulative error in mapping for agricultural scenarios, we propose a robot localization method that fuses global and local environmental features. I was responsible for liaising with the Academy of Agricultural Sciences and implementing the real-world validation.

</div>
</div>



### Under Review



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/ICRA2026_CoSTr.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold;  margin-bottom: 0.9em;"> CoSTr: a Fully Sparse Transformer with Mutual Information for Pragmatic Collaborative Perception </p>

<!-- **Qianxin Qu**, Chen Xia, Ziyi Song, Guipeng Zhang, Sheng Zhou†, Zhisheng Niu. -->

<!-- Under Review for ICRA 2026 -->

<a href="assets/CoSTr-full-v5.pdf"><img src="https://img.shields.io/badge/arXiv-PDF-b31b1b?logo=arxiv" alt="arXiv" /></a>

*tl;dr:* Current cooperative perception suffers from redundant dense BEV features, insufficient sparse receptive fields, and poor spatio-temporal robustness. We propose a sparse Transformer, combining mutual information and flow-awareness, to achieve a fully sparse-feature pipeline for cooperative perception.

</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/AAAI26_UniMM-V2X.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.9em;"> UniMM-V2X: MoE-Enhanced Multi-Level Fusion for End-to-End Cooperative Autonomous Driving  </p>

<a href="assets/withAppendix_UniMM-V2X_MoE-EnhancedMulti-LevelFusionforEnd-to-EndCooperativeAutonomousDriving.pdf"><img src="https://img.shields.io/badge/arXiv-PDF-b31b1b?logo=arxiv" alt="arXiv" /></a>

*tl;dr:* We argue that current cooperative driving methods, which only fuse at the perception level, fail to align with downstream planning and can even degrade performance. To address this limitation, we propose UniMM-V2X, an end-to-end framework that introduces multi-level fusion (cooperating at both perception and prediction levels) enhanced with Mixture-of-Experts (MoE).

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/ParallelismTraining.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.9em;"> A Survey on Hybrid Parallelism Techniques for Large Model Training </p>

<a href="assets/LLM_mixed_parallel_training.pdf"><img src="https://img.shields.io/badge/arXiv-PDF-b31b1b?logo=arxiv" alt="arXiv" /></a>

*tl;dr:* As traditional parallelism fails for massive Transformers , this survey reviews hybrid strategies (DP, TP, PP, SP, EP). We introduce a unified framework based on operator partitioning to analyze these methods and the evolution of automatic parallelism search.

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/WAMoE.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.9em;"> WAMoE3D: Weather-aware Mixture-of-Experts for MLLM-based 3D Scene Understanding in Autonomous Driving </p>

*tl;dr:* To address the sharp performance drop of MLLMs in adverse weather, we built a VQA dataset and benchmark for traffic scene understanding based on the <a href="https://arxiv.org/pdf/2310.07602">Dual-Radar</a> dataset. We then proposed an adaptive fusion framework for the LLaMA architecture, utilizing a Weather-aware Mixture-of-Experts (WAMoE) module to dynamically fuse camera, LiDAR, and radar features, coupled with LoRA-based fine-tuning to enhance perception and reasoning capabilities in adverse weather.

</div>
</div>



<!-- # 📖 Educations
- *2019.06 - 2022.04 (now)*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2019.09 - 2023.06*, 


<!-- # 💻 Internships
- *2019.05 - 2020.02*, [Lorem](https://github.com/), China. --> 

<script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?cl=ffffff&w=280&t=n&d=jd_2WhYJ2igXcCghIx7Djyi4Puoie_IuT4K7SfCT6z8"></script>

<footer>
  <p style="font-size: small; text-align: center;">Last updated on: {{ site.time | date: "%Y-%m-%d" }}</p>
</footer>
