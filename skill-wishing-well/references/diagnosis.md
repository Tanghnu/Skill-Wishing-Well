# 诊断与质量

[中文](#中文--chinese) | [English](#english)

## 中文 / Chinese

## 从证据形成问题解释

读取与当前困扰直接相关的材料、流程和已有能力。不要为了背景调查扫描整个用户目录。找出输入、处理动作、输出、失败点和重复频率；没有证据的原因标成假设，而不是用户事实。

把“每次整理材料都很麻烦”先解释为候选问题，例如重复分类、结论难追溯、输入格式不一致。通过当前材料区分原因，必要时只问具体事实，如“最近一次最耗时的是整理还是核对来源？”不要要求用户填写技术需求或选复用/新建。

## 由代理提出可检查标准

为实际任务选择少量高价值标准，写明检查输入、期望结果和判定方式：

- 有效：关键输入能够得到用户需要的输出，缺失信息不靠猜测填补。
- 有改善：与当前做法比较重复步骤、纠错次数或实际耗时；没有基线就只报告观察，不声称提升百分比。
- 可用：目标环境与依赖匹配，遇到失败能说明原因和下一步。
- 可维护：职责集中，避免复制已维护能力；引用资源可定位。
- 可信：结论与来源匹配，未验证项明确标出。

这些维度不是每次都要打印的检查表。不要用字数、候选数量、星标或形式漂亮代替任务质量。

例如用户希望反复把零散会议记录整理为行动项：建议目标是提取决定、行动、负责人、期限及原文证据。可用标准是每个行动项有来源位置；未明确的负责人和期限标未知；讨论中的建议不冒充已决定事项。真实会议内容未提供时先用明确标为示例的小样说明，不宣称已适配用户会议。

## 不确定性的处理

缺少用户偏好时提出推荐默认值及理由，在回复内展示小样。只有事实缺口会改变路线、无法安全推导或存在重要取舍时才询问。继续不依赖回答的调查与设计，不能用等待超时补齐权限或事实。

信息不足以构建可靠产物时，把依赖的最少信息说清楚；不要生成一个空泛 skill 后宣称完成。用户认可示例只证明该示例的体验，不证明所有输入都有效。

## 从诊断进入推敲

当存在重要取舍或用户要求挑战计划时，转入 [计划推敲](plan-grilling.md)。先提出质量目标，再询问会改变目标或实现的选择；不要把“用户认可”当作证据正确或测试通过。对已确认答案保留上下文，低风险偏好可以使用注明的默认值，关键事实和权限不能猜。

---

## English

# Diagnosis and quality

## Explain the problem from evidence

Read materials, processes, and capabilities directly related to the problem, not the user's entire directory. Identify inputs, processing, outputs, failure points, and recurrence. Label unsupported causes as hypotheses, not user facts.

Translate complaints such as “organizing materials is always tedious” into possible causes: repeated classification, poor traceability, or inconsistent formats. Distinguish them using available material. Ask concrete factual questions only when needed, such as whether organization or source checking took longest last time. Do not require technical specifications or ask the user to choose reuse versus new construction.

## Propose checkable standards

Choose a few valuable criteria and specify test inputs, expected results, and judgment methods:

- Effective: critical inputs produce needed outputs without inventing missing information.
- Improved: compare repeated steps, corrections, or actual elapsed time with the current method. Without a baseline, report observations, not improvement percentages.
- Usable: environment and dependencies fit; failures explain their cause and the next step.
- Maintainable: focused responsibilities, no duplication of maintained capabilities, and locatable references.
- Trustworthy: conclusions match sources and unverified aspects are explicit.

These are not a checklist to print every time. Length, candidate counts, stars, and appearance do not replace task quality.

For recurring extraction of action items from meeting notes, propose decisions, actions, owners, deadlines, and original evidence. Require source locations; mark unspecified owners and deadlines as unknown; do not present suggestions as decisions. Without real notes, use clearly labeled sample material and do not claim adaptation to the user's meetings.

## Handle uncertainty

For missing preferences, recommend defaults with reasons and illustrate them in the reply. Ask only when a factual gap changes the route, cannot safely be inferred, or involves a consequential tradeoff. Continue independent investigation and design; waiting does not supply facts or permissions.

If reliable construction is impossible, state the minimum missing information. Do not declare a vague empty skill complete. Approval of a sample establishes only that sample's experience, not validity for every input.

## Move from diagnosis to scrutiny

For consequential tradeoffs or explicit plan challenges, use [Plan grilling](plan-grilling.md). Propose quality goals first, then ask about choices that change goals or implementation. User approval does not establish factual correctness or passing tests. Retain confirmed answers. Mark low-risk defaults; never guess critical facts or permissions.
