# relevant_work_for_thesis：论文阅读资料

本仓库保存异步稳态视觉诱发电位（SSVEP）脑机接口方向的论文原文、阅读笔记与中英对照译文，供个人学习和研究查阅。

**论文复现代码、四个版本的实现和实验结果统一存放在 [asyn-SSVEP](https://github.com/slate-zyc/asyn-SSVEP)。** 本仓库负责文献阅读资料；两个仓库通过 README 互相链接。

## 当前文献

**Zhao et al. (2024). An EEG dataset for studying asynchronous steady-state visual evoked potential (SSVEP) based brain computer interfaces.**

- [论文 DOI](https://doi.org/10.1080/27706710.2024.2418650)
- [官方 YSU 数据集（Figshare v3）](https://doi.org/10.6084/m9.figshare.24906300.v3)
- 资料位于 [文献阅读](文献阅读/) 下对应的论文目录，包括原文 PDF、`translation/` 中的中英对照译文 PDF / LaTeX 源码与配图，以及 `文献阅读笔记/` 中的 Markdown、LaTeX 和 PDF 笔记。

译文仅供理解参考，存在歧义时以英文原文为准。原文为 CC BY 4.0 开放获取文章，使用和转载时请保留原作者署名与论文引用。

## 本地目录与编译

本地根目录保持为 `E:\deepseek_harness\relevant_work_for_thesis`，已有资料继续保存在其 `文献阅读` 子目录，不移动、不重命名。

中英对照译文 PDF 已提供章节书签，可在阅读器的书签 / 导航面板中展开。修改译文源码后，在 `translation/` 目录使用 XeLaTeX 编译；源码通过 `bookmark` 生成完整导航，并为摘要及其他无编号章节显式提供书签。需要交叉引用时仍建议编译两遍。

```powershell
xelatex -interaction=nonstopmode -halt-on-error "中英对照译文_SSVEP异步BCI数据集.tex"
xelatex -interaction=nonstopmode -halt-on-error "中英对照译文_SSVEP异步BCI数据集.tex"
```

复现实验的数据准备、运行方法、方法边界及参考算法项目，请参阅 [复现仓库 README](https://github.com/slate-zyc/asyn-SSVEP#readme)。
