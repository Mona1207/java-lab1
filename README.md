# Java 实验1：基本程序设计与选择结构

课程《Java 语言程序设计（基础）》实验 1 的配套学习站点，纯静态页面（原生 HTML / CSS / JavaScript，无构建步骤、无后端），通过 GitHub Pages 公开访问。

## 在线访问

- 站点入口（导航落地页）：<https://Mona1207.github.io/java-lab1/>
- 精讲网站：<https://Mona1207.github.io/java-lab1/guide/>
- 答题闯关：<https://Mona1207.github.io/java-lab1/quiz/>

## 目录结构

```
.
├── index.html                 # 导航落地页
├── guide/
│   └── index.html             # 知识点精讲网站
├── quiz/
│   └── index.html             # 50 题答题闯关网站
└── .github/workflows/
    └── deploy-pages.yml       # GitHub Pages 自动部署工作流
```

## 内容覆盖

两个 Java 程序（均已实际编译运行，11 组测试用例全部通过）：

1. **GradeCalculator** —— 课程总评成绩计算器：`final` 权重常量、`Scanner` 键盘输入、0~100 合法性校验、加权总评（10% / 30% / 60%）、`printf %.2f` 格式化输出、`if-else if` 分数段等级。
2. **TriangleAnalyzer** —— 三角形类型分析器：1~1000 范围校验、三角形不等式（含退化情形）、等边/等腰/不等边分类、勾股逆定理直角判定、周长与海伦公式面积（避开整数除法陷阱）。

精讲网站包含 12 个核心知识点、逐段代码讲解、判定流水线、两个可交互在线实验台、2 道思考题精讲与十大易错点；答题网站包含 50 道题（36 单选 + 10 判断 + 1 多选 + 3 填空），每题带解析，交卷后给出模块掌握度与错题回顾。

## 本地预览

直接用浏览器打开对应 `index.html` 即可；或在仓库根目录启动任意静态服务器：

```bash
python3 -m http.server 8000
# 浏览器访问 http://localhost:8000/
```

## 部署方式

推送到 `main` 分支后，`.github/workflows/deploy-pages.yml` 会自动把仓库根目录构建为 Pages 站点（GitHub 官方 Actions：configure-pages → upload-pages-artifact → deploy-pages）。
