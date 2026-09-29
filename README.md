# 📚 蒸馏作品收藏集

> 收集 GitHub 上优秀的"知识蒸馏"项目——把古籍、长文、书籍提炼成结构化知识的作品与工具。
> 本仓库为个人收藏导读，全部项目版权归原作者所有，本仓库仅整理链接与笔记。

---

## 一、中医古籍蒸馏类

### ⭐ [zhongyishijia-skill](https://github.com/erikgqp8645/zhongyishijia-skill)
把中医世家网站 678 本古医书（5.7GB 原始数据）蒸馏成 **31.7 万张结构化 evidence card**（268MB JSONL）。
- 每张卡含：方剂名 / 病证名 / 中药名 / 主治 / 处方 / 各家论述 / 出处
- 三层结构：L2 蒸馏卡（快速检索）→ L1 书籍 JSON（689 本完整结构）→ L0 原始 SQLite（全量兜底）
- 每张卡可回溯到《伤寒论》《金匮要略》等具体古籍原文，"不编造、可验证"
- 📎 本仓库收录样例：[样例_桂枝人参汤历代注解.md](样例_桂枝人参汤历代注解.md)（105 条按朝代排序）

### [tcm-db](https://github.com/xiaogege6697/tcm-db)（倪海厦中医知识数据库）
3867 条结构化 SQLite 记录（中药/方剂/医案/经典/针灸/天纪）+ 2987 条 OCR 讲稿，RAG-ready。

### [ni-haisha-tcm-skill](https://github.com/qmzz/ni-haisha-tcm-skill)
经方库 113 首 + 汉唐方剂 89 首 + 本草 415 味 + 腧穴 411 个，每味带"方义推演 + 讲义实录"。

### [tcm_lib_search](https://github.com/wang-shuyu/tcm_lib_search)
从古籍**自动抽取方剂**的文本挖掘工具，附带按药味组成检索 791 本古籍的数据库。提供 Windows/Mac 免安装可执行包。

### [TCM-Ancient-Books 数据集](https://github.com/yardstick17/TCM-Ancient-Books)
约 700 本中医药古籍电子文本（80MB），先秦至清末民国，覆盖医学理论、方剂学、药物学、临床案例。

---

## 二、拆书 / 读书蒸馏类

### [book-distiller](https://github.com/daizhouchen/book-distiller)
把一本书蒸馏成**中文典雅风单页 HTML 报告**：宋体排版、水墨 SVG、速读/精读/深读三种模式、来源 A-D 分级。
- Claude Code Skill 形式，MIT 协议
- 同系列：[movie-distiller 电影蒸馏](https://github.com/daizhouchen/movie-distiller)、[domain-onboarding 领域入门](https://github.com/daizhouchen/domain-onboarding)
- 红楼梦旗舰示范：产物 487KB，8 场景细读 + 10 人物小传 + 3 诗词专题

### [book-deep-analysis](https://github.com/wenrui-ai/book-deep-analysis)
纸质书/扫描 PDF → OCR → 概念卡 → Obsidian 知识图谱。290 页扫描书 2 小时 40 分变 81 张概念卡 + 81 节点 728 连接的图谱。用智谱 API。

### [spinedigest](https://github.com/oomol-lab/spinedigest)
逐章提取知识点 + 自动建知识图谱，输出 .sdpub 格式，配套可视化阅读器 Inkora。`npx spinedigest` 免安装。

### [books-notes-zk](https://github.com/abetts00/books-notes-zk)
书摘 PDF → Obsidian 卡片盒 + 实体自动链接（人物/书籍/概念自动互链），带 MCP server，成本约 $0.01/本。

---

## 三、使用笔记

（此处记录自己使用以上项目的心得，随用随补）

- 2026-09-29：初建收藏集，抓取了 zhongyishijia-skill 的桂枝人参汤样例。GitHub raw 下载需走 `curl -4` 强制 IPv4，大文件（268MB LFS）建议空闲时段单独拉取。
