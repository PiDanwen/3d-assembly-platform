# 3D模型搭建配置平台

一个用于3D模型零件解析、安装方向配置、模拟搭建预览的在线工具。

## 功能特性

- 📦 **资源管理** - 3D模型资源的增删改查
- ⚙️ **零件解析** - 自动解析GLB/GLTF/OBJ格式模型
- 🔄 **安装方向配置** - 可视化配置6个方向（X+/X-/Y+/Y-/Z+/Z-）
- 👁️ **360°旋转预览** - 独立小窗口预览选中零件
- ✈️ **飞入动画** - 零件沿安装方向飞入到正确位置
- 🎮 **手动步骤预览** - 点击"下一步"控制装配流程

## 技术栈

- Three.js 0.160.0 (3D渲染)
- 原生HTML/CSS/JavaScript
- localStorage (数据持久化)

## 快速开始

### 在线访问

直接打开 `resource-list.html` 文件即可使用。

### 本地开发

1. 克隆仓库
```bash
git clone https://github.com/PiDanwen/3d-assembly-platform.git
cd 3d-assembly-platform
```

2. 使用任意静态服务器启动
```bash
# Python
python -m http.server 8000

# Node.js
npx serve .
```

3. 浏览器打开 `http://localhost:8000`

## 页面说明

| 页面 | 文件 | 说明 |
|------|------|------|
| 资源列表 | `resource-list.html` | 管理3D模型资源 |
| 3D配置 | `3d-assembly-platform.html` | 配置零件安装方向 |

## 使用流程

1. **新建资源** - 在资源列表页点击"新建资源"
2. **上传模型** - 上传GLB/GLTF/OBJ格式文件
3. **配置零件** - 为每个零件选择安装方向
4. **预览确认** - 使用手动步骤预览检查装配效果
5. **保存发布** - 保存配置并发布资源

## 浏览器兼容性

- Chrome 80+
- Firefox 75+
- Safari 14+
- Edge 80+

## License

MIT
