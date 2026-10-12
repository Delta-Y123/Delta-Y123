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

## 仓库

| 仓库 | 说明 |
| --- | --- |
| [denominator-weighted-shapiro-cyclic-sum](https://github.com/Delta-Y123/denominator-weighted-shapiro-cyclic-sum) | 分母加权 Shapiro 循环和：论文全文、LaTeX 源码、RBFGS 算法实现、以及经独立校验的 1349 次数值实验汇总 |
| [Codex + DeepSeek Harness 桌面宠物](https://github.com/Delta-Y123/codex-deepseek-pet/tree/main) | 一个 Windows 悬浮小挂件：实时监控 **OpenAI Codex** 和 **DeepSeek Harness** 两个 AI 编程工具的用量、额度和花费 |
