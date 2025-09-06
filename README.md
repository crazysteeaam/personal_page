# Public 文件夹说明

这个文件夹包含了网站的所有静态资源文件，Vite 会直接将这些文件复制到构建输出目录中。

## 📁 文件夹结构

```
public/
├── favicon.ico              # 网站图标
├── favicon-16x16.png        # 16x16 像素图标
├── favicon-32x32.png        # 32x32 像素图标
├── apple-touch-icon.png     # iOS 主屏幕图标 (180x180)
├── android-chrome-192x192.png # Android 图标 (192x192)
├── android-chrome-512x512.png # Android 图标 (512x512)
├── og-image.jpg             # 社交媒体分享图片 (1200x630)
├── avatar.jpg               # 个人头像
├── project-screenshots/     # 项目截图
├── backgrounds/             # 背景图片
├── icons/                   # 图标文件
└── README.md                # 本说明文件
```

## 🚀 使用方法

### 1. 替换占位符文件

目前创建的文件都是占位符，你需要：

1. **删除占位符文件**
2. **放入真实的图片文件**
3. **确保文件名和扩展名正确**

### 2. 在代码中引用

#### React 组件中

```jsx
// 方式1：直接引用（推荐）
<img src="/avatar.jpg" alt="个人头像" />

// 方式2：导入使用
import avatar from '/avatar.jpg'
<img src={avatar} alt="个人头像" />
```

#### CSS 中

```css
.hero {
  background-image: url('/backgrounds/hero-bg.jpg');
}
```

#### HTML 中

```html
<link rel="icon" href="/favicon.ico">
<meta property="og:image" content="/og-image.jpg">
```

## 📏 图片尺寸建议

| 用途 | 尺寸 | 格式 | 文件大小 |
|------|------|------|----------|
| Favicon | 16x16, 32x32 | ICO, PNG | < 10KB |
| Apple Touch Icon | 180x180 | PNG | < 100KB |
| Android Icon | 192x192, 512x512 | PNG | < 200KB |
| Open Graph | 1200x630 | JPG | < 500KB |
| 头像 | 200x200 | JPG | < 100KB |
| 项目截图 | 800x600 | JPG | < 500KB |
| 背景图 | 1920x1080 | JPG | < 1MB |

## 🎨 图片优化建议

1. **压缩图片**: 使用工具如 TinyPNG 压缩
2. **选择合适的格式**: 
   - JPG: 照片和复杂图像
   - PNG: 图标和需要透明度的图像
   - SVG: 图标和简单图形
3. **响应式图片**: 考虑为不同屏幕尺寸提供不同大小的图片
4. **懒加载**: 对于大图片使用懒加载技术

## 🔧 技术说明

- **Vite 处理**: 这些文件会被直接复制到 `dist/` 目录
- **路径引用**: 在代码中使用 `/文件名` 的方式引用
- **缓存策略**: 生产环境中这些文件会被添加哈希值用于缓存控制
- **CDN 部署**: 可以轻松部署到 CDN 服务

## 📝 注意事项

1. **文件名**: 避免使用中文和特殊字符
2. **文件大小**: 控制图片大小以提升加载速度
3. **备份**: 保留原始高质量图片文件
4. **版权**: 确保使用的图片有合法使用权
