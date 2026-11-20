# 验证记录 / Validation record

版本：0.1.0  
日期：2026-11-20  
范围：本地虚构材料，离线模拟试用。

## 怎么执行的

两个独立 Codex 子代理分别测试英文与中文版本；它们未继承编写对话、未读取预期答案，也未读取对方结果。每个执行者读取对应语言的完整技能与原始输入，实际完成任务。两个执行者测试了两个项目，因此这些结果不是跨模型基准，也不是统计样本。

发布整理者随后阅读实际输出，按输入检查关键判断、边界和来源保留。没有人工改写执行者交付来制造通过结果。案例导读与首页是另外编辑的摘要。

- [英文输入](inputs/research.en.md) → [英文原始输出](runs/english.md)
- [中文输入](inputs/research.zh-CN.md) → [中文原始输出](runs/chinese.md)
- [显式边界检查](scope-checks.txt)

## 本次观察

| 检查 | 中文结果 | 英文结果 |
|---|---|---|
| 同一个项目的两个来源合为一项候选 | 通过 | 通过 |
| 把 macOS 13+ 与芯片要求分别检查 | 通过，条件推荐 | 通过，条件推荐 |
| 排除上传、付费导出、单语文件方案 | 通过 | 通过 |
| 不把 Linux／外部识别提供方的未知条件当作满足 | 通过 | 通过 |
| 区分文档支持与运行验证 | 通过 | 通过 |
| 移除合适候选后，不降低要求凑推荐 | 通过 | 通过 |

两种语言的翻译请求边界检查均认为此 Skill 不适用，并直接交付翻译。但这只是加载说明后的任务判断，**没有测试客户端自动发现或自动触发**。

独立试用发现用户的具体 macOS 版本未提供。首页与案例因此保留 macOS 13+ 的前提；没有把支持 Apple Silicon 简化为支持用户的全部设备条件。

## 文件检查

四份完整指令（两个项目、各中英版本）使用当前环境内置 skill-creator 的 quick_validate.py 检查格式。发布目录的本地链接、必要文件、单一技能入口和本机路径泄漏另外检查。

技能运行本身无需 Python；Python 仅用于这里的开发检查。格式检查与模拟行为试用是不同的证据。

## 还没有证明什么

- 没有量化“使用 Skill 比不使用提升多少”，没有无技能对照。
- 没有测试真实联网、外部账号、注册、购买、安装候选或写入云平台。
- 没有证明所有输入格式、长资料集、模型与客户端版本都稳定。
- 中文与英文各只进行一次主任务试用，不能据此声称成功率。
- 场景是虚构的，不能作为真实产品或上线项目的证明。

## 怎样复现

新开独立执行环境，只给对应语言的技能文件与输入材料，执行材料中的请求，保存自己的结果。不要先读本目录的 runs 或本页检查结论。随后用上述要求评审实际结果。表述、分类名称和排版可以不同，关键是判断依据、信息保留与任务范围。

## English summary

Two isolated Codex evaluators, one per language, received instructions and raw fictional inputs without expected answers or the authoring conversation. They did not browse, install candidate products or mutate source materials. The release editor reviewed the actual artifacts against the inputs.

Both executions consolidated the two WindowCaption sources, retained the macOS 13+ prerequisite, excluded hard failures, kept unknowns unresolved and gave no qualified recommendation when S1/S2 were removed. Recommendations remained documentation-based, not runtime-tested.

This is a small simulated forward-test, not an automatic-trigger test, cross-model benchmark, comparison against no skill, or verification of real products. The scope probes show how the loaded instructions handled translation-only requests, not how the host's selector behaves.
