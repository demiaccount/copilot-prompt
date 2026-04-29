微软copilot

1.文本生成的四个要素：角色定视角，结构定逻辑，深度（每点给出可执行动作+数据占位）定价值，格式定效率

2.图像生成的通用prompt模板
【场景描述】【文字内容（可选）】【风格】【光影/视角】【宽高比】

一、PPT 大纲生成

场景背景

| 员工需要为某公司某款车型下半年营销计划制作一份 PPT，但不知道如何组织内容。希望通过 Copilot 快速生成大纲。 |
|:---|


普通 Prompt（反面案例）

| 帮我写一份某公司某款车型下半年营销计划的 PPT |
|:---|



| 输出内容空洞，只有“市场概况、策略、预算”等标题，无具体数据和建议。 |
|:---|


高级 Prompt（正面案例）

| 你是某公司中国营销策略专家。充分通过网页搜索，充分调研，特别关注竞品信息，请为 某车型 下半年营销计划生成一份 PPT 大纲。  要求： - 每页包含：核心观点（一句话）+ 数据支撑（用[占位]标注）+ 具体执行动作 - 分页方式：用“第1页：” “第2页：” 依次列出 - 至少包含：市场分析、竞品对比（其他公司某车型/其他公司某车型）、核心策略、执行路线图  请直接输出大纲内容。 |
|:---|



| 输出包含可执行建议、数据占位和清晰结构。 |
|:---|

二、Excel 分析
场景背景

| 员工有一份 2026 年 Q1 各区域销量 Excel 表格（含区域、Q1销量、Q4销量），需要分析环比、排名，并得出业务结论。 |
|:---|


普通 Prompt（反面案例）

| 分析这份销量数据 |
|:---|



| 输出只有总销量、平均值，无环比、无排名、无结论。 |
|:---|


高级 Prompt（正面案例）

| 你是某公司中国销售运营分析师。请基于上传的 Excel（2026年Q1各区域销量）完成以下任务：  1. 计算每个区域的 Q1 销量、环比 Q4 增长率 2. 找出增长率最高和最低的区域 3. 给出 2 条可能的原因推测（结合实际业务） 4. 输出一个表格，包含：区域、Q1销量、环比增长率、排名 5. 最后用一句话总结：哪个区域需要重点关注  注意：如果缺少数据，请用“待补充”标注，不要编造。 |
|:---|



| 输出包含完整表格、排名、原因推测和行动指向。 |
|:---|






三、Word 会议纪要
场景背景

| 员工刚开完售后满意度提升会议，有零散的会议记录，需要整理成正式会议纪要，包含待办事项和负责人。 |
|:---|


普通 Prompt（反面案例）

| 帮我写一份会议纪要 |
|:---|



| 输出流水账，无议题、结论、待办事项区分。 |
|:---|


高级 Prompt（正面案例）

| 你是某公司售后业务助理。请将以下会议记录转化为正式会议纪要。  要求： - 结构：议题 → 结论 → 待办事项（负责人+截止日） - 待办事项用 [ ] 标注状态（[ ] 表示未开始） - 语气：内部专业，明确  会议记录原文： [张总]：Q1售后满意度 NPS 从 72 降到 68，主要是等待时间太长和配件缺货。 [李经理]：平均等待时间 45 分钟，目标 30 分钟。缺货集中在刹车片和机滤。 [王主管]：SA 话术不统一，客户抱怨时不知道怎么安抚。 [张总]：三件事：1）优化预约流程，减少等待；2）缺货配件建立安全库存；3）本周五前出安抚话术。下周三再开会检查。 |
|:---|



| 输出包含清晰议题、结论、带负责人和截止日的待办列表。 |
|:---|

四、邮件生成
场景背景

| 员工需要向各区域经理发送邮件，催促提交周报。要求语气专业但温和，包含截止时间和支持选项。 |
|:---|


普通 Prompt（反面案例）

| 写邮件给区域经理，催他们交周报 |
|:---|



| 输出语气生硬（“请尽快提交”），无背景、无截止时间。 |
|:---|


高级 Prompt（正面案例）

| 你是某公司销售运营总监。请写一封邮件给区域销售经理。  背景：本周周报需要用于月度 executive review，数据完整性非常重要。  语气：专业但温和，强调重要性。  内容要求： - 提醒截止时间（周四 18:00） - 附加周报模板链接（用 [模板链接] 占位） - 询问是否需要支持 - 最后加一句“感谢配合”  邮件格式：包含主题、称呼、正文、落款。 |
|:---|



| 输出包含完整背景、礼貌语气、具体截止时间和支持选项。 |
|:---|

五、图像生成 —— PPT 背景图

场景背景

| 员工需要一张某公司主题的 PPT 背景图，要求深色、科技感、左侧留白用于放文字，可直接设为幻灯片背景。 |
|:---|


Prompt（正面案例）

| Create a 16:9 image for PowerPoint background, deep blue to black gradient, subtle glowing lines forming a road perspective, one company logo silhouette in bottom right, left side 40% dark solid area for text, modern corporate style. |
|:---|



| 生成图片，设为 PPT 背景（右键 → 设置背景格式 → 图片填充）。 |
|:---|


六、图像生成 —— 活动海报
场景背景

| 市场部需要为“JOY FEST 2026”活动制作一张宣传海报，包含标题、日期、霓虹风格背景。 |
|:---|


Prompt（正面案例）

| A corporate event poster, title "JOY FEST 2026" in large bold white letters, subtitle "JUNE 20-22 | SHANGHAI", neon purple and blue gradient background, silhouette of a car and crowd, 16:9, modern festival style. |
|:---|



| 生成带文字的海报，文字清晰、风格鲜明。 |
|:---|


七、图像生成 —— 社交媒体截图
场景背景

| 市场部需要模拟一个 TikTok 爆款视频截图，用于创意提案，包含高点赞量、高播放量和热门评论。 |
|:---|


Prompt（正面案例）

| A TikTok video screenshot, driving POV from a BMW i5, view count "2.5M", heart icon "189k", caption "Highway autopilot is insane", verified blue check, 9:16 ratio. |
|:---|



| 生成带有社交平台 UI 元素（点赞、播放量、蓝V认证）的截图，逼真可用。 |
|:---|


八、图像生成 —— 复古旅行海报
场景背景

| 品牌部门需要一张复古风格的旅行海报，用于文化宣传或内部装饰，融合某公司元素和地中海风光。 |
|:---|


Prompt（正面案例）

| Amalfi Coast vintage travel poster, hand-drawn pencil illustration, pastel Mediterranean colors, Italian coastline with lemon trees and sailboats, text "DRIVE THE DREAM" in elegant serif, One company logo small at bottom, 1950s tourism aesthetic, 3:4 ratio. |
|:---|



| 生成具有艺术感和品牌调性的复古海报。 |
|:---|


九、图像生成 —— UI 模拟
场景背景

| 产品团队需要展示某公司车主 App 的界面设计概念，用于汇报或用户手册配图，要求深色模式、关键信息突出。 |
|:---|


Prompt（正面案例）

| iPhone 17 Pro mockup showing a company owner app dashboard, dark mode, large "MY i5" text, battery range "412 km", tire pressure all green, bottom navigation with 4 icons, clean modern UI. |
|:---|



| 生成逼真的手机 App 界面，包含数据卡片和底部导航栏。 |
|:---|

生成prompt 的prompt
你是一个 Prompt 工程师。请通过多轮提问帮我生成一个专业 Prompt。
依次问我：
1. 任务类型（PPT大纲/Excel分析/Word报告/邮件/搜索聚合/图像生成）
2. 目标受众
3. 期望的内容深度或风格
4. 输入信息（如有）
5. 输出格式（纯文本/表格/列表/图片比例）
6. 最需要避免的问题
最后输出完整的 Prompt。
