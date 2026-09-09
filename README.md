# 妈，我真睡了 · 一分钟随机检查版

这是 Cocos Creator 3.8.8 Web Mobile 构建的静态发布成品，不需要 Node.js、后端或外部 CDN。

## 游戏

- 60 秒倒计时，顶部显示 01:00。
- 点击“补作业”或“装睡”，一次点击切换并保持状态。
- 门口、留房、床侧、窗外、老鼠检查每局各一次，随机顺序与间隔。
- 原有预警、动画和结局规则不变；本次只增加总时长。

## 发布到 GitHub Pages

1. 解压发布 ZIP。把里面的 `index.html`、`.nojekyll`、`README.md` 放到用于发布的仓库根目录。
   **不要只上传 ZIP，也不要把 ZIP 外面的一层文件夹当成网站根目录。**
2. 在仓库的 Settings → Pages 中，找到 Build and deployment。
3. Source 选择 Deploy from a branch，分支选择实际放置文件的分支（通常为 `main`），目录选择 `/ (root)`，保存。
4. 等待 GitHub 的部署完成。实际访问地址以 Pages 设置页给出的地址为准。
   仓库代码文件页面不等于游戏网址；请打开 Pages 网站，而不是 GitHub 的 HTML 源码预览。

如果仓库已有网站，先备份原 `index.html`，避免覆盖旧网站。
是否能启用 Pages 取决于你的仓库与账号设置。本包未替你创建仓库或进行线上发布。

## 包内文件

- `index.html`：唯一运行入口，所有游戏脚本、引擎和素材已内嵌。不要改入口文件名。
- `.nojekyll`：直接发布构建成品，不需要 Jekyll 处理。
- `README.md`：本说明，不参与游戏运行。

本地也可以直接双击 `index.html`。
没有包含账号凭据、构建缓存、测试日志或原工程目录。

## 官方发布文档

发布来源与分支/目录设置已于 2026-09-09 核对 GitHub 官方文档：
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

本地构建与浏览器测试通过不等于已经在你的 GitHub Pages 站点上线；
线上网址、手机真机和仓库权限需要你部署后再验收。
