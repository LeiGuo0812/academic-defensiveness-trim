# 编辑判例：从原文到可用稿

以下 14 例均为本技能自拟的练习。数字、研究情境和材料只在各例内部成立，不是实证引文，也不能补入真实稿件。每例的“已有材料”是编辑可以使用的全部依据。先独立判断原文中哪一句在报告事实、哪一句在解释、哪一句仅在表态，再看改文。中英文例句分别按各自语言写作，不要求逐词对应。

## 按问题查找

| 我要判断…… | 对应判例 |
| --- | --- |
| 两条限定能否合成一条；不同位置的重复该不该删 | [E01 筛查标签与内部验证](#e01) · [E12 摘要与图注](#e12) |
| 怎样报告较差结果、组内检验或阴性结果 | [E02 对照条件](#e02) · [E05 两个组内检验](#e05) · [E06 区间与等效](#e06) |
| 哪些观察能写，哪些因果或机制判断过头了 | [E03 摘要未报告](#e03) · [E04 同次访视](#e04) · [E13 神经影像整段修订](#e13) · [E14 文献共现与计数冲突](#e14) |
| 定性材料、理论前提和后续问题怎么处理 | [E07 档案来源](#e07) · [E08 理论反例](#e08) · [E09 编码分歧](#e09) |
| 何时直接回答质疑；如何写未开展的研究 | [E10 审稿回复与正文](#e10) · [E11 基金申请](#e11) |

<a id="e01"></a>
### E01｜预测模型：保留两个不能互相替代的限定

**已有材料：** 资料来自一家医院；只做了内部交叉验证。预测标签是筛查问卷是否达到阈值，没有临床诊断标签。原段正在讨论是否可以辅助诊断。

**原文：** “为避免误解，我们绝无意声称该模型已经可用于诊断。尽管表现令人鼓舞，必须谨慎指出，我们仅做了内部验证，而且标签并不是诊断。因此其临床意义仍需谨慎看待。”

**改文：** “模型在同一家医院的数据上接受了交叉验证，预测目标是筛查问卷是否达到阈值。现有分析没有评估模型在新医院的表现，也没有检验它识别临床诊断的能力。”

**判定：** 删掉作者表态和没有指标支撑的赞誉，留下两项范围不同的事实。新医院的独立样本回答的是能否迁移；临床诊断标签决定能否评估诊断表现。“尚需外部验证”单独一句不能同时表达两件事。如果只是在方法中交代模型任务，并未讨论诊断应用，写到改文第一句就够了。

<a id="e02"></a>
### E02｜英文方法与结果：撤掉“公平”和借口，保留失利

**已有材料：** 两种模型使用同一训练集，也在同一留出集上评价。只有准确率可用；未分析标签噪声或证实差异的原因。

**Original:** “For the sake of fairness, both models used the same training set. Our model understandably suffered from noisy labels, but its performance remains promising: it achieved 71% accuracy versus 76% for the reference model.”

**Revision:** “Both models used the same training set. On the held-out set, accuracy was 71% for our model and 76% for the reference model.”

**判定：** 相同训练集是读者可核对的条件；“公平”是对整个比较的评价。保留具体条件和参照模型，连同不利结果一起报告。若前一句已在方法部分交代，结果段可直接从 “On the held-out set” 开始。把 “noisy labels” 改成 “possibly noisy labels” 仍凭空引入原因；反过来声称标签没有噪声也无依据。

<a id="e03"></a>
### E03｜文献摘录：中文否定句原样保留

**已有材料：** 只审阅了摘要。在 12 篇提到疼痛的报告中，有 3 篇交代评估时间；其余 9 篇没有提供足以判断评估实施情况的信息。

**原文与交付稿（不改）：** “12篇报告提到疼痛，只有3篇给出评估时间。其余9篇是否开展过疼痛评估，仅凭摘要无法判断。”

**判定：** 第一处数字的单位是报告，不是受试者。第二句区分“看不见相关信息”和“研究未实施”，提供了第一句没有表达的证据范围。**反例：** “其余9篇未开展疼痛评估。”删掉的是资料来源的限制，得到的却成了一项新的研究事实。即使局限一节提到只读摘要，这里的限定仍有助于独立理解该结果。

<a id="e04"></a>
### E04｜英文观察研究：在相应的主张旁写明测量与时序

**已有材料：** 在同一次访视收集自报睡眠时长和疲劳评分；睡眠时长较短与疲劳评分较高相关。原讨论提出“何者先发生”，没有时间顺序或干预资料。

**Original:** “We wish to stress that no causal mechanism is being claimed. Shorter sleep may possibly be related to tiredness, but the reader should exercise considerable caution when interpreting this finding.”

**Revision:** “Shorter self-reported sleep duration was associated with higher fatigue scores at the same visit. The measurements do not establish whether shorter sleep preceded fatigue.”

**判定：** “was associated with” 直接报告分析结果；“self-reported” 界定实际测量，“at the same visit” 限定时序。第二句在讨论先后关系时有用。如果任务只要求写结果句，且不存在时序主张，交付第一句即可。不要把 “was associated with” 换成 “may contribute to”：后者虽有 “may”，已开始解释成因。

<a id="e05"></a>
### E05｜组内检验：收回未做直接比较的疗效排名

**已有材料：** 已确认 A 组评分在干预后较干预前降低（组内检验 p = 0.02），B 组前后差异未达统计学显著（p = 0.18）。没有两组变化量的直接比较，也未提供组别与时间的交互检验。

**原文：** “虽然并不能排除其他可能，但 A 组的显著改善和 B 组的不显著结果可能意味着 A 方案效果更好。”

**改文：** “A组干预后的评分低于干预前（p = 0.02）；B组前后差异未达统计学显著（p = 0.18）。这两项检验均在组内进行，未直接比较两组的评分变化。”

**判定：** 两个 p 值回答的是两个组内问题；其显著与否不直接回答组间问题。“可能更好”或“呈优势趋势”仍把比较对象写错。“B组没有改善”也超出了现有结果。若实际有预设的组间对比，应改报其估计及不确定性；材料未给时，不代算也不补造。

<a id="e06"></a>
### E06｜英文阴性结果：给出估计和区间，不把它改写成等效

**已有材料：** 结局是给定随访期内发生过该事件的参与者比例之差（A 组减 B 组），估计为 −1 个百分点，95% 置信区间为 −6 至 4 个百分点。研究没有预设等效界值，也未做等效检验。

**Original:** “Although the comparison did not reach significance, our reassuring findings show that the two approaches are essentially equivalent.”

**Revision:** “The estimated risk difference (group A minus group B) was −1 percentage point (95% CI, −6 to 4 percentage points). The interval includes differences in either direction.”

**判定：** 区间跨过零，直接说明这组数据没有确定差异方向。无须再加一句笼统的 “must be interpreted with caution”。“There was no difference” 将不确定性改写成相同；“clinically negligible” 又引入了材料中没有的临床界值。若原问题就是等效性，可另写 “Equivalence was not evaluated.”；不应把该句设为所有阴性结果的固定结尾。

<a id="e07"></a>
### E07｜质性与历史材料：保留对材料来源的质疑

**已有材料：** 现存 8 封来信均由一个反对改革的组织保存；其中 6 封写明反对增加登记费用。既无支持改革者的独立材料，也不知道原有来信如何筛选留存。

**原文：** “虽然很难排除各种偏倚，但民众很可能普遍反对改革，尤其是登记费用的上涨。我们的解释仍需谨慎。”

**改文：** “在反对改革的组织所保存的8封来信中，有6封明确反对增加登记费用。这些来信记录了反对意见所针对的一项具体条款；仅凭这个组织保存的材料，无法判断这种意见在当地居民中有多普遍。”

**判定：** 材料仍足以说明反对者关心的内容。应收回的是从来信推断当地居民态度的判断，而不是把所有材料都说成“不可靠”。写出保存者的立场可以进一步解释材料为何可能偏向一侧；不能据此断言该组织曾故意删除支持意见，也不能把反对一项费用等同于反对整项改革。

<a id="e08"></a>
### E08｜英文理论论证：有作用的反例原样保留

**已有材料：** 段落讨论“单调递增且有上界的实数序列收敛”，目的是解释为什么需要有上界这一条件。

**Original and final (unchanged):** “Monotonicity alone does not ensure convergence. The sequence xₙ = n is increasing and has no finite limit.”

**判定：** 第一句准确界定被否定的命题；第二句给出反例。它们不是作者为防止被批评而预先声明“我们没有证明什么”。改成 “The convergence result should be interpreted cautiously” 会同时丢掉必要条件和反例。即使用户要求精简，保留这两句比增加一句立场中性的概括更能服务论证。

<a id="e09"></a>
### E09｜从材料起草讨论：提出下一步，却不预先写出原因

**已有材料：** 两位编码员的主题归类分歧集中在匿名帖；其中部分帖子缺少前文。没有对照前文完整与缺失的匿名帖，也没有分析编码员如何作出判断。作者要求一句观察、一个后续问题。

**候选原文：** “匿名造成语境缺失，进而显著降低了编码一致性。这一重要发现仍需在更多研究中进一步验证。”

**可直接使用的讨论：** “两位编码员对主题归类的分歧集中在匿名帖。可在匿名帖中比较前文完整与缺失的帖子，检验分歧是否更常出现在缺少前文时。”

**判定：** 第一句只陈述观察；第二句把“缺少语境”保留为待研究的解释，并给出了与之相符的比较。材料不支持“匿名造成”“显著降低”或“与实名帖相比”的判断。若任务只是写结果而非讨论，应停在第一句，不主动加后续研究。

<a id="e10"></a>
### E10｜英文审稿回复与论文正文：同一个事实，两种写法

**已有材料：** 审稿人明确问 “Was an independent cohort used?”。唯一可核实的验证是开发队列内的十折交叉验证。作者尚未在手稿中增加说明。

**Original response:** “We respectfully note that there are many valid approaches to evaluation, and it would not be appropriate to presuppose that this is a limitation.”

**For the response letter:** “No. We used ten-fold cross-validation within the development cohort; an independent cohort was not evaluated.”

**For the manuscript, Methods:** “We evaluated the model using ten-fold cross-validation within the development cohort.”

**判定：** “No” 在回信中直接回答了真实问题；将同样的答复照搬到方法段则会让读者听见一场没有上下文的争论。若正文据此讨论对其他队列的推广，应在那项推断旁说明尚无外部表现数据。如果随后确实补写了方法，可以在回信中指向实际修改；现在不能写 “We have added …” 或编造页码。

<a id="e11"></a>
### E11｜基金或方案：明确计划，无须先为尚未取得的结果辩解

**已有材料：** 预试验的 8 名参与者均成功上传设备记录；预试验未评价疲劳或睡眠结局。正式研究拟同时收集活动节律和疲劳评分，检验两者的关联。

**原文：** “尽管我们尚不能断言活动节律对于疲劳的决定性作用，但可喜的预试验结果已经充分验证了这一思路，并为改善疲劳提供了强有力的依据。”

**改文：** “预试验的8名参与者均通过该流程成功上传了设备记录。正式研究将同步收集活动节律和疲劳评分，检验两者是否相关。”

**判定：** 成功上传支持数据采集流程的可行性；未测量疲劳就不能据此报告临床改善。使用“将检验”不是语气弱，而是准确标明研究阶段。未发生的结果既不用承诺，也无需提前道歉。

<a id="e12"></a>
### E12｜摘要、结果与图注：有些重复应移走，有些必须保留

**已有材料：** 一项单中心队列基线纳入 120 人，84 人完成随访，21 名完成者报告症状。图 2 的比例按有随访资料者计算。用户要求压缩摘要结果和图注；二者应可分别阅读。

**原摘要：** “需要指出这仅是单中心队列，结果须谨慎解释。120人中有84人完成随访，报告症状的比例为25%，但我们并不希望读者误解这一比例。”  
**原图注：** “如前所述本研究存在诸多局限。图2显示报告症状的比例。”

**改后摘要：** “该单中心队列纳入120人，84人完成随访；其中21人（25%）报告症状。”  
**改后图注：** “图2　随访时报告症状的比例：21/84（25%），分母为完成随访的参与者。”

**判定：** 将重复的“应谨慎”消去，在两个独立阅读位置各写清分母。“25% of the cohort” 容易被读成全体 120 人；未完成者的症状情况未知。单中心招募可在讨论外推时再作解释，图注无须重复。如果随访流失直接关系到某项判断，应在该判断旁说明其具体影响，而不是把全部限制集中到文末。

<a id="e13"></a>
### E13｜英文讨论整段：从事实、解释到真正未决的问题

**已有材料：** 比较报告持续耳鸣的成年人和未报告耳鸣的成年人。静息态分析显示，前者听觉皮层与前岛叶的功能连接较低，该组间差异经多重比较校正后仍达到显著。耳鸣组内，连接强度与自报困扰程度的相关未达到校正后的显著性标准。未进行听觉注意任务。

**Original paragraph:** “We wish to be clear that these preliminary observations must be interpreted with extreme caution. Nevertheless, the striking reduction in connectivity may point to an attentional deficit that drives tinnitus-related distress. The lack of a significant symptom correlation is understandable in such a difficult setting and does not detract from the potential clinical relevance of our work. Overall, these findings should be interpreted with caution.”

**Revised paragraph:** “Adults reporting persistent tinnitus showed lower resting-state connectivity between the auditory cortex and anterior insula than adults who did not report tinnitus. This group difference remained significant after correction for multiple comparisons. Within the tinnitus group, the association between connectivity and self-reported distress did not meet the corrected significance threshold. A study that also measures auditory attention could test whether individual differences in resting connectivity are associated with attention task performance.”

**逐步裁决：**

1. **保留组间观察。** 组别依据是参与者报告，测量是静息态功能连接，比较对象不是“健康而无任何疾病”的人。写明三者，再报告校正结果。
2. **把两种分析放回各自的位置。** 组间差异达到了校正标准，不足以推出组内困扰程度与连接有关；组内分析未达到校正标准，也不推翻组间观察。两种结果均保留。
3. **删去未经检验的借口。** 材料没有证明任务困难或样本原因导致未显著，也没有检验注意缺陷如何造成困扰。“may point to” 不能补上从静息信号到注意行为的缺失证据。
4. **让讨论仍然是讨论。** 若作者有兴趣研究听觉注意，把它写成下一步可以用任务表现检验的问题。若该段只服务于报告结果，则删除第四句，不必换成另一条通用局限。

<a id="e14"></a>
### E14｜文献计量与全稿核对：主题共现、实证关联和数字冲突分开处理

**已有材料：** 主题统计来自摘要。结果段写有 18 篇摘要同时提到睡眠时相和疲劳，结果表按同一口径写 19 篇；目前没有原始记录可判定哪个正确。单独核对过的另一项结果是：可从 7 篇摘要确认原研究检验过两个变量的个体层面关联。未提取关联方向或效应量。

**原文：** “尽管我们无意声称因果关系，但18篇文献共同证明睡眠时相可能参与疲劳的发生。为谨慎起见，需要更多研究进一步确认这一重要机制。”

**可直接使用的已核实内容：** “依据摘要，可确认7篇研究检验了睡眠时相与疲劳之间的个体层面关联。在同一摘要中提到这两个主题，并不能说明它们在参与者中呈何种关联。”

**另列给作者的注释：** “请核对结果段与结果表中同时提到两个主题的摘要数，分别为18和19。请据原始记录确认后，在对应位置补回一致的数量；此处的7篇是明确检验个体关联的研究数，不是对18或19的更正。”

**判定：** 讨论涉及的是研究者如何组织问题，不能据主题共现提出已得到证实的生物机制。“检验过关联”也不等于“发现了关联”。修订不能悄悄选一个冲突数字，更不能为了稿件看起来完整，把“约二十篇”当作定稿。这里暂时只交付可信的文字，并保留一眼可见的待核项；冲突解决前不能宣称整项结果已经定稿。
