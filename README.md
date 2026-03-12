# Yet Another NPU Thesis Template - Murphy
> - Forked from [Yet-Another-LaTeX-Template-for-NPU-Thesis](https://github.com/NWPUMetaphysicsOffice/Yet-Another-LaTeX-Template-for-NPU-Thesis)

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![LaTeX](https://img.shields.io/badge/LaTeX-Document-green.svg)](https://www.latex-project.org/)

## 概述

这是一个专为西北工业大学学位论文设计的 LaTeX 模板，支持硕士和博士学位论文的撰写。模板基于 `yanputhesis` 文档类，提供了完整的版本控制功能和模块化结构。

## 环境配置

- 操作系统: Windows 11 Pro 24H2
- TeX 发行版: TeX Live 2024
  - TeX 版本: 3.141592653 (TeX Live 2024)
  - kpathsea 版本: 6.4.0
- 编译器: XeTeX
- 编辑器: VS Code 1.106 + LaTeX Workshop 10.11.3

## 快速开始

### 1. 克隆项目
```bash
git clone https://github.com/murphyhoucn/Yet-Another-LaTeX-Template-for-NPU-Thesis-Murphy.git
cd Yet-Another-LaTeX-Template-for-NPU-Thesis-Murphy
git submodule update --init --recursive
```

### 2. 编辑基本信息

修改 `main.tex` 中的基本信息：

```latex
%% 设置论文类型（博士/硕士、是否盲评）
\documentclass[lang=chs, degree=master, blindreview=false, adobe=false]{yanputhesis}

%% 填写个人信息
\title{你的论文标题}{Your Thesis Title in English}
\author{你的姓名}{Your Name}
\school{你的学院}{Your School}
\major{你的专业}{Your Major}
\advisor{导师姓名}{Advisor Name}
\studentnumber{你的学号}
```

### 3. 版本控制说明

本模板采用版本控制结构，可以轻松管理不同版本的论文内容：

```latex
%% 在 main.tex 中设置当前版本
\newcommand{\VersionControl}{Thesis_v1_20250901}
```

目录结构：
```
Thesis_v1_20250901/
├── abstract/
│   ├── chinese-abstract.tex    % 中文摘要
│   └── english-abstract.tex    % 英文摘要
├── acknowledgement/
│   ├── acknowledgements.tex    % 致谢
│   └── accomplishments.tex     % 参加科研情况
├── chapters/
│   ├── chapter01-introduction.tex  % 第一章
│   ├── chapter02-theory.tex        % 第二章
│   ├── chapter03-method_1.tex      % 第三章
│   ├── chapter04-method_2.tex      % 第四章
│   ├── chapter05-conclusion.tex    % 第五章
│   └── appendices.tex              % 附录
└── references/
    └── reference.bib               % 参考文献
```

