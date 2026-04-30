# 日常学习

AI 和计算机知识的日常学习笔记与代码练习。

## 结构约定

```
daily-learning/
├── topics/       # 主题知识库 — 系统整理的领域知识
│   ├── ml/       #   机器学习
│   ├── dl/       #   深度学习
│   ├── cs/       #   计算机基础
│   ├── math/     #   数学基础
│   └── tools/    #   工程工具
├── daily/        # 每日记录 — YYYY/MM/YYYY-MM-DD.md
├── papers/       # 论文阅读 — 每篇一个 md，含摘要/方法/感想
├── code/         # 代码练习
│   ├── scratch/  #   临时实验，用完即清
│   └── snippets/ #   可复用片段，带注释说明
└── resources/    # 优质资源链接索引
```

## 命名规范
- `daily/` 文件：`YYYY-MM-DD.md`
- `topics/` 文件：按主题组织，用有意义的英文命名，如 `transformer-architecture.md`
- `papers/` 文件：`[年份]-[简写标题].md`，如 `2025-attention-is-all-you-need.md`
- `code/snippets/` 文件：`[语言]-[功能描述].py`，如 `py-data-augmentation.py`

## 记录原则
- **先写 daily**，每天学完随手记，不求格式，关键是记下来
- **定期整理**，daily 积累到一定量，挑有价值的内容整理进 topics
- **实验放 scratch**，验证完想法就清理，不留垃圾
- **资源随手存**，看到好的文章/课程/工具，直接加 resources 里

## 清理规则
- `code/scratch/`：任务完成即删除，最长保留不超过一周
- `daily/`：保留原始记录不删，但已整理进 topics 的内容可以在文件开头加 `[MERGED]` 标记
