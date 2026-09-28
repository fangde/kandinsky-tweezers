# 手腕不动,让镊子在指尖走完那 5 毫米

灵巧手在掌操作(In-Hand Dexterous Manipulation)的中文精读长页,以**康定斯基 / 包豪斯构造主义**风格排版。

> 原论文:*A Model-Based Framework for Dexterous In-Hand Tweezers Manipulation*

## 这是什么

一篇论文精读的可视化网页版:把镊子建模成一个「6 + 1」自由度的关节工具,用带约束的逆运动学,
让灵巧手的指尖直接生成毫米级的笛卡尔运动——**手腕完全不动**。

## 设计

| 维度 | 做法 |
|---|---|
| 配色 | 稻纸底 `#F2EEE3` + 炭黑 `#131313` + 包豪斯三原色(正红 `#DF3524` / 铬黄 `#F0C200` / 群青 `#1D3FA6`),平涂不叠加 |
| 字形 | 标题 Jost(几何无衬线,近 Futura),正文 Noto Sans SC,编号 IBM Plex Mono |
| 版式 | 方角优先、零渐变、零投影、硬边描线;左侧书脊 + 右侧章节导航 + 顶部三原色阅读进度 |
| 图形 | Hero 与内文插图均为几何抽象构图(圆 / 三角 / 方 / 同心圆 / 硬直斜线) |
| 公式 | 38 组公式全部由 KaTeX 实时渲染,可直接选中复制 LaTeX |
| 动效 | 入场分段揭示、滚动揭示、章节导航跟随;支持 `prefers-reduced-motion` |

## 文件结构

```
.
├── index.html          # 单页长文(自包含设计系统,仅依赖 CDN 字体 + KaTeX)
├── assets/images/      # 5 张包豪斯风格插图
├── .nojekyll           # 关闭 Jekyll 处理
└── README.md
```

## 本地预览

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000
```

## 许可

正文内容与图表版权归原论文作者所有;本页仅作排版与阅读体验的展示。
