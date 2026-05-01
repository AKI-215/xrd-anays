# xrd-anays

一个独立的 Claude skill，用于通用 XRD 判相与候选相筛选。它要求先收集样品类型、主要元素、少量元素和不可能出现的元素，再进入候选相预筛或峰匹配收敛，并输出 CIF 风格的候选相卡片。

## 仓库内容

- `SKILL.md`：skill 主说明
- `data/`：候选相种子表与别名表
- `references/`：匹配流程、卡片模板、Python/绘图用法说明
- `templates/`：search-match Python 模板与通用绘图脚本
- `Structures/`：本地结构资产
- `Structures_cif/`：本地 CIF 参考资产

## 适用场景

- XRD 判相
- 候选相预筛
- 峰位收敛
- 参考 CIF/PDF 卡复核建议
- 单谱图、叠图、overlay 图辅助分析

## 使用方式

把本仓库目录作为独立 skill 放入 Claude skills 目录，或直接复用其中模板、参考文件和结构资产。

## 说明

这个 skill 把 XRD 当作晶相判断工具，而不是单独证明腐蚀机理、分层位置或局部形貌来源的证据。对于多相、弱峰、重叠峰或科研级结论，仍应结合 refinement 和其他表征方法。
