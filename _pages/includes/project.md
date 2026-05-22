<style>
.carousel { position: relative; overflow: hidden; }
.carousel-track { display: flex; transition: transform 0.35s ease; }
.carousel-slide { min-width: 100%; }
.carousel-dots { text-align: center; padding: 6px 0 0; }
.carousel-dot { display: inline-block; width: 5px; height: 5px; border-radius: 50%; background: #ccc; margin: 0 3px; cursor: pointer; transition: background 0.2s; }
.carousel-dot.active { background: #555; }
#carousel-2 .carousel-slide { aspect-ratio: 1920 / 1040; background: #f8f8f8; }
#carousel-2 .carousel-slide a { display: block; width: 100%; height: 100%; }
#carousel-2 .carousel-slide img { display: block; width: 100%; height: 100%; object-fit: cover; }
</style>

# 📁 个人项目 {#personal-project}

<div class='paper-box'><div class='paper-box-image'><div>
<div class="carousel" id="carousel-1">
  <div class="carousel-track">
    <div class="carousel-slide"><img src='images/project/cloud_edge_device_sim/cloud_edge_device_sim.png' alt="云边端协同仿真平台" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/cloud_edge_device_sim/service-orchestration.png' alt="服务编排" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/cloud_edge_device_sim/request-template.png' alt="创建请求" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/cloud_edge_device_sim/simulation-controls.png' alt="仿真控制" width="100%"></div>
    <div class="carousel-slide"><img src='images/project/cloud_edge_device_sim/results-analysis.png' alt="结果分析" width="100%"></div>
  </div>
  <div class="carousel-dots">
    <span class="carousel-dot active" onclick="goToSlide('carousel-1',0)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-1',1)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-1',2)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-1',3)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-1',4)"></span>
  </div>
</div>
</div></div>
<div class='paper-box-text' markdown="1">
**[云边端协同任务卸载仿真平台 v2.2](https://github.com/wanghuaichen2/cloud_edge_device_sim)** \\
*2025.04.20*

面向云-边-端三层异构网络的任务卸载调度仿真平台。支持自定义网络拓扑与任务 DAG 建模，为边缘计算资源管理研究提供可复现的实验环境。
- 拓扑编辑器: 支持云/边缘/终端三层异构设备自由编排
- 服务编排与任务DAG：可视化 DAG 编辑器，通用计算服务+AI推理服务自由组合
- 自定义调度算法: 内置贪心、轮询、流水线拆分三种调度器，支持自定义算法
- 模型拆分*: 当单设备放不下大模型时，搜索多设备拆分方案，功能探索阶段
- 实时可视化分析: 1秒粒度时间序列性能折线图 + 设备利用率柱状图
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div>
<div class="carousel" id="carousel-2">
  <div class="carousel-track">
    <div class="carousel-slide"><a href='images/project/crown_2d_3d/laplacian_side_by_side.png' target="_blank"><img src='images/project/crown_2d_3d/laplacian_side_by_side.png' alt="Laplacian对比" width="100%"></a></div>
    <div class="carousel-slide"><a href='images/project/crown_2d_3d/pred_crown.png' target="_blank"><img src='images/project/crown_2d_3d/pred_crown.png' alt="预测牙冠" width="100%"></a></div>
    <div class="carousel-slide"><a href='images/project/crown_2d_3d/pred_crown_view.gif' target="_blank"><img src='images/project/crown_2d_3d/pred_crown_view.gif' alt="旋转展示" width="100%"></a></div>
    <div class="carousel-slide"><a href='images/project/crown_2d_3d/main_workflow.svg' target="_blank"><img src='images/project/crown_2d_3d/main_workflow.svg' alt="端到端主流程" width="100%"></a></div>
    <div class="carousel-slide"><a href='images/project/crown_2d_3d/run_log.png' target="_blank"><img src='images/project/crown_2d_3d/run_log.png' alt="训练日志" width="100%"></a></div>
  </div>
  <div class="carousel-dots">
    <span class="carousel-dot active" onclick="goToSlide('carousel-2',0)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-2',1)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-2',2)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-2',3)"></span>
    <span class="carousel-dot" onclick="goToSlide('carousel-2',4)"></span>
  </div>
</div>
</div></div>
<div class='paper-box-text' markdown="1">
**[3D牙冠自动生成 Crown 3D ↔ 2D v6.0](https://github.com/wanghuaichen2/Crown_3D_2D-pub)** \\
*2026.05.22*

将 3D 牙冠设计转化为 2D 球面图像回归问题：以 Attention U-Net + PatchGAN 预测全局径向距离图，再还原为 3D 网格。
- 球面投影: 以牙冠质心为球心，牙冠/基牙/对颌 → 2D 径向距离图，将 3D 设计转化为 2D 回归
- Attention U-Net + PatchGAN: 注意力机制聚焦牙冠关键区域，对抗训练增强边缘与曲面细节
- 颌面监督: 局部正交投影辅助监督，显著提升咬合面窝沟形态精度
- 推理模式: 支持 PLY 直推 / 球面三角化 / 泊松重建三种 3D 还原方式
- 临床验证: 5000 例 46 牙数据训练，近远中/颊舌侧合格率 95%↑，颌面合格率 80%↑（100 例医师评测）
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