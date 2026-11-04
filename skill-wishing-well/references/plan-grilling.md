# 计划推敲：在必要处追问，在明确处推进

[中文](#中文--chinese) | [English](#english)

## 中文 / Chinese

吸收用户指定 grill-me → grilling 的分轮追问、前置依赖和推荐答案思路，针对技能建设独立改写。不是原技能全文复制，不依赖外部技能或其工具；不继承强制委托、穷尽所有分支或一律暂停实施的规则。

## 选择强度

**轻量模式（默认）**：内部检查目标、关键假设、约束及验收。没有重要缺口便继续。发现会影响方案的取舍，集中提出少量必要问题；不打印全套问卷，不要求用户再定义“什么叫好”。

**深度模式（用户明确请求）**：围绕当前计划多轮挑战，逐步确认关键决定。态度直接但尊重，挑战假设而非评价用户；不靠反复反问或对抗语气制造深度。用户要求结束推敲时停止，并说明剩余重要未决项；没有得到答案不能伪装达成共识。

## 维护简明决策树

围绕任务真正需要的决定记录：问题、影响、依赖、依据、状态。状态只需“已确认／待调查事实／待用户决定／低风险默认／不适用”。简短任务可在上下文维护，无需创建文件或复杂系统。

先定目的和成功标准，再处理范围与约束，随后是实现取舍和验证；顺序受实际依赖约束，不要求套满类别。新答案可能让其他分支失效，及时删去不适用问题。用户改了目标，仅重开受影响决定。

区分三种内容：
- 可查事实：通过已有材料、文件、工具或公开来源调查。不要让用户回答文件在哪、接口是否存在等可查问题。工具不可用时说明缺口；有必要才索取用户独有资料。
- 专业实现选择：由代理基于证据推荐并说明理由。不要把选择复用/改造、文件结构等常规工作全部交给用户。
- 重要偏好：会影响结果、成本、等待、交互或验收且无法推导的取舍，才向用户提问。

调查可用授权工具独立完成；仅在宿主规则、任务范围和授权允许且确有收益时委托，不把“必须启动子代理”写成依赖。待调查事实属于未满足前置条件，其下游问题先不问。

## 一轮如何提问

选择前置条件已确定、答案会改变实现或验收的问题；相互依赖的问题不要同轮问。每轮默认不超过三问，优先最高影响项，其余待下一轮；用户明确要求完整清单时才展开。已确认的答案直接复用，不换措辞重问。

每题含：具体选择、推荐答案、主要代价及影响。让“同意”能够明确接受推荐，但不要把默认答案说成唯一正确答案。使用宿主的结构化提问工具（若可用且适合），否则编号提问。例如：

> Q1：是否先支持一个资料来源，再扩展多来源？
> 建议先支持一个，先验证输出准确性；代价是首版覆盖较窄。这决定首版接口及测试范围。

避免问“是否要高质量”“是否考虑风险”等没有真实取舍的问题。不要问用户能从材料直接推导的内容。关键事实不能用多选偏好代替。

提出问题后等待真实回答才推进依赖这些答案的工作；可并行处理不依赖答案且已授权的调查。低风险可逆细节可以用已说明的默认值继续，但记为假设；关键取舍、缺失事实和权限不能因超时默认同意。工具无回答也不证明用户认可。

## 吸收答案与结束

把答案改写成具体约束和验收行为，不只回复“收到”。检查答案是否产生冲突或新的高影响依赖；没有新证据，不重开已解决分支。

达到以下条件即停止拓展：目标及成功标准明确；会改变方案的范围/约束已定；关键未知有验证办法或清楚限制；常规实现有推荐选择；剩余低风险细节可默认。无需穷尽所有设想的边界情况。

- 轻量模式：简述重要决定（必要时），继续当前已授权任务，不额外设置“最终批准计划”步骤。
- 显式深度模式：汇总已确认取舍、默认值、重大残余风险及验收，询问共同理解是否准确。用户对当前轮全部关键建议明确同意且要求修改计划或执行时，视为相应理解已确认，不再重复总确认。
- 理解一致与执行授权分开：仅评审/计划请求不创建技能；明确构建请求在重要取舍已定后继续构建。安装、覆盖或对外行动仍服从当前会话授权和宿主权限。

用户明确“不再问，按你的判断执行”时，代理可决定通常属于偏好的取舍并注明假设；不能把不存在的事实补成真，也不能扩大授权。若缺口阻止可靠执行，说明最少必要信息，同时完成独立部分。

## 与许愿池其他环节衔接

默认在诊断和候选核验后推敲；会改变检索方向的歧义提前问。推敲不能替代公开候选搜索或回源核验；用户赞同方案也不能替代测试。输出的已确认约束进入建设简报与验收案例，避免多维护一份重复计划。

质量衡量：是否提前发现会改变实施的问题；答案是否落实到方案；是否减少返工，同时没有无效提问和延误。不以问题数量或访谈轮数表示质量，不虚构改善百分比。

---

## English

# Plan grilling: question where needed, proceed where clear

Independently adapted for skill construction from the round-based questioning, prerequisite dependencies, and recommended answers in the user-specified grill-me → grilling route. This is not a full copy, requires no external skill or tool, and does not inherit mandatory delegation, exhaustive branching, or unconditional pauses.

## Choose intensity

**Lightweight mode (default):** internally check goals, assumptions, constraints, and acceptance. Continue when no important gap remains. Ask a small number of consequential questions where needed, without printing an exhaustive questionnaire or making the user define quality again.

**Deep mode (explicit request):** challenge the plan over multiple rounds and settle critical decisions. Be direct and respectful; challenge assumptions, not the person. Repetition or confrontation does not create depth. Stop when requested and disclose remaining consequential issues; unanswered questions are not consensus.

## Maintain a compact decision tree

Track only decisions the task needs: question, effect, dependencies, evidence, and state. States are confirmed, factual investigation needed, user decision needed, low-risk default, or not applicable. Small tasks can keep this in context without files or elaborate systems.

Set purpose and success criteria before scope and constraints, then implementation and validation, following actual dependencies rather than filling every category. Remove branches invalidated by new answers. Reopen only affected decisions when the goal changes.

Distinguish three kinds of information:

- Discoverable facts: investigate materials, files, tools, or public sources. Do not ask the user for facts you can inspect, such as file locations or interface availability. Disclose unavailable tools and request user-only information when needed.
- Professional implementation choices: recommend based on evidence and explain the reason. Do not offload routine decisions about reuse, adaptation, or file structure.
- Consequential preferences: ask only when an uninferable choice affects outcome, cost, waiting, interaction, or acceptance.

Investigate with available authorized tools. Delegate only when host rules and task authorization allow it and it adds value; subagents are never a required dependency. Unresolved factual investigations are prerequisites, so defer their downstream questions.

## Conduct a round

Select questions whose prerequisites are settled and whose answers change implementation or acceptance. Do not batch dependent questions. Default to at most three per round, highest impact first; expand only when the user requests a full list. Reuse confirmed answers instead of rephrasing the same question.

Each question states concrete options, the recommendation, main cost, and effect. Make assent clearly accept a recommendation without suggesting it is the only valid option. Use a host structured-question tool when available and suitable, otherwise numbered questions. Example:

> Q1: Should the first version support one source before expanding to several? Recommended: one source to validate accuracy first; the tradeoff is narrower initial coverage. This determines the first interface and tests.

Avoid empty choices such as whether quality or risk matters. Do not ask what supplied material already answers. A critical fact cannot be replaced with a preference poll.

Wait for real answers before dependent work; continue independent authorized investigation. Use explicitly stated defaults for low-risk reversible details, marking them as assumptions. Timeout cannot settle critical choices, facts, or permission. No answer from a tool is not assent.

## Incorporate answers and stop

Translate answers into concrete constraints and acceptance behavior, not merely acknowledgments. Check for conflicts or new high-impact dependencies. Do not reopen settled branches without new evidence.

Stop expanding when the goal and criteria are clear, consequential scope and constraints are settled, critical unknowns have validation plans or explicit limits, routine implementation has a recommendation, and remaining low-risk details can default. Exhaustive hypothetical edge cases are unnecessary.

- Lightweight mode: briefly report important decisions if useful, then continue authorized work without a final-plan approval gate.
- Explicit deep mode: summarize confirmed tradeoffs, defaults, material residual risks, and acceptance, then confirm shared understanding. Explicit assent to all key recommendations plus an instruction to revise or execute already confirms that understanding; do not ask again.
- Keep understanding separate from execution authorization. Review-only or planning requests do not create skills. Authorized builds continue once critical choices are settled. Installation, overwriting, and external actions follow conversation authorization and host permissions.

When told to stop asking and use judgment, choose ordinary preferences and label assumptions. Do not invent facts or expand authorization. If a gap prevents reliable execution, identify the minimum missing information while completing independent work.

## Connect with the rest of the workflow

Normally scrutinize after diagnosis and candidate verification; clarify earlier if ambiguity changes search direction. Scrutiny does not replace public candidate search or original-source verification; user approval does not replace testing. Feed confirmed constraints into the construction brief and acceptance cases rather than maintaining a duplicate plan.

Judge whether scrutiny detects implementation-changing issues early, incorporates answers, and reduces rework without unnecessary questions or delay. Question count and interview rounds are not quality metrics; never invent improvement percentages.
