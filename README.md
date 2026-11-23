### 王安蕲 · Anqi Wang

同济大学数学科学学院 · School of Mathematical Sciences, Tongji University

---

## 研究成果

### 分母加权 Shapiro 循环和的研究与高效求解算法

**Research on the Denominator-Weighted Shapiro Cyclic Sum and Efficient Solution Algorithms**

Shapiro 循环不等式自 1954 年提出后历经三十余年，才由 Troesch 完全解决。本工作研究其分母加权推广

$$F(x,p)=\sum_{i=1}^{n}\frac{x_i}{p\,x_{i+1}+q\,x_{i+2}},\qquad p+q=1,\qquad 0\le p\le 1$$

的极值性质与高效求解算法。

**主要贡献**

- 把 Bushell–Ando 关于极小点的结构定理推广到分母加权情形，刻画了极小点的分段结构、比例关系与零位模式
- 将最小值 $P(n,p)=\min_{x}F(x,p)$ 的计算归结为求解**有限个二元多项式方程组**，并给出可行域 $UV_p$ 的显式描述
- 提出单位球面 $\mathbb{S}^{n-1}$ 上的**黎曼 BFGS 算法**，带振荡解检测与扰动重启机制
- 证明：对一切 $n\ge 3$，当 $\dfrac{\sqrt5-1}{2}\le p\le 1$ 时 $P(n,p)=n$

**链接**

- 📦 [代码与论文仓库](https://github.com/Delta-Y123/denominator-weighted-shapiro-cyclic-sum)
- 📄 [论文全文 (PDF, English)](https://github.com/Delta-Y123/denominator-weighted-shapiro-cyclic-sum/blob/main/paper/Denominator-Weighted-Shapiro-Cyclic-Sum.pdf)
- 🧾 [中文版论文](https://github.com/Delta-Y123/denominator-weighted-shapiro-cyclic-sum/blob/main/paper/Denominator-Weighted-Shapiro-Cyclic-Sum-CN.pdf)
- 🔖 [代码归档 (Zenodo, doi:10.5281/zenodo.19228120)](https://doi.org/10.5281/zenodo.19228120)

关键词：Shapiro inequality · Shapiro cyclic sum · Riemannian BFGS algorithm · minimizer analysis

<sub>本工作受同济大学大学生创新训练计划（SITP）资助，项目编号 X2025634。</sub>

---

## 开发成果

### Codex + DeepSeek Harness 桌面宠物

一个 Windows 悬浮小挂件：把 **OpenAI Codex** 和 **DeepSeek Harness** 两个 AI 编程工具
的用量、额度和花费并排放在桌面指定角落里，两行、可调的透明背景、几乎不占地方。

```
● Codex     gpt-5.6-sol   5h 100% · 7d 99%     0 tok · $0.00
● DeepSeek  v4-pro        余额 ¥6.90          62.3M tok · ¥23.35
```

**状态灯**：🟢 工作中　⚪ 休息中　🔴 未运行

## 在研项目

### 面向测地流二次守恒量的研究 Agent
本项目围绕“度量受到扰动后，二次测地流守恒量能否延续”这一问题，开发一个用于搜索与验证 Killing 张量的研究 Agent。项目将从二维可分离度量出发，逐步验证平直时空、Schwarzschild 与 Kerr 时空中的已知守恒量，再研究限定扰动族中的一阶守恒量延续问题。Agent 将调用符号计算工具生成并求解方程、回代检验候选结果，并记录计算所依赖的函数空间与参数条件。项目目标是形成可重复的计算流程和范围明确的数学结论，同时探索 Agent 如何辅助几何问题中的实验与验证。

### Syzygy：多智能体数学研究工作台

**Syzygy — A Multi-Agent Framework for Mathematical Research**

一个在本机运行的数学研究工作台。导入任务书后，主 Agent 规划 1–6 条研究路线（正反问题由程序保证同时保留正向证明与反向检验），文献 Agent 检索并阅读公开资料，各 Worker 独立推进证明或反例；Verifier 依据主 Agent 拆出的核验义务与依赖 DAG 做分项检查，再独立完成整体审查，通过验收的结果才进入事实图，最后交由论文 Agent 分节写作、定向修订并调用本地 XeLaTeX 生成论文。

面向需要多条路线、反复修订与长时间续跑的数学研究：每个 Agent 可单独选择模型与推理强度，运行中可注入四类提示（补充线索、补充信息、研究建议、调整方向），可单独暂停某条路线，也能从本地检查点继续。核验支持增量复用——仅当原文、义务、假设、依赖与上下文签名全部匹配时才复用旧证据。仓库附带 12 个任务书范例与一份格式模板（Kerr 潮汐与 Carter 常数、环面可积性、非凸优化、正特征代数几何、表示论、graphon 等），并公开了一次完整运行的耗时报告（自然跨度 46 小时 17 分，2 503 次 API 请求）。

服务与前端仅使用 Python 标准库和原生 HTML/CSS/JavaScript，无需第三方依赖或 Node.js。需要说明的是，模型核验是可供人工追溯的研究审阅，不构成形式化证明证书。

---

## 仓库

| 仓库 | 说明 |
| --- | --- |
| [分母加权 Shapiro 循环和的研究与高效求解算法](https://github.com/Delta-Y123/denominator-weighted-shapiro-cyclic-sum) | 分母加权 Shapiro 循环和：论文全文、LaTeX 源码、RBFGS 算法实现、以及经独立校验的 1349 次数值实验汇总 |
| [Codex + DeepSeek Harness 桌面宠物](https://github.com/Delta-Y123/codex-deepseek-pet/tree/main) | 一个 Windows 悬浮小挂件：实时监控 **OpenAI Codex** 和 **DeepSeek Harness** 两个 AI 编程工具的用量、额度和花费 |
| [面向测地流二次守恒量的研究 Agent：Killing 张量搜索、符号验证与扰动分析](https://github.com/Delta-Y123/Research-Agent-for-Quadratic-Conserved-Quantities-of-Geodesic-Flows/tree/main) | 构建结合符号计算与实验决策的研究 Agent，搜索并验证测地流的二次守恒量，研究已知守恒量在度量扰动下能否延续。 |
| [Syzygy：多智能体数学研究工作台](https://github.com/Delta-Y123/Syzygy/tree/main) | 本机运行的多智能体数学研究框架：主 Agent 规划路线、Worker 独立推进证明、Verifier 分项核验后进入事实图，最后由论文 Agent 生成 LaTeX/PDF；附 12 个任务书范例 |
| [同济图书馆座位监控](https://github.com/Delta-Y123/SeatWatch) | 一个帮你“盯座位”的安卓 App |
