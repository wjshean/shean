# Shean 的技术博客

一个使用 Hugo 和 PaperMod 构建的轻量级技术博客，通过 GitHub Actions 发布到 GitHub Pages。

## 本地运行

```bash
git clone --recurse-submodules https://github.com/wjshean/shean.github.io.git
cd shean.github.io
hugo server --buildDrafts
```

浏览器访问 `http://localhost:1313/shean.github.io/`。

## 创建文章

```bash
hugo new content posts/my-article.md
```

编辑生成的 Markdown 文件，将 `draft` 改为 `false` 后提交。推送到 `main` 分支会自动触发部署。

## 发布地址

当前仓库是项目站点，默认地址为：

<https://wjshean.github.io/shean.github.io/>

如果将仓库改名为 `wjshean.github.io`，需要同时把 `hugo.yaml` 中的 `baseURL` 改为 `https://wjshean.github.io/`。
