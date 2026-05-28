## [2026-05-28] 新增 — 将.claude软连接到.agents

## [2026-05-28] 新增 — 每日系统分析知识点背诵状态

- 变更文件：
  `notebookLM/flashcards/.flashcard-delivery-state.json`、
  `ChangeLog.md`
- 变更内容：首次执行每日系统分析知识点背诵自动化，从 NotebookLM 闪卡 CSV 中随机抽取 10 条知识点并发送到当前连接 Gmail 账号；新增发送状态文件，用于记录当天 selected_ids、章节、来源文件、主题和发送时间，避免同日重复发送。
- 操作 Agent：Codex

## [2026-05-28] 新增 — 第3、4章 NotebookLM 闪卡 CSV

- 变更文件：
  `notebookLM/flashcards/3/3.1 计算机系统概述.csv`、
  `notebookLM/flashcards/3/3.2 存储器系统.csv`、
  `notebookLM/flashcards/3/3.3 输入输出系统.csv`、
  `notebookLM/flashcards/3/3.4 指令系统.csv`、
  `notebookLM/flashcards/4/4.1 计算机网络基础.csv`、
  `notebookLM/flashcards/4/4.2 网络体系结构与协议.csv`、
  `ChangeLog.md`
- 变更内容：新增第3章计算机系统相关4个小节与第4章网络相关2个小节的 NotebookLM 闪卡 CSV，便于后续导入和复习使用；同步在变更日志顶部记录本次新增内容。
- 操作 Agent：Codex

## [2026-05-27] 新增 — 补充PDF文件
操作 烩面

## [2026-05-27] 新增 — 补充第3-5章的单个小章节的PDF文件
操作 烩面

## [2026-05-26] 修改 — 补充第3章 3.1-3.6 英文术语表

- 变更文件：
  `vocabulary/vocabulary.md`、
  `ChangeLog.md`
- 变更内容：基于 `books/Split Chapters/第3章 计算机系统.pdf` 分章节读取并整理 3.1 至 3.6 中出现的英文术语、缩写与对应中文释义，按有序列表补充到 `vocabulary.md` 的对应小节，并对重要高频概念添加代码样式标记。
- 操作 Agent：Codex

## [2026-05-24] 重构 — 第3章笔记归入 3/ 子目录

- 变更文件：
  `studyNotes/3.1_计算机系统概述_备考笔记.md` → `studyNotes/3/3.1_计算机系统概述_备考笔记.md`、
  `studyNotes/3.2_存储器系统_备考笔记.md` → `studyNotes/3/3.2_存储器系统_备考笔记.md`、
  `studyNotes/3.3_输入输出系统_备考笔记.md` → `studyNotes/3/3.3_输入输出系统_备考笔记.md`、
  `studyNotes/3.4_指令系统_备考笔记.md` → `studyNotes/3/3.4_指令系统_备考笔记.md`、
  `studyNotes/3.5_多处理机系统_备考笔记.md` → `studyNotes/3/3.5_多处理机系统_备考笔记.md`、
  `studyNotes/3.6_操作系统_备考笔记.md` → `studyNotes/3/3.6_操作系统_备考笔记.md`
- 变更内容：将第3章6篇备考笔记从 studyNotes/ 根目录移至 studyNotes/3/ 子目录，按章节组织文件结构，便于后续章节笔记扩展。
- 操作 Agent：Claude

## [2026-05-24] 新增 — 3.2～3.6 备考笔记（5篇）

- 变更文件：
  `studyNotes/3.2_存储器系统_备考笔记.md`、
  `studyNotes/3.3_输入输出系统_备考笔记.md`、
  `studyNotes/3.4_指令系统_备考笔记.md`、
  `studyNotes/3.5_多处理机系统_备考笔记.md`、
  `studyNotes/3.6_操作系统_备考笔记.md`
- 变更内容：基于对应原文提取 Markdown 并结合联网搜索，依次生成第3章剩余5节（3.2存储器系统、3.3输入输出系统、3.4指令系统、3.5多处理机系统、3.6操作系统）的完整备考笔记，每篇包含核心概念、高频考点、概念对比、模拟题、背诵知识点等标准结构。
- 操作 Agent：Claude

## [2026-05-24] 新增 — 3.3、3.4、3.6 原文提取（3篇）

- 变更文件：
  `books/Docx/3/3.3_输入输出系统_原文提取.md`、
  `books/Docx/3/3.4_指令系统_原文提取.md`、
  `books/Docx/3/3.6_操作系统_原文提取.md`
- 变更内容：从 `books/Split Chapters/第3章 计算机系统.pdf` 中分别提取 3.3（第13-19页）、3.4（第19-23页）、3.6（第28-50页）小节完整内容并整理为 Markdown。
- 操作 Agent：Claude

## [2026-05-24] 新增 — 3.2、3.5 原文提取（2篇，子Agent协助）

- 变更文件：
  `books/Docx/3/3.2_存储器系统_原文提取.md`、
  `books/Docx/3/3.5_多处理机系统_原文提取.md`
- 变更内容：从 `books/Split Chapters/第3章 计算机系统.pdf` 中分别提取 3.2（第3-12页）和 3.5（第24-28页）小节完整内容并整理为 Markdown（子 Agent 辅助完成）。
- 操作 Agent：Claude（子Agent协助）

## [2026-05-23] 新增 — 3.1 计算机系统概述备考笔记

- 变更文件：`studyNotes/3.1_计算机系统概述_备考笔记.md`
- 变更内容：基于 `books/Docx/3/3.1_计算机系统概述_原文提取.md` 原文内容并结合联网搜索，生成 3.1 计算机系统概述的完整备考笔记，包含核心概念（层次结构、冯·诺依曼体系、软件分类、固件）、高频考点（7条）、概念对比（5组）、模拟题（5道）及背诵知识点（10条）。
- 操作 Agent：Claude

## [2026-05-23] 新增 — 3.1 计算机系统概述原文提取

- 变更文件：`books/Docx/3/3.1_计算机系统概述_原文提取.md`
- 变更内容：从 `books/Split Chapters/第3章 计算机系统.pdf` 中提取 3.1 小节（计算机系统概述）完整内容并整理为 Markdown，包含 3.1.1 计算机系统层次结构、3.1.2 计算机系统硬件、3.1.3 计算机系统软件三个子节，提取范围为 PDF 第 1-2 页。
- 操作 Agent：Claude

## [2026-05-23] 重构 — 提取笔记模板至 references 并统一引用

- 变更文件：
  `.claude/skills/system-analyst-expert/SKILL.md`（修改）、
  `.claude/skills/system-analyst-expert/references/note-template.md`（新增）、
  `studyNotes/AGENTS.md`（修改）
- 变更内容：
  1. 将 SKILL.md 中内嵌的「输出格式」Markdown 模板提取为独立文件 `references/note-template.md`；
  2. SKILL.md 的「输出格式」节改为引用 `references/note-template.md`；
  3. `studyNotes/AGENTS.md` 的「正文结构建议」节同步引用同一模板文件，确保两处格式约束一致。
- 操作 Agent：Codex

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
