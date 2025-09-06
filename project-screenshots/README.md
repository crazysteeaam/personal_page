# 项目截图文件夹

这个文件夹用于存放你的项目截图和演示图片。

## 推荐的文件结构

```
project-screenshots/
├── agent-system.jpg          # AI Agent系统截图
├── simulation-optimization.jpg # 流程仿真优化截图
├── form-automation.jpg       # 表单自动化截图
├── ai-platform.jpg          # AI平台截图
└── other-projects/          # 其他项目截图
    ├── project1.jpg
    ├── project2.jpg
    └── project3.jpg
```

## 图片要求

- **格式**: JPG 或 PNG
- **尺寸**: 建议 800x600 或 1200x800 像素
- **质量**: 清晰、专业，展示项目亮点
- **文件大小**: 建议每张图片不超过 500KB

## 使用方式

在React组件中，你可以这样引用这些图片：

```jsx
import projectImage from '/project-screenshots/agent-system.jpg'

// 在组件中使用
<img src={projectImage} alt="AI Agent系统" />
```

或者直接使用路径：

```jsx
<img src="/project-screenshots/agent-system.jpg" alt="AI Agent系统" />
```
