# UniCoD: 通过统一连续和离散表示学习增强机器人策略

这是UniCoD项目的官方网站，基于论文《UniCoD: Enhancing Robot Policy via Unified Continuous and Discrete Representation Learning》构建。

## 项目概述

UniCoD是一个统一的机器人学习框架，遵循理解-生成-执行的范式，将离散任务理解与连续未来机器人状态预测相结合。

### 主要贡献

1. **统一表示学习**: 提出了一个统一的视觉-语言-动作(VLA)预训练框架，集成了离散和连续表示。

2. **两阶段训练策略**: 设计了一个两阶段训练策略，在保持原始预训练模型能力的同时实现动作表示对齐。

3. **最先进性能**: 我们的最佳模型在仿真和真实世界环境中都实现了最先进的结果。

## 技术架构

- **Mix-of-Transformers架构**: 采用模态专用专家模块
- **两阶段训练**:
  - 第一阶段: 跨实体操作数据的视觉-语言预测
  - 第二阶段: 实体特定的动作学习
- **连续和离散表示**: 统一处理不同类型的表示

## 实验结果

- **SimplerEnv-WindowX**: 71.0% 成功率
- **SimplerEnv-Google Robot**: 78.4% 成功率  
- **Calvin ABC-D**: 超越所有基线方法
- **真实世界部署**: 在Franka机械臂和XArm灵巧手上验证

## 文件结构

```
├── index.html                 # 主页面
├── pi0_dino_pred.pdf         # 论文PDF
├── media/
│   ├── images/               # 图片资源
│   └── videos/               # 视频资源
├── static/                   # 静态资源
└── pi0_dino_pred/           # LaTeX源码和图片
```

## 使用方法

1. 在浏览器中打开 `index.html` 查看项目主页
2. 点击"论文 PDF"按钮阅读完整论文
3. 浏览不同部分了解方法和实验结果

## 引用

如果您使用了我们的工作，请引用：

```bibtex
@article{unicod2026,
  title={UniCoD: Enhancing Robot Policy via Unified Continuous and Discrete Representation Learning},
  author={Hippocampus, Antiquus S. and Cerebro, Natalia and Amygdale, Amelie P. and Ren, Ji Q. and LeNet, Yevgeny},
  journal={ICLR},
  year={2026}
}
```
