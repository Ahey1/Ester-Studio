# Ester Studio 实算图例和结构来源

[返回 Ester Studio 首页](../README.md)

三维结构和等值面由 Ester Studio 的视口及原生导出组件生成。等值面外观与散点配色采用 2.1.2 启动默认设置。结构展示使用各自标出的预设。软件界面截图来自 2.1.2 Windows x64 正式便携包。

## 多巴胺

起始几何为 [PubChem CID 681](https://pubchem.ncbi.nlm.nih.gov/compound/681) 的 3D 构象。取气相中性单重态，以 GFN2-xTB 6.8.0 优化，13 步收敛。对收敛结构单点，导出 Molden 波函数。Multiwfn 2026.10.18 计算前线轨道、电子密度和静电势格点。

- HOMO 和 LUMO 分别为轨道 30 和 31，轨道等值为 ±0.030 bohr⁻³ᐟ²。
- 电子密度图与静电势图的表面为 ρ = 0.001 e/bohr³。静电势采用原子单位。
- 优化曲线使用 xTB 输出的 13 个能量点，并以最后一步能量为零点。点线样式采用 ES 空心预设。

## 面对面苯二聚体

从 [S66 第 24 例](https://doi.org/10.1021/ct2002946) 的错位平行构型起步。GFN2-xTB 优化后，层间距为 3.3045 Å，面内错位为 1.2159 Å。两个片段分别对应原子 1–12 与 13–24。

IRI 与 IGMH 使用同一份 GFN2-xTB 波函数，格距 0.20 Bohr。IRI 等值为 1.0，片段间 IGMH δg 等值为 0.0015 a.u.。三维表面和散点按 sign(λ₂)ρ 着色。散点取自同次计算的一一配对格点，按科研图的显示窗口取景。

## 水笼

自建十二面体外层水笼并放入中央水，得到气相中性单重态 (H₂O)₂₁ 起始结构。用 GFN2-xTB 优化后，中央氧到最近四个外层氧的距离为 2.64–2.71 Å。中央 1 个水与外层 20 个水共同参与 Hirshfeld 分析。

Hirshfeld 表面使用中央水权重 0.5，格距 0.15 Bohr，以 dₙₒᵣₘ 着色。指纹图由同一次 Multiwfn 计算的 8,927 对 dᵢ 和 dₑ 值绘制。颜色表示 0.02 Å 邻域内的点数，总接触面积为 39.055 Å²。

## 其他分子与晶体

| 图例 | 结构来源与显示条件 |
| --- | --- |
| 咖啡因 | [PubChem CID 2519](https://pubchem.ncbi.nlm.nih.gov/compound/2519) 的 3D 构象 |
| 18-冠-6 | [PubChem CID 28557](https://pubchem.ncbi.nlm.nih.gov/compound/28557) 的 3D 构象 |
| 金刚烷 | [PubChem CID 9238](https://pubchem.ncbi.nlm.nih.gov/compound/9238) 的 3D 构象 |
| Trp-cage | [PDB 1L2Y](https://www.rcsb.org/structure/1L2Y) 第一套 NMR 构型的 154 个重原子 |
| 岩盐型 NaCl | 晶格常数 5.6402 Å 的标准岩盐单胞，2×2×2 超胞 |
| 金刚石 | [COD 9008564](https://www.crystallography.net/cod/9008564.html)，2×2×2 超胞 |
| 立方 BaTiO₃ | [COD 2100862](https://www.crystallography.net/cod/2100862.html)，2×2×2 超胞并显示 Ti–O 配位 |
| Cu(111) | 由 [COD 9008468](https://www.crystallography.net/cod/9008468.html) 的 fcc 晶格参数构造的 4×4 四层表面模型 |

晶体资料使用 [Crystallography Open Database](https://www.crystallography.net/cod/) 的 CC0 坐标。超胞在原晶格上重复。周期连接表示按邻近距离构建的结构显示。

## 方法

[GFN2-xTB](https://doi.org/10.1021/acs.jctc.8b01176) · [Multiwfn](https://doi.org/10.1002/jcc.22885) · [IRI](https://doi.org/10.1002/cmtd.202100007) · [IGMH](https://doi.org/10.1002/jcc.26812) · [Hirshfeld 表面](https://doi.org/10.1039/B818330A)
