# Skill许愿池 / Skill Wishing Well

**v1.1.0 · `skill-wishing-well` · 中文 / English**

## 中文

从实际困扰出发，诊断能力缺口，提出目标与验收标准，按需推敲关键假设，搜索和评估现有技能，再按授权复用、组合、改造或新建。

这是供 AI 助手读取的指令型技能，是独立社区项目，不是 OpenAI 官方产品；提及第三方项目不表示背书。本项目借助 AI 编写与整理。

### 用途与边界

- 寻找或比较技能，核对实际覆盖、依赖和限制。
- 将工作方法固化为可用技能，或改造已有技能。
- 默认轻量检查；明确要求深度推敲时分轮提问，每轮默认最多三问，包含推荐与代价。
- 显式调用处理具体任务时，即使仅使用一次也默认固化为技能；明确的只搜索、只计划或不写文件限制优先。
- 普通知识问答和抱怨不会自动触发建设；建设不自动授权安装或发布。

### 安装与使用

下载仓库或发布包，将完整 `skill-wishing-well` 文件夹放入宿主的个人技能目录。Codex 默认位置为 `~/.codex/skills/`；设置了 `CODEX_HOME` 时使用其下的 `skills` 目录。先备份已有同名文件夹，再替换；不要把整个仓库当作技能目录安装。旧内部标识 `skill-forge` 应移出技能目录备份，避免重复加载。

在宿主重新发现技能后调用：

> 使用 $skill-wishing-well，先深度推敲这个技能计划，再根据已确认的取舍完成构建和验证，先不要安装。

> 使用 $skill-wishing-well 比较这两个技能，核对来源、依赖和覆盖，只给建议，不创建文件。

### 依赖与验证

技能包只有 Markdown 和 YAML，无可执行脚本、额外运行库、内置密钥或 grill-me/grilling 安装依赖。实际搜索、文件操作和权限由宿主提供；宿主或第三方服务可能另行收费。其他宿主的兼容性尚未验证。

中文升级版完成结构检查及六种合成情境的独立下一步响应模拟；双语修订完成引用、元数据长度、文件与压缩包摘要检查，没有重跑上述行为模拟。尚未验证真实用户连续访谈、跨设备或跨宿主体验，也没有证据证明普遍质量提升。搜索失败不代表不存在合适技能。

反馈请提供宿主版本、脱敏请求、预期与实际行为、是否显式调用；勿公开密钥或客户资料。

## English

Start from a practical problem, diagnose capability gaps, propose goals and acceptance criteria, examine consequential assumptions as needed, discover and assess existing skills, then reuse, compose, adapt, or build within authorization.

This instruction-based skill is an independent community project for AI assistants, not an official OpenAI product. References to third parties do not imply endorsement. AI assisted its writing and organization.

### Uses and boundaries

- Find or compare skills by actual coverage, dependencies, and limitations.
- Capture working methods as usable skills or adapt existing ones.
- Use lightweight checks by default; explicit deep scrutiny proceeds in rounds of at most three questions by default, with recommendations and costs.
- Explicit invocation for a concrete task defaults to capturing its method as a skill, even for one-time use. Explicit search-only, plan-only, and no-files limits take priority.
- General questions and complaints do not automatically trigger construction. Building does not authorize installation or publication.

### Installation and usage

Download the repository or release package and place the complete `skill-wishing-well` folder in your host's personal skills directory. Codex defaults to `~/.codex/skills/`; if `CODEX_HOME` is set, use its `skills` directory. Back up an existing folder before replacement. Do not install the entire repository as the skill folder. Move the old internal `skill-forge` folder outside the skills directory as a backup to prevent duplicate loading.

After the host rediscovers the skill, invoke:

> Use $skill-wishing-well to scrutinize this skill plan deeply, then build and validate it from the confirmed decisions. Do not install it yet.

> Use $skill-wishing-well to compare these two skills, checking sources, dependencies, and coverage. Only recommend; do not create files.

### Dependencies and verification

The skill contains only Markdown and YAML, with no executable scripts, additional runtime libraries, embedded keys, or required grill-me/grilling installation. Actual searches, file operations, and permissions depend on the host. Host or third-party services may charge separately. Compatibility with other hosts remains unverified.

The Chinese upgrade received structural checks and independent next-response simulations for six synthetic scenarios. The bilingual revision received reference, metadata-length, file, and ZIP hash checks; those behavior simulations were not rerun. Continuous real-user interviews, cross-device and cross-host experience remain unverified; no evidence establishes general quality improvement. Failed discovery does not prove suitable skills do not exist.

For feedback, provide the host version, sanitized request, expected and actual behavior, and whether invocation was explicit. Never publish keys or customer materials.

## 文件结构 / Package structure

```text
skill-wishing-well/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── construction.md
    ├── diagnosis.md
    ├── discovery.md
    ├── plan-grilling.md
    └── validation.md
```

## 来源与许可 / Sources and license

[来源说明 / Acknowledgments](ACKNOWLEDGMENTS.md) · [版本记录 / Changelog](CHANGELOG.md) · [MIT License / MIT 许可证](LICENSE)

版权 / Copyright © 2026 Tanghnu。使用、修改、再分发和商用须保留版权及许可声明；不授予第三方项目、服务或商标权利。 / Use, modification, redistribution, and commercial use require retaining the copyright and permission notice. No rights to third-party projects, services, or trademarks are granted. Full terms are in LICENSE.
