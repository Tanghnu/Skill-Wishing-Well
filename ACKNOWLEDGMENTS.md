# 来源与设计参考

以下清单依据 2026-11-03 的开发调研记录整理，用于说明设计参考，不表示合作、认可或背书。链接可能随上游更新而变化。

| 来源 | 参考方向 |
| --- | --- |
| [Vercel find-skills](https://github.com/vercel-labs/skills/tree/main/skills/find-skills) | 从需求生成搜索关键词、发现能力 |
| [Universal Skill Finder](https://github.com/bibryam/universal-skill-finder) | 多源发现、候选身份与来源记录 |
| [dangogit skill-finder](https://github.com/dangogit/skill-finder) | 本地能力盘点与任务匹配 |
| [alibustami claude-skill-finder](https://github.com/alibustami/claude-skill-finder) | 读取候选原文、检查资源和许可 |
| [prompts.chat skill-lookup](https://github.com/f/prompts.chat/tree/main/plugins/claude/prompts.chat/skills/skill-lookup) | 搜索后读取完整技能内容 |
| [Google finding-google-skills](https://github.com/google/skills/tree/main/plugins/cloud/google-cloud-developer/skills/finding-google-skills) | 按需发现与原文核验 |
| [Anthropic skill-creator](https://github.com/anthropics/skills/tree/main/skills/skill-creator) | 示例任务、行为评估与反馈迭代 |
| Codex 环境提供的系统 skill-creator | 简洁入口、渐进披露和技能结构检查 |
| [Agent Skills 规范](https://agentskills.io/specification) | 技能目录和元数据格式 |

开发记录将本包记载为独立撰写的指令；发布目录未捆绑上述项目的脚本、资源、下载副本或执行依赖。本次发布准备未对全部上游文本逐句进行相似性比对，不能据此作全面权利清查保证。

来源说明不代替第三方许可。若以后复制、翻译或改编第三方受保护内容，应先核对对应版本的许可，并保留所要求的声明。

本项目不是第三方 SkillForge 项目的重命名版本。旧内部标识 `skill-forge` 已改为 `skill-wishing-well`。

## 1.1.0 补充 / Addition

用户指定的 grill-me → grilling 路由提供了分轮追问、前置依赖和推荐答案的设计思路，本包针对技能建设独立改写；不捆绑原包、不要求外部依赖，也不继承强制委托。未确认公开上游链接或固定版本，因此不推定具体作者或许可证。

The user-specified grill-me → grilling route informed round-based questions, prerequisite dependencies, and recommended answers. This package independently adapts those ideas for skill construction without bundling the original package, requiring it as a dependency, or inheriting mandatory delegation. No public upstream URL or fixed version was verified, so no specific author or license is inferred.

## English — Sources and design references

The preceding table records design references from development research dated 2026-11-03. It does not imply collaboration, approval, or endorsement. Links may change upstream.

| Source (links in the table above) | Design reference |
| --- | --- |
| Vercel find-skills | Task-derived search keywords and capability discovery |
| Universal Skill Finder | Multi-source discovery, candidate identity, and provenance |
| dangogit skill-finder | Local inventory and task matching |
| alibustami claude-skill-finder | Original-file, resource, and license checks |
| prompts.chat skill-lookup | Reading full skill content after search |
| Google finding-google-skills | On-demand discovery and original-source verification |
| Anthropic skill-creator | Example tasks, behavioral evaluation, and feedback iteration |
| System skill-creator supplied by the Codex environment | Concise entry points, progressive disclosure, and structural checks |
| Agent Skills specification | Directory and metadata format |

Development records describe independently written instructions. This distribution bundles none of those projects' scripts, resources, downloaded copies, or executable dependencies. Release preparation did not perform exhaustive sentence-level similarity comparisons against all upstream texts and does not establish a comprehensive rights audit.

Attribution does not replace third-party licensing. Before future copying, translation, or adaptation of protected material, check the relevant version's license and retain required notices.

This project is not a renamed third-party SkillForge project. Its former internal identifier `skill-forge` was changed to `skill-wishing-well`.
