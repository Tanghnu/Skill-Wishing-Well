# 发现与证据

[中文](#中文--chinese) | [English](#english)

## 中文 / Chinese

## 工具与来源

新建技能前的公开搜索是必经步骤，例外以 SKILL.md 为准。先将需求概括为不含敏感信息的任务、交付物与环境关键词，再实际调用搜索工具；只检查本地目录、凭记忆列项目或宣告“准备搜索”均不算完成。搜索用于选择实现路径，不自动授权安装候选。

先使用会话给出的目录和工具元数据，再读取相关候选。根据宿主实际能力使用搜索、仓库读取、注册表连接器或文件读取；不要假设工具名或自行安装 CLI、MCP、模型及搜索后端。

联网发现可从 skills.sh、相关官方技能仓库和公开 GitHub 原文入手；这些是起点，不是静态可信白名单。第三方目录用于扩大覆盖，具体能力回到原始文件检查。只有实际接口存在且满足任务时才使用可选后端，遵守其输出契约，不把别的 skill 的内部脚本当稳定 API。没有联网能力时报告局限，仍可分析本地能力或已提供内容。

从任务、交付物和环境约束生成互补关键词，中文需求补充英文术语。普通发现默认两轮，每轮最多三个查询；关键缺口仍未解决可再补一轮。用户要求深入搜索时扩大预算。已有充分证据则提前结束；源不可访问不应无限重试，也不是绕过权限的理由。

新建前至少完成一轮针对具体需求的公开搜索。发现相关候选后，读取最相关候选的原始 SKILL.md；仅能看到摘要或原文无法访问时，明确标为未核验。使用任务关键词及 skill/SKILL.md 等定位词；第一轮偏题或无结果时，换同义词或来源补查，不能用一次过窄查询支持“没有现成方案”。保留搜索词、来源、原文核验状态及选择理由，简短回复即可，不强制另建报告。

## 候选记录与身份

按需要记录：名称、原始仓库及技能目录、版本或提交（未知则明确）、发现渠道、读取日期、任务覆盖、依赖、限制、相关文件和证据状态。不必为几条候选创建数据库或 JSON。

只有明确相同的仓库、目录及版本才合并记录，并保留全部发现渠道；同名不同源、不同版本、相似内容不能自动合并。引用未知版本的同一路径可以标为疑似同一目标，不能冒认相同字节。确认原作者或上游需要明确来源证据。

## 逐层核验

区分：

1. 仅发现：只有摘要或索引记录。
2. 原文已读：已读取实际 SKILL.md，识别适用边界。
3. 相关资源已查：已读取支撑关键能力的引用、配置或脚本；记录未覆盖文件。
4. 环境已检查：目标宿主、工具和依赖已检查，注明只是文档兼容还是本机检测。
5. 任务已实测：记录运行输入、环境、结果和测试范围。

这些不是安全评级。明确推荐关键能力需要相应原文支持；暂时无法读取者保留为待核验线索，不包装成已验证首选。未知不等于失败，未运行不等于不可用。

先核验最相关的少量候选；若均不适配，再核验替代者。不能因先读了五个就忽略已发现的更合适候选。

## 选择与输出

硬约束优先。比较实际覆盖、操作清晰度、依赖成本、维护证据及适配工作量；低热度但符合需求者可以优于热门者。来源身份和许可证可验证并不保证安全。注册表安装量、仓库星标各自标明含义和来源，不跨来源相加或换算成质量分。

默认精选最多 3–5 个，实际合格数量不足则减少；用户要求广泛列表时展开。每项解释适用情况、关键限制、证据程度和原始链接，最后给出推荐路径。源失败、搜索范围与未解决缺口要保留。

---

## English

# Discovery and evidence

## Tools and sources

Public search before creating a skill is required, subject to the exceptions in SKILL.md. Abstract the need into nonsensitive task, deliverable, and environment terms, then actually invoke search. Local inspection, remembered projects, or announcing an intention to search do not count. Discovery informs implementation; it does not authorize installation.

Start with supplied skill catalogs and tool metadata, then read relevant candidates. Use actual host search, repository readers, registry connectors, or file readers. Do not assume tool names or independently install CLIs, MCP servers, models, or search backends.

Possible starting points include skills.sh, relevant official skill repositories, and original public GitHub files. These are not permanent trusted allowlists. Third-party directories broaden coverage; verify capabilities in original files. Use optional backends only when their interfaces exist and fit the task, respecting their output contracts. Another skill's internal script is not a stable API. Without networking, state the limitation and analyze local or supplied material.

Generate complementary queries from the task, deliverable, and constraints, adding English terms to Chinese requests. Default to two rounds of at most three queries each; add one round for an unresolved critical gap. Expand the budget for explicit deep-search requests. Stop early when evidence suffices. Do not retry inaccessible sources indefinitely or use failure to justify bypassing permissions.

Before new construction, complete at least one task-specific public-search round. Read the most relevant candidate's original SKILL.md when candidates are found; summaries alone or inaccessible originals remain unverified. Use task terms plus locators such as skill or SKILL.md. If the first round misses the topic or finds nothing, vary synonyms or sources; one overly narrow query cannot establish no ready-made solution. Preserve queries, sources, original-file verification status, and selection reasons, usually in a brief reply rather than a mandatory report.

## Candidate records and identity

Record as needed: name, original repository and directory, version or commit (explicitly unknown when unavailable), discovery channel, reading date, coverage, dependencies, limitations, relevant files, and evidence status. A few candidates need no database or JSON.

Merge records only for demonstrably identical repository, directory, and version, preserving all discovery channels. Identical names, different versions, or similar content do not establish identity. The same path with unknown versions may be a suspected match, not verified identical bytes. Attribution to an original author or upstream requires source evidence.

## Verify in layers

1. Discovered only: summary or index entry available.
2. Original read: actual SKILL.md inspected and applicability understood.
3. Supporting resources checked: relevant references, configurations, or scripts inspected; uncovered files recorded.
4. Environment checked: host, tools, and dependencies assessed; distinguish documentation compatibility from local inspection.
5. Task tested: inputs, environment, results, and test scope recorded.

These are not security ratings. Strong recommendations for critical capabilities require corresponding original-source evidence. Inaccessible candidates remain leads, not verified first choices. Unknown does not mean failed; untested does not mean unusable.

Check the most relevant few candidates first, then alternatives if needed. An arbitrary count of inspected candidates must not exclude a better candidate already discovered.

## Selection and output

Prioritize hard constraints. Compare actual coverage, clarity, dependency costs, maintenance evidence, and adaptation effort. Less popular candidates may fit better. Verified identity and licensing do not guarantee safety. Label registry installs and repository stars with their meanings and sources; do not combine them into quality scores.

Usually shortlist at most three to five candidates, fewer when fewer qualify; expand for a requested broad list. Explain fit, limitations, evidence level, and original links, then recommend a path. Preserve source failures, search scope, and unresolved gaps.
