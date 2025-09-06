# 图标文件夹

这个文件夹用于存放网站使用的各种图标。

## 推荐的文件结构

```
icons/
├── social/                   # 社交媒体图标
│   ├── github.svg
│   ├── linkedin.svg
│   ├── twitter.svg
│   └── email.svg
├── tech/                     # 技术栈图标
│   ├── react.svg
│   ├── python.svg
│   ├── java.svg
│   └── ai.svg
├── ui/                       # 界面图标
│   ├── arrow-right.svg
│   ├── menu.svg
│   ├── close.svg
│   └── download.svg
└── custom/                   # 自定义图标
    ├── logo.svg
    └── brand-icon.svg
```

## 图标要求

- **格式**: SVG（推荐）或 PNG
- **尺寸**: SVG 可缩放，PNG 建议 24x24 或 32x32 像素
- **风格**: 统一的设计风格，建议使用线性图标
- **颜色**: 支持 CSS 变量控制颜色

## 使用方式

### SVG 图标（推荐）

```jsx
import { ReactComponent as GithubIcon } from '/icons/social/github.svg'

// 在组件中使用
<GithubIcon className="icon" />
```

### 普通图片图标

```jsx
import githubIcon from '/icons/social/github.png'

// 在组件中使用
<img src={githubIcon} alt="GitHub" className="icon" />
```

### CSS 中使用

```css
.icon {
  width: 24px;
  height: 24px;
  fill: currentColor; /* SVG 图标颜色 */
}
```
