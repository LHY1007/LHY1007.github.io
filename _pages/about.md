---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<html>
<head>
   <meta charset="UTF-8">
   <title>Google Translate Button with Day/Night Mode</title>
   <style>
      /* 白天模式的基本样式 */
      body {
         background-color: #fff;
         color: #000;
         transition: background-color 0.3s, color 0.3s;
      }

      /* 黑夜模式的基本样式 */
      .dark-mode {
         background-color: #111;
         color: #eee;
      }

      /* 让Google Translate按钮适配不同模式 */
      #google_translate_element {
         background-color: transparent;
         border: none;
         transition: background-color 0.3s;
      }

      /* 按钮样式 */
      button {
         position: fixed;
         top: 100px; /* 改变这个值，使按钮位置往下偏移 */
         right: 10px;
         z-index: 9999;
         background-color: #007BFF;  /* 白天模式下的按钮背景色 */
         color: white;  /* 白天模式下的按钮文字颜色 */
         border: none;
         padding: 10px 15px;
         cursor: pointer;
         border-radius: 5px;
      }

      button:hover {
         background-color: #0056b3;
      }

      /* 黑夜模式按钮样式 */
      .dark-mode button {
         background-color: #333;  /* 黑夜模式下的按钮背景色 */
         color: #fff;  /* 黑夜模式下的按钮文字颜色 */
      }

      /* Google Translate 插件的容器位置 */
      #google_translate_element {
         position: fixed;
         top: 140px; /* 改变这个值，使按钮位置往下偏移 */
         right: 10px;
         z-index: 9999;
      }
   </style>
</head>
<body>
   <!-- 切换模式按钮 -->
   <button onclick="toggleDark()">🌙 切换暗色模式</button>

   <!-- Google Translate 插件容器 -->
   <div id="google_translate_element"></div>

   <script type="text/javascript">
      // 初始化Google Translate插件
      function googleTranslateElementInit() {
         new google.translate.TranslateElement({
            pageLanguage: 'zh-CN', // 设置当前页面语言为简体中文
            includedLanguages: 'zh-CN,zh-TW,en,fr,es,ja,ko,de,ar,pt,ru', // 按所需语言顺序排列
            layout: google.translate.TranslateElement.InlineLayout.HORIZONTAL, // 横向按钮布局
            autoDisplay: false
         }, 'google_translate_element');
      }

      // 引入Google Translate脚本
      (function() {
         var script = document.createElement('script');
         script.type = 'text/javascript';
         script.src = 'https://translate.google.com/translate_a/element.js?cb=googleTranslateElementInit';
         document.body.appendChild(script);
      })();

      // 切换白天/黑夜模式的函数
      function toggleDark() {
         document.body.classList.toggle('dark-mode');
      }
   </script>
</body>
</html>




<!-- {% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %} -->

<span class='anchor' id='about-me'></span>

<h3>👋 关于我</h3>
<p style="font-size: 16px; line-height: 1.6; text-align: justify;">
  我是 <strong>东北大学（中国）</strong> 与 <strong>邓迪大学（英国）</strong> 的中英联合培养本科生，当前正在苏格兰邓迪进行本科第四年的学习。
</p>

<p style="font-size: 16px; line-height: 1.6; margin-top: 10px;">
  我的研究兴趣包括：
</p>

<ul style="font-size: 16px; line-height: 1.6; margin-left: 20px;">
  <li>🤖 人工智能（AI）</li>
  <li>🧬 智能影像组学（Intelligent Radiomics）</li>
  <li>🧠 神经科学（Neuroscience）</li>
  <li>🏃‍♂️ 活动识别（Activity Recognition）</li>
  <li>💓 医学生理信号分析（Biomedical Signal Processing）</li>
</ul>

  
 <!-- <a href='https://scholar.google.com/citations?user=5sOyw0IAAAAJ&hl'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=引用"></a>。 -->

<span class='anchor' id='-xl'></span>

<h3>🎓 学历</h3>

<div style="display: flex; align-items: flex-end; margin-bottom: 8px;">
  <span>
    <em>2021.09 - 2025.06</em>, 东北大学 医学与生物信息工程学院, 辽宁沈阳, 本科
  </span>
  <img class="svg" src="/images/NEU_logo.png" width="130pt" style="margin-left: 18px;">
</div>

<div style="display: flex; align-items: flex-end;">
  <span>
    <em>2021.09 - 2025.06</em>, 邓迪大学 科学与工程学院, 苏格兰邓迪, 荣誉本科
  </span>
  <img class="svg" src="/images/UoD_logo.svg" width="90pt" style="margin-left: 40px;">
</div>

 
<span class='anchor' id='-xscg'></span>

# 📝 学术成果

<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Publications</title>
  <style>
    .publications-container {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      max-width: 800px;
      margin: 0 auto;
    }
    
    .publication-item {
      border: 1px solid #e0e0e0;
      border-radius: 8px;
      margin-bottom: 16px;
      box-shadow: 0 1px 3px rgba(0,0,0,0.1);
      transition: box-shadow 0.3s ease;
    }
    
    .publication-item:hover {
      box-shadow: 0 3px 6px rgba(0,0,0,0.15);
    }
    
    .publication-header {
      padding: 16px;
      cursor: pointer;
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
    }
    
    .publication-citation {
      margin: 0;
      line-height: 1.5;
    }
    
    .publication-links {
      margin-top: 8px;
    }
    
    .publication-links a {
      color: #0366d6;
      text-decoration: none;
      margin-right: 12px;
      font-size: 14px;
    }
    
    .publication-links a:hover {
      text-decoration: underline;
    }
    
    .publication-toggle {
      color: #767676;
      flex-shrink: 0;
      margin-left: 12px;
    }
    
    .publication-detail {
      padding: 16px;
      background-color: #f7f7f7;
      border-top: 1px solid #e0e0e0;
      display: none;
    }
    
    .publication-detail h4 {
      margin-top: 0;
      margin-bottom: 8px;
      font-weight: 500;
    }
    
    .publication-detail p {
      margin: 0;
      font-size: 14px;
      color: #444;
      line-height: 1.5;
    }
    
    .highlight {
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="publications-container">
    <h3 style="font-size: 1.25rem; font-weight: bold; margin-bottom: 1rem;">已发表论文</h3>
    
    <!-- Publication 1 -->
    <div class="publication-item">
      <div class="publication-header" onclick="toggleDetail(this)">
        <div>
          <p class="publication-citation">Wang, X.¹, <span class="highlight">Liu, H.</span>¹, Zhang, Y., Zhao, B., Duan, H., Hu, W., ... & Li, C. (2025). Joint Modelling Histology and Molecular Markers for Cancer Classification. Medical Image Analysis, 102(4): 103505.</p>
          <div class="publication-links">
            <a href="https://www.sciencedirect.com/science/article/pii/S1361841525000532">[网页]</a>
            <a href="https://arxiv.org/pdf/2502.07979">[预览]</a>
            <a href="/paper/MedIA2024.pdf"  download>[下载]</a>

          </div>
        </div>
        <div class="publication-toggle">▼</div>
      </div>
      <div class="publication-detail">
        <h4>论文简介</h4>
        <p>This paper introduces a novel approach for cancer classification by integrating histological images with molecular marker data. The proposed model utilizes a multi-modal deep learning architecture to effectively combine features from different data sources, resulting in improved diagnostic accuracy compared to single-modality methods. Our framework demonstrates significant performance improvements across multiple cancer types and provides interpretable results that can aid clinicians in treatment planning.</p>
      </div>
    </div>
    
    <!-- Publication 2 -->
    <div class="publication-item">
      <div class="publication-header" onclick="toggleDetail(this)">
        <div>
          <p class="publication-citation"><span class="highlight">Liu, H.</span>¹, Wang, Z.*,¹, Zhao, B., Shen, Q., Li, M., Que, N., ... & Xin, J.* (2024, August). Multi-scale context-aware networks based on fragment association for human activity recognition. In Proceedings of the Thirty-Third International Joint Conference on Artificial Intelligence (pp. 3169-3177).</p>
          <div class="publication-links">
            <a href="https://www.ijcai.org/proceedings/2024/351">[网页]</a>
            <a href="https://www.ijcai.org/proceedings/2024/0351.pdf">[预览]</a>
            <a href="/paper/IJCAI2024.pdf"  download>[下载]</a>
          </div>
        </div>
        <div class="publication-toggle">▼</div>
      </div>
      <div class="publication-detail">
        <h4>论文简介</h4>
        <p>This work presents a novel approach to human activity recognition through multi-scale context-aware networks. We introduce a fragment association mechanism that enables the model to capture temporal relationships across different time scales. Our method achieves state-of-the-art performance on multiple benchmark datasets by effectively modeling both local and global temporal patterns in sensor data, leading to more robust recognition of complex human activities.</p>
      </div>
    </div>
    
    <!-- Publication 3 -->
    <div class="publication-item">
      <div class="publication-header" onclick="toggleDetail(this)">
        <div>
          <p class="publication-citation"><span class="highlight">Liu, H.</span>¹, Zhao, B.¹, Dai, C., Sun, B., Li, A., & Wang, Z* (2023). MAG-Res2Net: A novel deep learning network for human activity recognition. Physiological Measurement, 44(11), 115007.</p>
          <div class="publication-links">
            <a href="https://iopscience.iop.org/article/10.1088/1361-6579/ad0ab8/meta">[网页]</a>
            <a href="https://iopscience.iop.org/article/10.1088/1361-6579/ad0ab8/pdf">[预览]</a>
            <a href="/paper/PMEA2023.pdf"  download>[下载]</a>
          </div>
        </div>
        <div class="publication-toggle">▼</div>
      </div>
      <div class="publication-detail">
        <h4>论文简介</h4>
        <p>In this paper, we propose MAG-Res2Net, an innovative deep learning architecture specifically designed for human activity recognition using wearable sensor data. Our network combines multi-attention gating mechanisms with a hierarchical residual structure to capture both fine-grained motion details and high-level activity patterns. Extensive experiments demonstrate that MAG-Res2Net outperforms existing methods, particularly for complex activities and in challenging real-world scenarios with noise and variability.</p>
      </div>
    </div>
  </div>

  <script>
    function toggleDetail(element) {
      // 获取论文详情区域
      const detail = element.parentNode.querySelector('.publication-detail');
      const toggle = element.querySelector('.publication-toggle');
      
      // 切换详情区域显示状态
      if (detail.style.display === 'block') {
        detail.style.display = 'none';
        toggle.textContent = '▼';
      } else {
        detail.style.display = 'block';
        toggle.textContent = '▲';
      }
    }
  </script>
</body>
</html>

---
### 在投论文

- Tang H^1^, `Liu, H.*`^1^, Li C. (2025). FOD-Diff: 3D Multi-Channel Patch Diffusion Model for Fiber Orientation Distribution. MICCAI2025

- `Liu, H.*`, Li, X.^1^, Jiang, Y.^1^, Tang, H., Wu, D., & Guo, Y. (2025). Redundant feature screening method for human activity recognition based on attention purification mechanism. arXiv preprint arXiv:2503.23537.
[[网页]](https://arxiv.org/abs/2503.23537) [[预览]](https://arxiv.org/pdf/2503.23537) <a href="/paper/submit1.pdf" download>[[下载]]</a>

- `Liu, H.*`,  Li, S.^1^, Yu, Y.^1^, Jiang, Y., Xiao, H., Long, J., & Tang, H. (2025). CMD-HAR: Cross-Modal Disentanglement for Wearable Human Activity Recognition. arXiv preprint arXiv:2503.21843.
[[网页]](https://arxiv.org/abs/2503.21843) [[预览]](https://arxiv.org/pdf/2503.21843) <a href="/paper/submit2.pdf" download>[[下载]]</a>

- Yu Y.^1^, Wang H., Wang J., Yan M., Han X., Wu D., Zhao X., `Liu, H.*`.(2024). Optimizing End-to-End Sensor-Based Human Activity Recognition Through Multi-Attention Interaction.
[[网页]](http://dx.doi.org/10.2139/ssrn.4777248) [[预览]](https://download.ssrn.com/eaai/a82c853c-7bba-4b08-a2aa-a7e46d848f71-meca.pdf?response-content-disposition=inline&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEB0aCXVzLWVhc3QtMSJHMEUCIEdqTqH9q5j68yOtSNvmrsi2gqCVfFCa1HEJR1QT6gzFAiEAl79kD11aAyzDXZ0gi0ZSQd03YdrFSr3usrchgrLNGMIqxwUIlv%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAEGgwzMDg0NzUzMDEyNTciDBo16dv9IkhB%2BwB5nSqbBTOZ2Y7FH8HUBrd2fwShDNFKTx%2F8S186kRw8GoYTaV6YwmrlTnZQ%2Bpq59PnnAuC8RJ2WwDUdpIi2jeuy7AFAVGqXDv%2FAcenwnnmhBfib2ifmuCNfY8OUcH8fHBvkp4lJwZIQGudSEGKwL%2FXaqj97efimGbLT2Ym2feaDuAy60SM8kdlIlh7UIyaXs7%2FNMV9JPOYzFGTRoekL9qocorlVuPhP%2Bu%2B5sfHNj7byoyJ6uo92AOK2XJB%2BXDeA5yJiqDrJ8njZ5DogJscyh2p8NF4Y3PmKgrzKcUYb0D8VOfV3WVNPhD7kz3B%2BupnlHv9AiQLNuIvsjKzl3N7o6DwN5RfQc0FUM%2FhiyJgcNwuuc6OoTiMajQTjE4jFO2Ld4UEbFNgPBkWyIxeV8ZrGHUSHdJbdlU6b0vPEQKN8EEDlC%2BNg4zleoN%2FgRxcdWR0wW9hpjFuBz2ZwJJTfFAydwfYHGxobzfuAwT4VdUuWREBQXWu6OjLzPeDK6lS51EFmIe86Heqg81oCCQmYs0U6mg%2BZC%2BRmAOUFnSrsun97Rrpe0kshk1AjCh7nA%2Fo3HIgq1PnQ8G4ssB1cg0ysPw558EzhrD2gab%2BaCXrzEBkOkzb1xneHAoFAf%2BlrQf3hIKyC7sZLtNR3BNNeeGvvMkTRkgKX1Lpg7ebAmU4FRLrRmENOT5zkjrSN1%2Fzpqclmr9jblZTFf1tbklOXPsLTT%2BZCAMVQuQe1RTz%2BYDceUym1rdWElJyxS2kKtr0RV5wRKHRdCfnF4PJRgmm4qTN2OLpc3PBMj3qSo4N7jfEQPX2WVXKzG4gfLUpBdaaRIJ5ceI%2Ff9mIeYl0DJvGCEy2rJuckv3NZrUVay1%2FpIsem4y0bpY8vGUZZyGLNloNgZ042FxNWTA8w%2Fr3bvwY6sQHVfX96i89YmH%2BO5KMGjakO%2Buz6CDzrZFxRo%2BqjEAwqfT6IB5M5cDe86OijOjHDbjg%2FmFJP3AYvrH53gIiU%2FAFaJhApOFyobA3mC3GfnUG6sMMq0r2Z1rQT0OxcVPfAvYsBGbmxqKhu%2FUtnQtJk1DBhD3wyX8YkQ1AF%2F2C733xQrWoqbWvxj5njfcrL5EiuoBxr8W9tMcXAHsoPVIMMVLeCWlCAldKgN%2BEZIk9FsZdAkfA%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20250409T214847Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAUPUUPRWEYIZAGPIX%2F20250409%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=62a3e491cc76e6077650d885d9f6d6ecd220b1f82666e47149750599e1b1d0b5&abstractId=4777248) <a href="/paper/submit3.pdf" download>[[下载]]</a>

### 学术服务
- AAAI2024 会议审稿
- IJCAI2024 会议审稿
- MICCAI2025 会议审稿
- 为MICCAI-CMMCA2025大会提供技术支持 [[网页]](https://miccai-workshop.github.io/CMMCA2025/)
- IEEE Transactions on Industrial Informatics 期刊审稿人
- Engineering Applications of Artificial Intelligence 期刊审稿人

### 专利
- `刘涵瑜`, 赵伯阳, 王之琼. 基于多尺度度量学习的人类活动识别综合优化方法. （已受理）
  
### 软件著作权
-  赵伯阳, `刘涵瑜`, 王之琼. 基于多尺度神经网络的动作识别系统V1.0.（已受理）

<span class='anchor' id='-kyxm'></span>

<h3>💻 科研项目</h3>

<div style="display: flex; flex-direction: column; gap: 10px; font-size: 15px;">
  <div style="padding: 10px; border: 1px solid #ccc; border-radius: 10px;">
    <strong>空间转录组学研究</strong><br>
    <em>2024.09 - Now</em><br>
    剑桥大学 | 临床医学院 - 临床神经科学系（英国剑桥）
  </div>

  <div style="padding: 10px; border: 1px solid #ccc; border-radius: 10px;">
    <strong>弥散胶质瘤研究</strong><br>
    <em>2024.04 - 2025.01</em><br>
    剑桥大学 | 数学院 - 应用数学与理论物理系（英国剑桥）
  </div>

  <div style="padding: 10px; border: 1px solid #ccc; border-radius: 10px;">
    <strong>化工异常检测与故障诊断</strong><br>
    <em>2023.12 - 2025.03</em><br>
    东北大学 | 信息科学与工程学院（辽宁沈阳）
  </div>

  <div style="padding: 10px; border: 1px solid #ccc; border-radius: 10px;">
    <strong>低质量多模态生理信号数据分析</strong><br>
    <em>2023.07 - 2024.04</em><br>
    东北大学 | 医学与生物信息工程学院 & 计算机科学与工程学院（辽宁沈阳）
  </div>

  <div style="padding: 10px; border: 1px solid #ccc; border-radius: 10px;">
    <strong>人体活动识别研究</strong><br>
    <em>2022.10 - 2023.04</em><br>
    东北大学 | 医工学院（辽宁沈阳）
  </div>
</div>

<span class='anchor' id='-ryjx'></span>

<h3>🏅 荣誉奖项</h3> 
- *2024.8* 获得 中国大学生计算机博弈大赛——第十八届中国计算机博弈锦标赛 `一等奖`  
- *2024.4* 获得 中国国家大学生创新设计训练计划项目 `专业第一名, 国家级优秀结题`  
- *2023.8* 获得 中国大学生生物医学工程创新设计大赛 `第一名, 二等奖` 
- *2023.8* 获得 中国大学生计算机博弈大赛——第十七届中国计算机博弈锦标赛 `二等奖`  


<span class='anchor' id='-xshy'></span>

<h3>🏅 学术会议</h3> 
- *2024.8*, International Joint Conferences on Artificial Intelligence, 韩国济州岛, 受邀报告

<!-- <span class='anchor' id='-gzsx'></span> -->


<!-- <div class='paper-box'><div class='paper-box-image'><div><div class="badge">Sens. Actuators Phys. 2021</div><img src='images/IJCAI2025.svg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

-	`Jian Tang`, Rongbiao Wang, Bocheng Liu, Yihua Kang. A novel magnetic flux leakage method based on the ferromagnetic lift-off layer with through groove. *Sensors and Actuators A: Physical*. 2021: 113091. (JCR:Q1; IF:4.291)  
[[网页]](https://dx.doi.org/10.1016/j.sna.2021.113091) [[预览]](https://github.com/tangjyan/tangjyan.github.io/blob/main/pdf/TangJ-2021-A%20novel%20magnetic%20flux%20leakage%20method%20based%20on%20the%20ferromagnetic%20lift-off%20layer.pdf) [[下载]](/pdf/TangJ-2021-A%20novel%20magnetic%20flux%20leakage%20method%20based%20on%20the%20ferromagnetic%20lift-off%20layer.pdf)

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Int. J. Appl. Electrom. 2020</div><img src='images/PMEA.svg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

-	`Jian Tang`, Rongbiao Wang, Jikai Zhang, Yihua Kang. The influence of magnetic head’s pose on magnetic flux leakage detection. *International Journal of Applied Electromagnetics and Mechanics*. 2020, 64(1–4): 493–500. (JCR:Q4; IF:0.536)  
[[网页]](https://dx.doi.org/10.3233/JAE-209356) [[预览]](https://github.com/tangjyan/tangjyan.github.io/blob/main/pdf/TangJ-2020-The%20influence%20of%20magnetic%20head%E2%80%99s%20pose%20on%20magnetic%20flux%20leakage%20detection.pdf) [[下载]](/pdf/TangJ-2020-The%20influence%20of%20magnetic%20head%E2%80%99s%20pose%20on%20magnetic%20flux%20leakage%20detection.pdf)

</div>
</div> -->
