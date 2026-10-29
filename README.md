<div align="center">

<img src="docs/images/ester-icon.png" width="96" alt="Ester Studio ES 图标">

# Ester Studio

**一站式计算化学建模、输入准备与结果后处理工作台**

免费使用 · 源码公开 · 免安装 · 开箱即用

[下载 Windows 便携版](https://github.com/Ahey1/Ester-Studio/releases/download/v1-ester/Ester-Studio-v1-Windows-x64.zip) · [下载完整源码](https://github.com/Ahey1/Ester-Studio/releases/download/v1-ester/Ester-Studio-v1-source-code.zip) · [碘到为酯 · B站](https://space.bilibili.com/3493133310495553)

</div>

## 从结构到结果

- **建模**：分子与晶体、片段与结构库、周期结构与预优化。
- **输入准备**：Gaussian / ORCA 方法、基组、电荷与自旋、溶剂、约束和资源设置。
- **结果与后处理**：结构与能量、轨道与振动、激发态、NTO、ESP、IRI / IGMH。
- **科研出图**：四种分子模型预设、自定义光照与材质、完整图片与透明背景导出。

## 软件实际出图

以下图片由本软件的既有 SY-Studio 构建实际导出。Ester Studio 延续相同的科学计算与绘图功能；图片完整保留画面，模型为公开咖啡因结构。

<table><tr><td align="center"><img src="docs/images/model.png" width="420" alt="青碳高光分子预设"><br>青碳高光模型</td><td align="center"><img src="docs/images/homo.png" width="420" alt="咖啡因 GFN2-xTB HOMO 轨道"><br>HOMO 轨道</td></tr></table>

<p align="center"><img src="docs/images/esp.png" width="760" alt="咖啡因 GFN2-xTB ESP 着色表面及完整色尺"></p>

<p align="center">ESP 着色分子表面 · 保留色尺与单位</p>

轨道和 ESP 示例来自咖啡因 GFN2-xTB 气相单点，后处理由软件调用用户配置的 Multiwfn 完成。图片展示出图能力，不标作 DFT 或 NTO 结果。

## 下载与使用

**v1 / 1.0.0**：通过 [Ester Studio v1 下载页](https://github.com/Ahey1/Ester-Studio/releases/tag/v1-ester) 获取 Windows x64 便携包和单个完整源码包。校验值见同页版本说明。[旧 SY-Studio v1](https://github.com/Ahey1/Ester-Studio/releases/tag/v1) 保留供历史查阅。

本仓库仅维护介绍页、展示图片和发行下载，不存放产品源码树。GitHub 自动生成的 **Source code (zip/tar.gz)** 仅包含这个介绍站的文件；完整产品源码请下载 **Ester-Studio-v1-source-code.zip**。

完整解压后运行 **Ester-Studio.exe**。首次启动先阅读 LICENSE，再核对计算资源，默认 4 核、8 GB。常规使用无需另外安装 Python、Node.js 或开发工具。部分波函数分析需要在 Settings 中配置用户自己的 Multiwfn；Gaussian / ORCA 输入生成与结果读取不代表内置这两款计算程序。

Ester Studio 简称 **ES**，原名 SY-Studio。新项目使用 **`.es`**，保留旧 `.sy` 项目的打开与原位保存兼容。Windows 11 已有前版的本机及另一台电脑测试记录，本次更新执行更名、项目格式入口与首启流程定向验证。Windows 10 后续验证。

## 许可与交流

免费使用，遵循[自定义许可](LICENSE.txt)；销售软件副本需作者书面授权。第三方组件遵循各自许可，发行附件中附有相应材料。

[碘到为酯 · B站主页](https://space.bilibili.com/3493133310495553) · [提交问题或建议](https://github.com/Ahey1/Ester-Studio/issues)

作者：**Zixuan Zhang** · 许可事务：**ddwz@sciyue.cn**

欢迎提供版本、系统、复现步骤与截图。目前官方主线由作者维护，不直接接收外部代码合入。
