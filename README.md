# Semi-Utils Pro

> 基于 [semi-utils](https://github.com/leslievan/semi-utils) 二次开发，增加了 Vercel 云端部署支持。
>
> **一个用于给照片批量添加水印、处理像素比、图像色彩和质量的工具。**

[![license](https://img.shields.io/github/license/ydhawesome/semi-utils)](LICENSE)
![language](https://img.shields.io/github/languages/top/ydhawesome/semi-utils?color=orange)
[![Vercel](https://img.shields.io/badge/Vercel-deployed-brightgreen)](https://semi-utils-main.vercel.app)

## 在线使用

直接访问，无需安装：

**[https://semi-utils-main.vercel.app](https://semi-utils-main.vercel.app)**

或通过 GitHub Pages 入口：**[https://ydhawesome.github.io/semi-utils/](https://ydhawesome.github.io/semi-utils/)**

## 本地运行

**环境要求：** Python 3.11+

```bash
# 安装依赖
pip install -r requirements.txt

# 启动服务
python app.py
```

浏览器访问 `http://localhost:15050`

> **可选**：下载 [exiftool](https://exiftool.org/) 放到 `exiftool/` 目录可获得更完整的 EXIF 读取支持；不配置时自动使用 Pillow 作为备用。

## 效果展示

| 模板 | 描述 | 效果 |
|------|------|------|
| [standard1](./static/standard1.json) | 经典 EXIF 水印，包含相机型号、镜头、光圈、快门、ISO 和品牌 Logo | ![standard1](./static/standard1.jpeg) |
| [standard2](./static/standard2.json) | 在 standard1 基础上添加圆角、阴影和留白，适合社交媒体分享 | ![standard2](./static/standard2.jpeg) |
| [nikon_blur](./static/nikon_blur.json) | 尼康风格水印，红色「Z」字高亮，配合模糊背景 | ![nikon_blur](./static/nikon_blur.jpeg) |
| [blur](./static/blur.json) | 相机型号+参数垂直居中，配合模糊背景 | ![blur](./static/blur.jpeg) |
| [normal1](./static/normal1.json) | 极简风格，右下角显示拍摄参数 | ![normal1](./static/normal1.jpeg) |
| [normal2](./static/normal2.json) | 文件夹名称+拍摄时间，橙色文字 | ![normal2](./static/normal2.jpeg) |
| [center_logo](./static/center_logo.json) | 中心 Logo 水印，可自定义四周文字 | ![center_logo](./static/center_logo.jpeg) |

## 部署到自己的 Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/ydhawesome/semi-utils)

或手动部署：

```bash
npm i -g vercel
vercel deploy --prod
```

## 许可证

基于 [Apache License 2.0](LICENSE) 发布。

原项目 [semi-utils](https://github.com/leslievan/semi-utils) 由 [@LeslieVan](https://github.com/leslievan) 开发。
