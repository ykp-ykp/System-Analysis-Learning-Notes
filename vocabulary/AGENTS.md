# AGENTS.md — vocabulary 目录操作规范

> 本文件适用于 `vocabulary/` 目录中的词汇整理与新增操作。

---

## 一、词条格式规范

新增单词或术语时，必须统一使用以下格式：

```text
中文释义（英文全称，英文简写）【音标】
```

示例：

```text
中央处理单元（Center Processing Unit，CPU）【/ˈsentər ˈprəʊsesɪŋ ˈjuːnɪt/】
```

要求：

1. 先写中文释义。
2. 中文释义后使用中文全角括号 `（）`。
3. 括号内依次写英文全称、中文顿号分隔的英文简写。
4. 音标使用 `【】` 包裹。

---

## 二、列表格式规范

1. `vocabulary/` 中新增的词条必须使用有序列表。
2. 列表编号必须采用 Markdown 标准有序列表格式，例如：

```markdown
1. 中央处理单元（Center Processing Unit，CPU）【/ˈsentər ˈprəʊsesɪŋ ˈjuːnɪt/】
2. 随机存取存储器（Random Access Memory，RAM）【/ˈrændəm ˈækses ˈmeməri/】
3. 只读存储器（Read Only Memory，ROM）【/riːd əʊnli ˈmeməri/】
```

3. 不得使用无序列表、手写编号样式或混合列表格式。

---

## 三、编码规范

1. `vocabulary/` 中所有 Markdown 文件默认使用 UTF-8 编码保存。
2. 如终端显示乱码，应先使用 UTF-8 方式重新读取后再继续编辑。
