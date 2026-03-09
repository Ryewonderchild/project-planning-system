# 团队项目执行看板

这是一个轻量级管理看板，展示：
- 首页总览
- 任务清单
- 甘特排期
- 成员负荷

## 为什么之前“无法打开”
之前版本依赖 `npm install` 拉取 React/Vite/Tailwind 包，但当前环境访问 npm registry 返回 `403`，导致依赖无法安装，应用无法启动。

## 当前打开方式（零安装）
本版本改为 CDN 运行 React + TypeScript(Babel) + Tailwind，无需 `npm install`。

```bash
python -m http.server 4173
```

然后访问：

`http://127.0.0.1:4173`

> 也可以直接双击 `index.html` 打开；若浏览器阻止跨源脚本，请使用上面的本地服务方式。
