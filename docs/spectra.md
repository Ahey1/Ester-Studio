# Ester Studio 光谱图集与数据来源

[返回仓库光谱图集](../README.md#光谱图集)

图集展示 Ester Studio 2.1.2 对 Gaussian 和 ORCA 计算输出的后处理。曲线使用 ES 的光谱样式，渐变填色和柱图使用其对应的绘图设置。

## 展宽与强度

- **紫外吸收**使用高斯展宽，半高全宽为 0.24 eV。波长图的横轴由激发能换算，展宽在能量域计算。
- **红外**使用洛伦兹展宽，半高全宽为 20 cm⁻¹。柱图所用的原始积分强度以 km/mol 计。
- **拉曼**使用洛伦兹展宽，半高全宽为 20 cm⁻¹。Stokes 谱的激光波长为 532 nm，温度为 298.15 K。各曲线按对应全谱的最大值归一化，局部图沿用同一归一化基准。
- **柱图**展示原始振子强度、红外积分强度或拉曼活性。拉曼活性的单位为 Å⁴/amu。

## 计算来源

| 体系 | 程序与计算级别 | 对应图号 | 来源 |
| --- | --- | --- | --- |
| 二乙烯基苯 | Gaussian 09 · TD-B3LYP/STO-3G | S01、S02、S03、S04、S05 | [cclib-data 原始日志](https://github.com/cclib/cclib-data/blob/0103b6867ce7d6a3f719fe2e757ee3eb95cd5268/Gaussian/Gaussian09/dvb_td_revA.02.out) |
| 二乙烯基苯 | ORCA 4.2 · TDA-B3LYP/STO-3G | S06、S07 | [cclib-data 原始日志](https://github.com/cclib/cclib-data/blob/0103b6867ce7d6a3f719fe2e757ee3eb95cd5268/ORCA/ORCA4.2/dvb_td.out) |
| 二乙烯基苯 | Gaussian 09 · B3LYP/STO-3G | S08、S09、S10、S13 | [cclib-data 原始日志](https://github.com/cclib/cclib-data/blob/0103b6867ce7d6a3f719fe2e757ee3eb95cd5268/Gaussian/Gaussian09/dvb_ir_revA.02.out) |
| 水 | ORCA 6.1 · B3LYP-D3(BJ)/def2-SVP | S11 | Ester Studio 频率验收样本 |
| 2-甲基-1-丙醇 | Gaussian 16 · PM7 | S12 | Ester Studio Opt/Freq 验收样本 |
| 二乙烯基苯 | Gaussian 09 · B3LYP/STO-3G | S14、S15、S16、S17 | [cclib-data 原始日志](https://github.com/cclib/cclib-data/blob/0103b6867ce7d6a3f719fe2e757ee3eb95cd5268/Gaussian/Gaussian09/dvb_raman_revA.02.out) |
| 二乙烯基苯 | ORCA 4.2 · B3LYP/STO-3G（数值频率） | S18 | [cclib-data 原始日志](https://github.com/cclib/cclib-data/blob/0103b6867ce7d6a3f719fe2e757ee3eb95cd5268/ORCA/ORCA4.2/dvb_raman.out) |

## 图号与原图

| 图号 | 类型 | 展示方式 | 半高全宽或柱图数据 |
| --- | --- | --- | --- |
| [S01](images/spectra/s01.png) | 紫外吸收 | 能量轴全谱 | 0.24 eV |
| [S02](images/spectra/s02.png) | 紫外吸收 | 波长轴 · 渐变填色 | 0.24 eV |
| [S03](images/spectra/s03.png) | 紫外吸收 | 全谱＋主峰区放大 | 0.24 eV，局部范围 5.12–5.6 eV |
| [S04](images/spectra/s04.png) | 紫外吸收 | 吸收包络与跃迁棒谱 | 0.24 eV |
| [S05](images/spectra/s05.png) | 紫外吸收 | 振子强度 · 实色柱 | 原始数值 |
| [S06](images/spectra/s06.png) | 紫外吸收 | 振子强度 · 渐变柱 | 原始数值 |
| [S07](images/spectra/s07.png) | 紫外吸收 | 波长轴全谱 | 0.24 eV |
| [S08](images/spectra/s08.png) | 红外 | 红外全谱 | 20 cm⁻¹ |
| [S09](images/spectra/s09.png) | 红外 | 指纹区放大 · 渐变填色 | 20 cm⁻¹，局部范围 750–1650 cm⁻¹ |
| [S10](images/spectra/s10.png) | 红外 | 全谱＋指纹区副图 | 20 cm⁻¹，局部范围 840–1150 cm⁻¹ |
| [S11](images/spectra/s11.png) | 红外 | 水的红外全谱 | 20 cm⁻¹ |
| [S12](images/spectra/s12.png) | 红外 | 醇的红外全谱 · 渐变填色 | 20 cm⁻¹ |
| [S13](images/spectra/s13.png) | 红外 | 指纹区 IR 强度 · 渐变柱 | 原始数值，选取 850–1120 cm⁻¹ 内的振动模态 |
| [S14](images/spectra/s14.png) | 拉曼 | Stokes 全谱 | 20 cm⁻¹ |
| [S15](images/spectra/s15.png) | 拉曼 | 主峰区放大 · 渐变填色 | 20 cm⁻¹，局部范围 1200–1850 cm⁻¹ |
| [S16](images/spectra/s16.png) | 拉曼 | Stokes 全谱＋主峰区副图 | 20 cm⁻¹，局部范围 1520–1860 cm⁻¹ |
| [S17](images/spectra/s17.png) | 拉曼 | 拉曼活性 · 渐变柱 | 原始数值，选取 1200–1850 cm⁻¹ 内的振动模态 |
| [S18](images/spectra/s18.png) | 拉曼 | 数值频率的 Stokes 全谱 | 20 cm⁻¹ |
