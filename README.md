# 📚 ArXiv论文爬虫

这是一个专门用于抓取arXiv上最新扩散模型(Diffusion Models)和图像/视频生成相关论文的爬虫程序。它不仅会下载论文PDF，还会提取论文中的图片，并生成一个包含论文摘要和图片的markdown文档，方便快速浏览和研究。

## ✨ 功能特点

- 🤖 自动搜索和下载扩散模型相关论文
- ⏰ 支持指定时间范围的论文搜索（默认最近7天）
- 🖼 生成包含论文摘要的markdown文档
- 🔧 自动整理已下载的论文到日期文件夹
- ⚙️ 支持命令行参数配置

## 🔍 搜索范围

### 🎯 主要关键词（必须包含其中之一）
- 🌟 diffusion model
- 🌟 DDPM
- 🌟 stable diffusion
- 🌟 latent diffusion

### 🎨 次要关键词（必须包含其中之一）
- 🖼️ image generation
- 🎬 video generation
- 📝 text-to-image
- 🎥 text-to-video
- 🎨 image synthesis
- 🎬 video synthesis

### 📚 学科分类
仅搜索以下分类的论文：
- 👁️ 计算机视觉 (cs.CV)
- 🧠 机器学习 (cs.LG)
- 🤖 人工智能 (cs.AI)

## 🚀 安装和使用

### 🔰 基本使用
1. 📥 克隆仓库
```bash
git clone https://github.com/offline888/arxiv-crawler.git
cd arxiv-crawler
```

2. 📥 安装依赖
```bash
python -m pip install -r requirements.txt
```

3. 🚀 运行爬虫
```bash
python arxiv_crawler.py
```

### 🔰 命令行参数
```bash
python arxiv_crawler.py --days 10 --dir "D:/paper"
```

### 🔰 注意事项 
- 请确保安装了所需的依赖包，否则程序会提示缺失的包并询问是否安装。
- 请确保有足够的磁盘空间来保存下载的PDF和提取的图片。
- 请确保网络连接稳定，否则可能会导致下载失败。
- 请确保有足够的权限来保存文件到指定的目录。
