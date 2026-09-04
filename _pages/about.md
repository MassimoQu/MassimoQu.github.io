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

I am **Qianxin Qu**, a Ph.D. student in the **Internet of Things (IoT) Thrust** at the <a href="https://www.hkust-gz.edu.cn/">Hong Kong University of Science and Technology (Guangzhou)</a>, advised by Prof. <a href="https://facultyprofiles.hkust-gz.edu.cn/faculty-personal-page/?id=146">Ying Cui (崔颖)</a>. I am based in Guangzhou, China, and work at the intersection of **spatial intelligence**, **V2X**, and **autonomous driving**.

<div class="current-position" markdown="1">
<span class="current-position__label">CURRENT POSITION</span>
<strong>Ph.D. Student · IoT Thrust</strong>
<span><a href="https://www.hkust-gz.edu.cn/">The Hong Kong University of Science and Technology (Guangzhou)</a></span>
<span>Advised by Prof. <a href="https://facultyprofiles.hkust-gz.edu.cn/faculty-personal-page/?id=146">Ying Cui (崔颖)</a></span>
</div>

Before starting my Ph.D., I was a Research Assistant at the <a href="http://www.svm.tsinghua.edu.cn/">School of Vehicle and Mobility</a>, <a href="https://www.tsinghua.edu.cn/">Tsinghua University</a>, mentored by Prof. <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Xinyu Zhang</a> and Prof. <a href="https://www.tsinghua.edu.cn/info/1166/93890.htm">Jun Li</a>. I earned my B.Eng. in Computer Science and Technology from <a href="https://www.cumtb.edu.cn/">China University of Mining and Technology (CUMTB)</a> in 2023, where I was guided by Prof. <a href="https://ai.cumtb.edu.cn/info/1053/1134.htm">Jiajing Li</a>. From 2022 to 2023, I also participated in joint training at Tsinghua University.

# 🦄 Research

My research focuses on building spatial intelligence for autonomous systems. I study how connected vehicles and infrastructure can perceive, align, and reason about shared 3D environments, with the goal of building reliable spatial representations for autonomous systems.

More broadly, I explore how 3D vision, Visual Language Models (VLMs), and 3D reconstruction foundation models can support spatial intelligence for autonomous systems. Much of my previous work has centered on multi-agent traffic scenarios, especially V2X / CAV settings, where the key challenge is to turn heterogeneous observations into a reliable shared spatial representation. My published work has therefore focused on spatio-temporal alignment, calibration, localization, and cooperative perception, while my more recent efforts extend this line toward VLM-based scene understanding and geometry-aware representations.

I am also exploring Agentic AI for the physical world, with a particular interest in improving agents' long-horizon task capabilities: how agents can reason over 3D and spatial observations, maintain task context, interact with embodied systems, and support decision-making in real-world autonomous scenarios. Alongside this direction, I use agentic AI to build research-assistance workflows for literature discovery, hypothesis generation, experiment planning, and manuscript iteration, while studying how researchers can collaborate effectively with agents.

My current research interests include:

- **Spatial Intelligence:** 3D vision, reconstruction foundation models, and geometry-aware representations;
- **V2X & Autonomous Driving:** cooperative perception, shared spatial reasoning, and connected autonomous systems;
- **Spatial Alignment:** registration, calibration, localization, and spatio-temporal alignment;
- **Agentic AI:** spatial reasoning for physical-world agents and human-agent research workflows.

# 📝 Publications 

<div class='paper-box' id='pub-tits2025'><div class='paper-box-image'><div><div class="badge">T-ITS 2025</div><img src='images/TITS-V2ICALIB++.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> V2X-Reg++: A Real-time Global Registration Method for Multi-End Sensing System in Urban Intersections </p>
<!-- <div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.9em;"> <strong style="color: black; text-decoration: underline;">Qianxin Qu</strong>*, <strong>Xinyu Zhang*†, Yijin Xiong*</strong>, Chen Xia, Ziqiang Song, Qian Peng, Kang Liu, Jun Li </div> -->
<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.9em;"> <strong>Xinyu Zhang*†</strong>, <strong style="color: black; text-decoration: underline;">Qianxin Qu*</strong>, Yijin Xiong, Chen Xia, Ziqiang Song, Qian Peng, Kang Liu, <strong>Jun Li†</strong>, Keqiang Li </div>
<div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
Note: This work was my independent research project, conducted under the auspices of <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Prof. Xinyu Zhang</a>. I handled the entire research process, from literature review and concept development to methodological refinement, benchmark experiments, manuscript writing, revision, and the coordination of real-vehicle tests. 
</div>

Accepted by IEEE Transactions on Intelligent Transportation Systems (T-ITS, JCR Q1, IF:8.4)


<a href="https://arxiv.org/abs/2410.11008"><img src="https://img.shields.io/badge/arXiv-2410.11008-b31b1b?logo=arxiv" alt="arXiv" /></a> <a href="https://ieeexplore.ieee.org/document/11237211"><img src="https://img.shields.io/badge/IEEE-Paper-blue"></a> <a href="https://github.com/MassimoQu/v2i-calib"><img src="https://img.shields.io/github/stars/MassimoQu/v2i-calib?style=social" alt="" /> </a> 

*tl;dr:* We argue that current spatial alignment methods, which require an initial pose, are impractical for real-world Vehicle-to-Everything (V2X) cooperative perception. To address this limitation, we propose an online global registration algorithm that uses perception priors to align heterogeneous sensors in real-time.

</div>
</div>




<div class='paper-box' id='pub-iros2024'><div class='paper-box-image'><div><div class="badge">IROS 2024 oral</div><img src='images/IROS2024_V2I-CALIB.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> V2I-Calib: A Novel Calibration Approach for Collaborative Vehicle and Infrastructure LiDAR Systems </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.9em;"><strong style="color: black; text-decoration: underline;">Qianxin Qu</strong>*, Yijin Xiong*, Guipeng Zhang, Xin Wu, Xiaohan Gao, Xin Gao, Hanyu Li, Shichun Guo, <strong>Guoying Zhang†</strong></div>

<!-- **Qianxin Qu**\*, Yijin Xiong\*, Guipeng Zhang, Xin Wu, Xiaohan Gao, Xin Gao, Hanyu Li, Shichun Guo, Guoying Zhang† -->

IEEE/RSJ International Conference on Intelligent Robots and Systems(IROS), 2024


<a href="https://ieeexplore.ieee.org/abstract/document/10802098"><img src="https://img.shields.io/badge/IROS25-Paper-blue?logo=paper"/> </a>  <a href="https://github.com/MassimoQu/v2i-calib"><img src="https://img.shields.io/github/stars/MassimoQu/v2i-calib?style=social" alt="" /> </a>  <a href="https://mp.weixin.qq.com/s?search_click_id=2428615448500534455-1727774148445-8298043828&__biz=MzkyMDY0OTc1NA==&mid=2247504642&idx=1&sn=5e8e8f523c59fc69bf997fa4d99b8897&chksm=c0cebdfa1d2adf1bb12c4a4806f62e77c9e81423bee9d0726d95003f5c9f57a08b1b22944373&scene=7&subscene=10000&sessionid=1727767087&clicktime=1727774148&enterid=1727774148&ascene=65&fasttmpl_type=0&fasttmpl_fullversion=7404782-en_US-zip&fasttmpl_flag=0&realreporttime=1727774148463&devicetype=android-34&version=28003337&nettype=3gnet&abtest_cookie=AAACAA%3D%3D&lang=en&countrycode=IT&exportkey=n_ChQIAhIQOf1YI7b%2BnFnQn0bb%2Fz%2B%2B4xLfAQIE97dBBAEAAAAAAK6AKbESUMEAAAAOpnltbLcz9gKNyK89dVj0PhCrrft%2BplkV1nNAvevodERZfCUl1%2Fb4M2DDiZD%2FbFVoZegjV4q%2FDtLGSxD356hm284NbUCDDnGQLomN2VVb7NDh9nFtDUxc1HK49ZQ8Hu8Tt25eKvwfVm2Wo%2BD1OCMS%2FexqYgoqy7MI%2Bn9cGyonbnsPt5sBU9cTjqu0L5GwQ1XE9nVqSDWJXBOrEAPh2oxNMo0%2FPD8JlPaXFIl5fO%2F6m45NUNx05YrM6xkf0LuFo0f%2BY9rwabhb3Dw%3D&pass_ticket=d19o4MvXBDDn6peTtEFxPIxAp6v3oFFS%2FUdTdsUkXZPfGJXKz%2FFaO%2FmHzyq%2FcRAy&wx_header=3"><img src="https://img.shields.io/badge/Chinese_Blog-09B83E?logo=wechat&logoColor=white&label="> </a> 

*tl;dr:* We re-examine the evolution of sensor calibration in V2I scenarios, highlighting the shift in demand from static, one-time calibration to dynamic, continuous alignment. We then propose an online, global registration of cross-source point cloud for algorithm for V2I.

</div>
</div>



<div class='paper-box' id='pub-iotj2025'><div class='paper-box-image'><div><div class="badge">IoT-J 2025</div><img src='images/arxiv2024_survey.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> Cooperative Visual-LiDAR Extrinsic Calibration Technology for Intersection Vehicle-Infrastructure: A review  </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.25em;"> Yijin Xiong, <strong>Xinyu Zhang†</strong>, Xin Gao, <strong style="color: black; text-decoration: underline;">Qianxin Qu</strong>, Chun Duan, Renjie Wang, Jing Liu, <strong>Jun Li†</strong> </div>

<div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
Note: This survey was initiated by <a href="https://scholar.google.com/citations?user=myxo9mQAAAAJ">Dr. Yijin Xiong</a> under the auspices of <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Prof. Xinyu Zhang</a>. I later took responsibility for a substantial revision of the manuscript, expanding the literature coverage from 60+ to 120+ papers and reframing V2X calibration from a direct sensor-calibration problem to a broader spatial-alignment issue that extends into downstream cooperative perception.
</div>


IEEE Internet of Things Journal, 2025 (IoT-J, JCR Q1, IF:8.9)

<a href="https://arxiv.org/abs/2405.10132"><img src="https://img.shields.io/badge/arXiv-2405.10132-b31b1b?logo=arxiv" alt="arXiv" /></a> <a href="https://ieeexplore.ieee.org/abstract/document/10993426/"><img src="https://img.shields.io/badge/IEEE-Paper-blue"></a> 

*tl;dr:* This survey systematically organizes the evolution of sensor calibration from single-vehicle to cooperative intelligence.

</div>
</div>




<div class='paper-box' id='pub-tim2023'><div class='paper-box-image'><div><div class="badge">T-IM 2023</div><img src='images/TIM2023.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> Automated Extrinsic Calibration of Multi-Cameras and LiDAR </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.25em;"> <strong>Xinyu Zhang†</strong>, Yijin Xiong, <strong style="color: black; text-decoration: underline;">Qianxin Qu</strong>, Shifan Zhu, Shichun Guo, Dafeng Jin, Guoying Zhang, Haibing Ren, <strong>Jun Li†</strong></div>

<!-- Xinyu Zhang, Yijin Xiong†, **Qianxin Qu**, Shifan Zhu, Shichun Guo, Dafeng Jin, Guoying Zhang, Haibing Ren, Jun Li -->

<div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
Note: This research was initiated by <a href="https://scholar.google.com/citations?user=myxo9mQAAAAJ">Dr. Yijin Xiong</a> under the auspices of <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Prof. Xinyu Zhang</a>. It served as my undergraduate thesis; I proposed and improved the calibration algorithm and conducted the real-vehicle validation.
</div>

IEEE Transactions on Instrumentation and Measurement, 2023 (T-IM, JCR Q1, IF:5.9, Student First Author)

<a href="assets/TechnicalReport_AutomaticOnlineCalibrationTechnologyBasedonMonocularCameraand3DLiDAR.pdf"><img src="https://img.shields.io/badge/CN-TechnicalReport-purple"/></a> <a href="https://ieeexplore.ieee.org/document/10352967"><img src="https://img.shields.io/badge/IEEE-Paper-blue?logo=paper"/></a> <a href="https://github.com/TH-Lion/Line-based-Automatic-Calibration-of-LiDAR-and-Cameras"><img src="https://img.shields.io/github/stars/TH-Lion/Line-based-Automatic-Calibration-of-LiDAR-and-Cameras?style=social" alt="" /> </a>  

*tl;dr:* We propose an online, line-feature-based method to address extrinsic parameter drift in Camera-LiDAR systems during operation. Its real-world effectiveness was validated with industry partners (<a href="https://mad.meituan.com/">Meituan</a>, <a href="https://www.mogoauto.cn/">MOGOX</a>, and <a href="https://www.saicmotor.com/">SAIC Motor</a>).

</div>
</div>




<div class='paper-box' id='pub-tase2024'><div class='paper-box-image'><div><div class="badge">T-ASE 2024</div><img src='images/TASE2024_GFSLAM.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<p style="font-weight: bold; margin-bottom: 0.25em;"> GF-SLAM: A Novel Hybrid Localization Method Incorporating Global and Arc Features </p>

<div style="color: dimgray; font-size: 0.9em; margin-bottom: 0.25em;">
Yijin Xiong, <strong>Xinyu Zhang†</strong>, Wenju Gao, Jing Liu, <strong style="color: black; text-decoration: underline;">Qianxin Qu</strong>, Shichun Guo, Yang Shen, <strong>Jun Li†</strong>
</div>

<!-- Yijin Xiong, Xinyu Zhang†, Wenju Gao, Yuchao Wang, Jing Liu, **Qianxin Qu**, Shichun Guo, Yang Shen, Jun Li -->

<div style="color: dimgray; font-size: 0.8em; font-style: italic; margin-top: 0.25em; margin-bottom: 0.9em;">
Note: This research was initiated by <a href="https://scholar.google.com/citations?user=myxo9mQAAAAJ">Dr. Yijin Xiong</a> under the auspices of <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=0Q7pN4cAAAAJ">Prof. Xinyu Zhang</a>. I was responsible for algorithm implementation and coordinating its real-world experiment.
</div>

IEEE Transactions on Automation Science and Engineering, 2024(T-ASE, JCR Q1, IF=6.4)

<a href="https://ieeexplore.ieee.org/abstract/document/10691946"><img src="https://img.shields.io/badge/IEEE-Paper-blue?logo=paper"/></a> 

*tl;dr:* To address cumulative error in mapping for agricultural scenarios, we propose a robot localization method that fuses global and local environmental features. I was responsible for liaising with the Academy of Agricultural Sciences and implementing the real-world validation.

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
