<img src="./image/line-neon.gif" width=100%><br>

<div id="user-content-toc">
  <ul align="center">
    <summary><h1 style="display: inline-block"><b>🌠 SYSU-Beamer: A Quickstart For Your Demonstration</b></h1></summary>
    <a href="https://github.com/LulietLyan/SYSU-Beamer"><strong>查看文档 »</strong></a>
    <br />
    <a href="https://github.com/LulietLyan/SYSU-Beamer">演示</a>
    &middot;
    <a href="https://github.com/LulietLyan/SYSU-Beamer/issues/new?labels=bug&template=bug-report---.md">Bugs</a>
    &middot;
    <a href="https://github.com/LulietLyan/SYSU-Beamer/issues/new?labels=enhancement&template=feature-request---.md">特性</a>
  </ul>
</div>

<p align="center"> 
    <img src="https://img.shields.io/github/followers/LulietLyan?label=Followers&style=for-the-badge&color=purple"alt="github follow"/>
    <img src="https://img.shields.io/github/stars/LulietLyan/SYSU-Beamer?label=Stars&style=for-the-badge"
    alt="github repo stars" >
    <img src="https://img.shields.io/github/contributors/LulietLyan/SYSU-Beamer?style=for-the-badge&logoColor=%23985684"
    alt="contributors" >
    <img src="https://img.shields.io/github/issues-pr/LulietLyan/SYSU-Beamer?style=for-the-badge&color=%23985684"
    alt="issues-pr" >
    <img src="https://img.shields.io/github/issues/LulietLyan/SYSU-Beamer?style=for-the-badge&color=%23777777" 
    alt="issues" >
    <img src="https://img.shields.io/github/forks/LulietLyan/SYSU-Beamer?style=for-the-badge&color=%23187777" 
    alt="forks" >
    <img src="https://img.shields.io/badge/Contributions-Welcome-%23028745?style=for-the-badge&labelColor=%23b08f42"
    alt="contribution"/>
    <img src="https://img.shields.io/badge/Star-IfYouLike-%23067897?style=for-the-badge&labelColor=%23879078"
    alt="star"/>
    <img src="https://img.shields.io/github/license/LulietLyan/SYSU-Beamer?style=for-the-badge"
    alt="license" >
</p>

<p align="center"> 
<a href="https://github.com/LulietLyan/SYSU-Beamer"><img src="./image/SYSU.svg" height=50pt alt="lulietlyan" /></a>
<a href="https://github.com/LulietLyan/SYSU-Beamer"><img src="./image/NSCC-GZ.svg" height=50pt alt="lulietlyan" /></a>
</p>

<img src="./image/line-neon.gif" width=100%><br>

# 📕 目录
- [📕 目录](#-目录)
- [✨ 功能特性](#-功能特性)
- [🚀 快速开始](#-快速开始)
  - [环境要求](#环境要求)
  - [安装指南](#安装指南)
  - [基础使用](#基础使用)
- [🎨 自定义配置](#-自定义配置)
  - [主题切换](#主题切换)
  - [字体配置](#字体配置)
- [🌐 多语言支持](#-多语言支持)
- [📊 项目结构](#-项目结构)
- [🤝 代码贡献](#-代码贡献)
  - [代码贡献人员](#代码贡献人员)
- [❓ 联系作者](#-联系作者)
- [❗ 授权说明](#-授权说明)

# ✨ 功能特性

|特性|描述|
|:-:|:-:|
|🎯 官方视觉规范|严格遵循中山大学VI系统，校徽绿（#006C35）配色方案|
|📐 响应式布局|智能分栏系统适配不同演示场景|
|🌓 双主题模式|Light/Dark主题一键切换|
|🧮 数学公式支持|原生LaTeX数学环境+AMS宏包扩展|
|🖼️ 矢量图形集成|内置SYSU校徽、标志性建筑等矢量素材|
|📈 数据可视化|预设科研数据图表模板（Matplotlib/TikZ）|
|🎭 渐进式呈现|支持Beamer \pause命令与逐项高亮|
|🛠️ 模块化设计|按章节拆分文件，便于大型演示文稿管理|

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

# 🚀 快速开始

## 环境要求

- **TeX 发行版**: TeX Live 2023+ 或 MiKTeX
- **编译引擎**: XeLaTeX（推荐） / LuaLaTeX
- **中文字体**: 思源宋体/霞鹜文楷

## 安装指南

```bash
# 克隆仓库
git clone https://github.com/SYSU-LaTeX/SYSU-Beamer.git
cd SYSU-Beamer

# 安装依赖（Ubuntu示例）
sudo apt-get install texlive-full fonts-lxgw-wenkai
```

## 基础使用
```bash
\documentclass[SYSU,en]{collegeBeamer} % en为英文模式
\usepackage{xeCJK}
\setCJKmainfont{LXGW WenKai} % 设置中文字体

\begin{document}
\maketitle % 生成标题页
\begin{frame}{演示帧标题}
    \begin{itemize}
        \item 使用itemize环境创建列表
        \item 数学公式示例: $\nabla \cdot \mathbf{D} = \rho_{\text{free}}$
    \end{itemize}
\end{document}
```

编译命令：
```bash
xelatex main.tex
```

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

# 🎨 自定义配置

## 主题切换

```bash
% 类选项配置
\documentclass[SYSU,       % 启用SYSU主题
               dark,       % 深色模式 
               aspectratio=169, % 16:9宽屏（默认）
               greenline   % 标题装饰线颜色
              ]{collegeBeamer}
```

## 字体配置

```bash
% 英文字体设置
\setmainfont{Helvetica Neue}
\setsansfont{Fira Sans}

% 中日韩字体设置
\setCJKmainfont{Source Han Serif SC}
\setCJKsansfont{Source Han Sans SC}
```

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

# 🌐 多语言支持

|语言|状态|示例代码|
|:-:|:-:|:-:|
|简体中文|✅|\documentclass[SYSU,zh]{...|
|英文|✅|\documentclass[SYSU,en]{...|
|日文|🚧|\usepackage{zxjatype}|
|韩文|🚧|\usepackage{nanumtype}|

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

# 📊 项目结构

```bash
SYSU-Beamer/
├── image/               # 文档资源
├── src/                 # 源代码
│   ├── SYSU/            # 主题文件
│   │   ├── color-logo.pdf
│   │   └── ...          # 图形资源
│   └── examples/        # 使用示例
├── SYSU-Beamer.tex      # 入口文件
├── LICENSE              # MIT 许可证
└── README.md            # 本文档
```

# 🤝 代码贡献

开源社区之所以能成为学习、交流与创新的绝佳平台，正是源于每一位参与者的无私奉献。我们诚挚感谢您以任何形式为项目添砖加瓦。

诚挚邀请志同道合的朋友们为本仓库贡献更多内容！若您希望贡献代码：
1. **Fork** 本仓库
2. 在本地拉取您 Fork 的仓库
3. **本地创建新的分支**并进行修改
4. 将修改后的项目**推送**到您 Fork 的仓库中
5. **Pull Request** 至本仓库等待合并

## 代码贡献人员

<a href="https://github.com/LulietLyan/SYSU-Beamer/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=LulietLyan/SYSU-Beamer" alt="contrib.rocks image" />
</a>

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

# ❓ 联系作者

- **项目维护者**：您的姓名  
- **社交媒体**：[@您的推特](https://twitter.com/your_username)  
- **电子邮箱**：email@example.com
- **项目地址**：[GitHub仓库](https://github.com/your_username/repo_name)  

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

# ❗ 授权说明

本项目采用 MIT LICENSE 开源协议（公有领域授权），完整授权条款请参见项目根目录下的 `LICENSE.txt` 文件。

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<img src="./image/line-neon.gif" width=100%><br>