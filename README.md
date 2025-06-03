# DPM-Collection-Crawler

本项目是一个用于自动化抓取故宫博物院官网外国文物藏品信息的小工具。它基于 Selenium 自动浏览网页，提取每件藏品的标题、简介和图片，并将结果整理到 Word 文档中，方便后续整理和知识库建设。

## 功能简介

- 自动访问故宫博物院外国文物页面
- 批量提取每件藏品的详情页链接
- 获取详情页的标题、简介（meta Description）和主图片
- 自动将内容和图片整理到 Word 文档

## 使用方法

1. **环境准备**

   - Python 3.7+
   - 安装依赖：
     ```bash
     pip install selenium python-docx requests -i https://mirrors.aliyun.com/pypi/simple/
     ```
   - 安装 Chrome 浏览器和 ChromeDriver，并确保 ChromeDriver 版本与 Chrome 浏览器一致。

2. **运行脚本**

   ```bash
   python 爬虫.py
   ```

3. **输出结果**

   - 运行结束后，会在当前目录生成 `故宫外国文物详情.docx`，包含所有抓取到的文物信息和图片。

## 注意事项

- 本工具仅用于学习和学术研究，请勿用于商业用途。
- 若网站结构有变动，需相应调整代码中的元素定位方式。
- 运行过程中会自动打开和关闭浏览器窗口，请勿手动干预。

## 贡献

欢迎提交 issue 或 PR 改进本项目！

