# christmas-tree-3d

一个手势交互 3D 圣诞树的原型项目（THREE.js + MediaPipe Hands）。

## 快速开始

这是一个**单文件应用**：`index.html`（包含 HTML + CSS + JS）。

由于浏览器摄像头权限要求，建议通过本地静态服务器运行：

```bash
# 任意一种都可以
python3 -m http.server 5173
# 或
npx serve .
```

然后打开：

- http://localhost:5173

## 当前已实现（基础框架）

- THREE.js 场景初始化（Scene/Camera/Renderer、基础光照、渲染循环）
- MediaPipe Hands 摄像头输入 + 手部关键点绘制
- 基础状态机：CLOSED / OPEN / ZOOM
- 手势映射：握拳 / 张手 / 捏合（pinch）
- 照片上传并作为纹理贴到场景中的占位平面上
- 简易 FPS 监控与状态显示面板
