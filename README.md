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

### 面向测地流二次守恒量的研究 Agent：Killing 张量搜索、符号验证与扰动分析

**Research Agent for Quadratic Conserved Quantities of Geodesic Flows: Killing Tensor Search, Symbolic Verification, and Perturbation Analysis**

> 开题阶段 · 《人工智能与数学》课程项目

**核心问题**：一个度量**原本具有的守恒量，在度量受到扰动之后能否继续存在？如果不能，阻碍出现在哪里？**

在黎曼或 Lorentz 流形 $(M,g)$ 上，测地流的二次守恒量 $Q=K^{ij}p_ip_j$ 与对称 **Killing 张量** $K_{ij}$（满足 $\nabla_{(i}K_{jk)}=0$）一一对应；在余切丛 $T^*M$ 上取 $H=\tfrac12 g^{ij}p_ip_j$，该条件等价于泊松括号方程 $\{Q,H\}=0$。这一等价关系使问题可以被完整地**算法化**：找到一个守恒量，回代残差为零即可确证；断言不存在，则给出线性系统不相容的代数证据。同时它又天然**需要决策**——扩大多项式次数还是更换函数基底、先做一般参数还是特殊参数、求解「卡住」是数学现象还是求解器做了不合法的参数除法、计算是否已超出预算。

本项目不做「从零发现 Kerr 的 Carter 常数」这类超出范围的事，而是把**搜索—验证—分类**做成一条可核验、可复现、可扩展的流水线，并在一个有限但明确的扰动空间内给出分类或阻碍结论。

**研究路径（三阶段）**

1. **二维模型跑通全流程** —— 在共形平坦度量族 $g_\eps=\lambda_\eps(\mathrm dx^2+\mathrm dy^2)$（$\lambda_\eps=1+x^2+2y^2+\eps x^2y^2$）上，研究 $\eps=0$ 时可分离的 Liouville 型守恒量 $Q_0$ 能否延续。首批实验（精确有理数运算，$d=2$）已给出：$\eps=0$ 时解空间维数为 **2**，而 $\eps=1$ 与 $\eps=-\tfrac14$ 时降为 **1** —— 即**可分离性在该搜索空间内丧失**。
2. **在广义相对论基准上验证工具** —— 依次通过平直空间、Schwarzschild 时空（$E,L_z,L^2,H$ 与可约性处理）、Kerr 时空（输入文献中的 Carter 常数并验证）三个基准，确认工具处理的是同一个几何问题、且适用于 Lorentz 度量，并显式面对四维的维数灾难。
3. **一阶扰动：能否把守恒量「修回来」** —— 令 $H_\eps=H_0+\eps H_1$、$Q_\eps=Q_0+\eps Q_1$，一阶守恒条件是对 $Q_1$ **线性**的方程 $\{Q_1,H_0\}=-\{Q_0,H_1\}$。在 Schwarzschild 的九参数静态轴对称扰动族上，给出存在性（显式 $Q_1$ 并回代验证）、限定范围内的不存在性（不相容的精确证据）或**参数分类**（哪些扰动允许守恒量延续）。参数分类是主要数学目标。

**方法与定位**

- **双重验证闭环**：Hamiltonian 表述 $\{Q,H\}=0$ 与几何表述 $\nabla_{(i}K_{jk)}=0$ 互相核对，自动暴露指标、符号与实现错误。
- **可约性完整化**：区分由 $g$ 及 Killing 向量对称积生成的「可约」二次守恒量与真正的隐藏对称性，使「无额外解」具有确定含义。
- **验证器优先**：基准集包含「应当找到的已知解」「重复解」「特意写错符号的候选量」「特殊参数下降秩的例子」四类样本，分别度量搜索器的漏解率与验证器的误收率。
- **Agent 的价值在策略自适应，而非「自动写代码」**：在扩次数／换基底、一般参数／特殊参数、数学现象／求解器产物、是否超预算这四类判断上做取舍，并把符号消元中的异常（例如除以 $\eps$ 而漏掉 $\eps=0$ 分支）作为一等公民管理。
- **证据包绑定结论**：每个结果都携带原始度量、候选函数空间（基底＋截断阶＋对称性假设）、生成的方程、解与参数假设、验证残差、复现命令与资源消耗；报告中的状态词（已验证解 / 限定空间内无额外解 / 一阶近似解已验证 / 未解决）预先定义、不得混用。

**技术栈**：Python + SymPy（符号线性代数、Gröbner 基），可选 EinsteinPy 辅助导入标准度量；不训练模型，第一版不做多 Agent 架构。

关键词：Killing 张量 · 二次守恒量 · 隐藏对称性 · 测地流 · 符号计算 · Agent 策略自适应

---

## 仓库

| 仓库 | 说明 |
| --- | --- |
| [denominator-weighted-shapiro-cyclic-sum](https://github.com/Delta-Y123/denominator-weighted-shapiro-cyclic-sum) | 分母加权 Shapiro 循环和：论文全文、LaTeX 源码、RBFGS 算法实现、以及经独立校验的 1349 次数值实验汇总 |
| [Codex + DeepSeek Harness 桌面宠物](https://github.com/Delta-Y123/codex-deepseek-pet/tree/main) | 一个 Windows 悬浮小挂件：实时监控 **OpenAI Codex** 和 **DeepSeek Harness** 两个 AI 编程工具的用量、额度和花费 |
