# academic-defensiveness-trim

用于起草、修改和审校中英文学术论文的 Codex 技能。它处理一种常见问题：作者花了几句话表示自己足够谨慎，读者却仍然不知道结果是什么、判断依据在哪里、结论适用于谁。编辑时先问：**如果删掉这句话，读者具体会误解什么？** 会误解的，就保留那条信息；删去只是在重复作者态度的措辞。准确、自然的原句可以一个字也不改。

第一次使用可从下面的例子开始；要了解编辑判断，直接看[规则手册](references/rulebook.md)；要比较原文、改文和误改，见[编辑判例](references/decisions.md)和[整段与跨章节示范](references/worked-edits.md)。

## 快速上手：修改一段摘要

把以下文字直接发给 Codex。数字为演示用的虚构材料。

```text
$academic-defensiveness-trim 请改写下面的中文摘要结果，只返回可直接粘贴的正文。
已知：80名参加者中，60人完成了3个月随访问卷；其中18人自报睡眠改善。没有对照组。
原文：必须强调的是，对这些初步结果的解读应保持充分谨慎。我们并无意过度解读，
但这项课程有可能在一定程度上改善了参加者的睡眠状况。
```

一种合适的输出是：

> 80名参加者中，60人完成了3个月随访问卷，其中18人自报睡眠改善（18/60，30%）。

原稿把有限的观察写成了课程效果，再用几个“可能”缓冲。改文直接给出测量时间、信息来源和分母。30%指完成问卷的人；其余20人的睡眠变化未知。此处只要求报告结果，所以可以就此收句。如果要回答讨论中的另一个问题——“观察到的改善能否归因于课程”——没有对照组便是一条要明确写出的设计限制。

## 选对模式，再给材料

| 我想做什么 | 最有用的输入 | 会得到什么 |
| --- | --- | --- |
| 根据材料起草 | 写明章节、语言和核心问题，附结果表、访谈摘录、理论前提或研究方案中相关内容。 | 一段或一节可直接使用的文字。方案写拟做的工作，已有发现另行表述。 |
| 修改现有稿件 | 给出原文，保留相关表号、引文、上下文；说明术语、含义或结构中不可更改的部分。 | 先给修订正文；需要时再说明影响解读的改动。指定“只给正文”，就省去编辑说明。 |
| 只读审校或拟批注 | 提供带段落位置的稿件或摘录，明确是否允许重写。 | 以“位置／原句／判断理由／最小改法”定位问题。原本准确的段落可判为无需修改。 |

有目标期刊、作者样文或手工批注时，一并提供最相关的部分即可。比如“结果保留原量表名称，讨论首次出现时解释其含义”，比“写得自然些”更能约束改写。技能按最新的明确要求和作者批注处理风格；如果批注中的数字与表格不一致，会指出具体冲突，留给作者判定。只提供摘录也可以，但无法凭一段文字断定某项限制已在全文其他位置交代。

## 五条可直接使用的指令

1. **摘录审校。** `$academic-defensiveness-trim 只检查随后这两段摘录。请标出重复的自我辩解，说明哪些否定句应保留及原因；按原句位置给中文批注，不替我改写全文。`
2. **英文润色，仅交正文。** `$academic-defensiveness-trim Edit the following Discussion paragraph in English. Keep the original citations and distinguish self-reported symptoms from clinical diagnoses. Return only the revised paragraph.`
3. **整稿修改。** `$academic-defensiveness-trim 按附件中的作者批注修改全文。先核对中英文摘要、表格和结论是否指向同一人群及比较。交付完整修订稿；数值矛盾单列待核对位置，不代选一个数值。`
4. **从材料起草。** `$academic-defensiveness-trim 根据随后提供的访谈摘录写一段中文质性研究结果。用摘录支撑解释，保留相反意见；不推算群体比例，不添加受访者没说过的话。`
5. **回复真实审稿意见。** `$academic-defensiveness-trim Draft a reply in English. The reviewer asks whether we used an independent cohort. We used internal cross-validation only. Answer the question directly, then propose a separate sentence for the manuscript. Do not say the manuscript has already been revised.`

## 哪些地方值得改，哪些应该保留

| 原文出现什么情况 | 编辑时看什么 |
| --- | --- |
| 讨论每段都说结果“有待谨慎解读” | 找出各句的实际依据。不同结果如共有一个样本来源限制，可在局限部分交代；如果某项结果只在探索性分析中出现，探索性身份就应留在它旁边。摘要和图注可供独立阅读，必要限定可以重复。 |
| “我们绝无意声称……”之后接一长串未做的事 | 判断读者是否真会把本文读成这些主张。若只需知道研究做了什么，直接写设计。若审稿人确实问“是否外部验证”，回信应清楚回答“否”，并写明实际验证方法。 |
| 较差表现被解释为小样本、任务太难或标签有误 | 区分观察与解释。有相应检验时可报告其结果；没有时不能把理由写成已证实的原因。必要的话可明确提出假设，再说明怎样检验。 |
| 出现 *may*、“未发现”或否定句 | 先看它们是否界定推断。“未发现明确的组间差异”不等于“两组等效”；“在连续性假设下”可能是证明成立的条件。不要为减少限定词而改变命题。 |

同一原则要用不同的证据来落实。文献计量论文中，“摘要提及”限定的是文献记载；它不能证明原研究实际做过或没有做过某项分析。预测研究中，模型区分筛查标签的能力不同于诊断疾病的能力。理论或定性研究的依据可以是证明步骤、反例、史料或访谈语境，不要求每个判断都改成数字。申请书则要区分已有结果、下一步计划和预期结果。

技能可以看出原稿中的结论是否超过所给材料，也可以发现可见的口径冲突；它不能仅凭文字确认未提供的原始数据、实验过程、全文引用或研究质量。它不鉴定作者身份，不提供“AI率”。定稿时，作者仍应核对关键数字、引文归属和研究解释。

## 如何查阅工具包

| 文件 | 适合什么时候打开 |
| --- | --- |
| [SKILL.md](SKILL.md) | 查看技能实际执行的流程、输入约束和交付方式。 |
| [规则手册](references/rulebook.md) | 按12条规则判断某项表述应删、留、改、移到别处，还是返回作者核实。 |
| [编辑判例](references/decisions.md) | 在14个中英文例子中对照材料、原文、改文和理由，尤其留意那些应原样保留的句子。 |
| [整段与跨章节示范](references/worked-edits.md) | 观察如何重组一段论证，以及为何同一限制可能在摘要保留、在相邻正文段落中合并。 |
| [来源记录](references/sources.md) | 核对参考的上游版本、设计取舍和上游许可原文。 |

## 安装、更新与验证

解压 ZIP，找到直接包含 `SKILL.md` 的 `academic-defensiveness-trim` 文件夹。把**整个文件夹**复制到运行 Codex 的环境中，保留 `agents/`、`assets/` 和 `references/`。技能本身无需额外软件包，也不用安装上游项目。个人技能可以跨项目使用；仅供某一项目使用的技能放在项目内。

| 使用位置 | 安装后应能找到的文件 |
| --- | --- |
| Windows 原生 Codex | `%USERPROFILE%\.agents\skills\academic-defensiveness-trim\SKILL.md` |
| macOS、Linux 或 WSL 中运行的 Codex | `~/.agents/skills/academic-defensiveness-trim/SKILL.md` |
| 单一项目 | 项目根目录下的 `.agents/skills/academic-defensiveness-trim/SKILL.md` |

如果目录不存在，先创建它。WSL 中的 `~` 是 Linux 用户的主目录，Windows 原生和 WSL 的个人目录不同。**更新已有安装时**，先把自己的改动备份到技能搜索目录以外，再把原技能文件夹整体换成新版。不要把备份和新版并排放在技能目录，也不要把新版套进同名的旧文件夹。

在 Codex CLI 中输入 `/skills` 查找名称，或在新会话中试用上面的快速示例。找不到技能时，先核对实际运行环境和表中路径；能找到技能但打不开判例时，检查是否只复制了 `SKILL.md`。参见[Codex 官方技能文档](https://developers.openai.com/codex/skills)。

## 手动上传到 GitHub

解压后，在目标仓库选择 **Add file → Upload files**；空仓库可以点击 **uploading an existing file**。

- **独立技能仓库：** 打开解压后的 `academic-defensiveness-trim` 文件夹，把**里面的全部文件和子目录**拖到仓库根目录。提交前应能看到根目录的 `README.md`、`SKILL.md` 和三个子目录；只上传 ZIP 不会在仓库首页展示这份说明。
- **多技能集合：** 打开仓库中存放其他技能的目录，拖入**整个** `academic-defensiveness-trim` 文件夹，使它与其他技能并列，避免覆盖集合自己的 README。

本技能参考了 [Academic Defensive Writing Auditor](https://github.com/Worigin0314/academic-defensive-writing-auditor) 对预防性辩解的分析，以及 [Academic Humanizer](https://github.com/AIScientists-Dev/academic-humanizer) 对证据强度和作者语气的处理。发布时将[来源与许可记录](references/sources.md)一并保留。
