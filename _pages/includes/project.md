<style>
.carousel { position: relative; overflow: hidden; }
.carousel-track { display: flex; transition: transform 0.35s ease; }
.carousel-slide { min-width: 100%; }
.carousel-dots { text-align: center; padding: 6px 0 0; }
.carousel-dot { display: inline-block; width: 5px; height: 5px; border-radius: 50%; background: #ccc; margin: 0 3px; cursor: pointer; transition: background 0.2s; }
.carousel-dot.active { background: #555; }
</style>

# 📁 个人项目 {#personal-project}

<div class='paper-box'><div class='paper-box-image'><div>
<div class="carousel" id="carousel-1">
  <div class="carousel-track">
    <div class="carousel-slide"><img src='images/project/cloud_edge_device_sim.png' alt="云边端协同仿真平台" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/service-orchestration.png' alt="服务编排" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/request-template.png' alt="创建请求" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/simulation-controls.png' alt="仿真控制" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/results-analysis.png' alt="结果分析" width="100%"></div>
  </div>
  <div class="carousel-dots">
    <span class="carousel-dot active" onclick="goToSlide('carousel-1',0)"></span>
    <span class="carousel-dot active" onclick="goToSlide('carousel-1',1)"></span>
    <span class="carousel-dot active" onclick="goToSlide('carousel-1',2)"></span>
    <span class="carousel-dot active" onclick="goToSlide('carousel-1',3)"></span>
    <span class="carousel-dot active" onclick="goToSlide('carousel-1',4)"></span>
  </div>
</div>
</div></div>
<div class='paper-box-text' markdown="1">
**[云边端协同任务卸载仿真平台 v2.2](https://github.com/wanghuaichen2/cloud_edge_device_sim)** \\
*2026.04.20*

面向云-边-端三层异构网络的任务卸载调度仿真平台。支持自定义网络拓扑与任务 DAG 建模，为边缘计算资源管理研究提供可复现的实验环境。
- 拓扑编辑器: 支持云/边缘/终端三层异构设备自由编排
- 服务编排与任务DAG：可视化 DAG 编辑器，通用计算服务+AI推理服务自由组合
- 自定义调度算法: 内置贪心、轮询、流水线拆分三种调度器，支持自定义算法
- 模型拆分*: 当单设备放不下大模型时，搜索多设备拆分方案，功能探索阶段
- 实时可视化分析: 1秒粒度时间序列性能折线图 + 设备利用率柱状图
</div>
</div>

<script>
function goToSlide(id, index) {
  const c = document.getElementById(id);
  c.querySelector('.carousel-track').style.transform = 'translateX(-' + (index * 100) + '%)';
  c.querySelectorAll('.carousel-dot').forEach(function(d, i) {
    d.classList.toggle('active', i === index);
  });
}
</script>