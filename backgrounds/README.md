# 背景图片文件夹

这个文件夹用于存放网站的背景图片和装饰性图片。

## 推荐的文件结构

```
backgrounds/
├── hero-bg.jpg              # 英雄区域背景
├── section-bg.jpg           # 章节背景
├── pattern.svg              # 装饰性图案
├── texture.jpg              # 纹理背景
└── overlays/                # 叠加层图片
    ├── gradient-overlay.png
    └── noise-texture.png
```

## 图片要求

- **格式**: JPG、PNG 或 SVG
- **尺寸**: 根据使用场景调整
- **风格**: 与网站整体设计风格一致
- **文件大小**: 建议每张图片不超过 1MB

## 使用方式

在CSS中使用：

```css
.hero {
  background-image: url('/backgrounds/hero-bg.jpg');
  background-size: cover;
  background-position: center;
}
```

在React组件中使用：

```jsx
import heroBg from '/backgrounds/hero-bg.jpg'

// 在组件中使用
<div style={{ backgroundImage: `url(${heroBg})` }}>
  {/* 内容 */}
</div>
```
