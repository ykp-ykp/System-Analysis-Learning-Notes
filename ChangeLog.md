## [2026-05-23] 重构 — 完善规范继承与目录级规则

- 变更文件：
  `AGENTS.md`（修改）、
  `.gitignore`（新增）、
  `gitignore`（删除）、
  `books/Docx/AGENTS.md`（新增）、
  `books/Docx/CLAUDE.md`（新增）、
  `vocabulary/AGENTS.md`（新增）、
  `vocabulary/CLAUDE.md`（新增）、
  `vocabulary/vocabulary.md`（修改）
- 变更内容：
  1. 重构 AGENTS.md：统一表格排版格式，项目根目录改为相对路径，目录权限新增 `.temp/` 临时目录并补充 `books/Docx/`、`vocabulary/` 子目录规范继承说明；
  2. 新增 `books/Docx/AGENTS.md`：定义该目录下的文件类型、标题层级、排版、来源信息、命名等规范；
  3. 新增 `vocabulary/AGENTS.md`：定义词条格式（中文释义+英文全称+音标）和有序列表规范；
  4. 新增 `vocabulary/CLAUDE.md` 和 `books/Docx/CLAUDE.md`：指向各自子目录 AGENTS.md 的跳转文件；
  5. 用 `.gitignore` 替换旧 `gitignore` 文件，并纳入版本控制；
  6. 清理 `vocabulary/vocabulary.md` 中无效测试词条。
- 操作 Agent：Codex

## [2026-05-23] 删除笔记 3.1 计算机系统概述备考笔记 和 3.2 存储器系统备考笔记

## [2026-05-21] 新增 — 3.2 存储器系统备考笔记

- 变更文件：`studyNotes/3.2_存储器系统_备考笔记.md`
- 变更内容：新增第3章第2节存储器系统备考笔记，涵盖存储器层次结构、Cache映射/替换/写策略、RAID技术0~6级对比、虚拟存储器（页式/段式/段页式）、相联存储器、存储保护、磁盘存取时间计算等核心考点，含5道计算模拟题及15条背诵知识点。
- 操作 Agent：Claude

## [2026-05-21] 新增 — 3.1 计算机系统概述备考笔记

- 变更文件：`studyNotes/3.1_计算机系统概述_备考笔记.md`
- 变更内容：新增第3章第1节计算机系统概述备考笔记，涵盖冯·诺依曼结构、Flynn 分类法、CISC vs RISC、流水线技术、存储器层次、Cache、RAID、系统可靠性、I/O 控制方式等核心考点，含历年真题/模拟题及背诵知识点。
- 操作 Agent：Claude

# 初始化项目的AGENT.md说明
