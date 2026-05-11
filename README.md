# Semiconductor Materials Research Group Website

这是一个小型静态网站，用于展示研究组成员、简介与研究方向。主要页面和样式位于仓库根目录。

快速链接（仓库内文件与符号）
- 主页面：[index.html](index.html)
- 成员页面：[zirui/index.html](zirui/index.html)、[kangling/index.html](kangling/index.html)
- 全局样式：[style.css](style.css)（示例符号：[`--blue-900`](style.css)、[`.hero`](style.css)、[`.profile-header`](style.css)）
- GitHub Pages 部署工作流：[.github/workflows/static.yml](.github/workflows/static.yml)
- 本文件：[README.md](README.md)

## 简介
本仓库包含一个静态网站，用于展示半导体材料研究组的成员与研究方向。页面基于纯 HTML/CSS，无构建步骤，便于直接在浏览器或 GitHub Pages 部署。

## 本地预览
在开发容器中用主机默认浏览器打开主页：
$BROWSER index.html

或使用简单静态服务器：
```sh
python3 -m http.server 8000
```

然后访问 http://localhost:8000/index.html

# 部署
仓库配置了 GitHub Pages 自动部署（见 [.github/workflows/static.yml](.github/workflows/static.yml)）。推送到 `main` 分支后，Actions 会构建并部署站点。

# 编辑与贡献
- 添加成员页面：在根目录创建子目录（例如 `name/index.html`），放置头像和页面文件，并在 [index.html](index.html) 的成员列表中添加链接。
- 参考现有成员页：[zirui/index.html](zirui/index.html)、[kangling/index.html](kangling/index.html)。
- 静态资源使用相对路径，放在成员目录或仓库根目录。

# 注意事项
- 使用相对路径以确保 GitHub Pages 部署时资源能正确加载。
- 样式与配色变量位于 [style.css](style.css)（示例：[`--blue-900`](style.css)）；布局类示例：[`.hero`](style.css)、[`.profile-header`](style.css)。
- 保持 README 简洁，必要时在每次大改动后更新部署/资源说明。