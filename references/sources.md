# 来源记录

以下两个项目分别用于核对预先辩解的识别方法，以及证据强度、作者语气与学术惯例的处理。技能主体和中英文编辑判例按用户的通用论文规范重新编写；无需安装上游项目。

- [Worigin0314 / Academic Defensive Writing Auditor](https://github.com/Worigin0314/academic-defensive-writing-auditor/blob/89f26b8a7f8149e6458f657010d354587d42cfe9/SKILL.md)：区分实质性限定与预防性辩解，检查段落之间重复的非主张，按实验事实描述比较条件。
- [AIScientists-Dev / Academic Humanizer](https://github.com/AIScientists-Dev/academic-humanizer/blob/94b88b23703bed7df507acae7d6d5876209a0cdf/SKILL.md)：检查主张动词与证据的关系，保留学术术语、引文和作者语气，按文体区分已完成研究与拟议研究。
- 用户已认可并校订的《论文写作与修改标准》：应用其证据边界、讨论深度和章节适配等偏好。新批注与更新要求优先。两份上游文档中的打分、固定段数、禁用标点和限定数量上限均未设为本技能的执行要求。

## 判断依据：写作偏好与研究报告的区别

文中关于段落收尾、作者语气和标点的建议属于编辑选择。涉及统计解释和报告完整性时，需要独立依据。可按具体问题查阅：

- [Gelman 与 Stern：两个检验显著与否不同，不等于二者的差异已得到检验](https://sites.stat.columbia.edu/gelman/research/published/signif4.pdf)。与[规则 R07](rulebook.md#r07)、[判例 E05](decisions.md#e05)有关。
- [PRISMA 2020 扩展清单](https://www.prisma-statement.org/s/PRISMA_2020_expanded_checklist-yc78.pdf)，第16a和16b项说明系统综述应交代研究筛选结果和相关排除情况。这是为何某些过程信息必须保留的实例，并不要求所有论文采用系统综述格式。

判例和整段演示均为原创、虚构的教学材料。上列来源支持相应的判断原则，不是示例数据或研究故事的出处。

## Worigin0314 / Academic Defensive Writing Auditor

[上游许可原文](https://github.com/Worigin0314/academic-defensive-writing-auditor/blob/89f26b8a7f8149e6458f657010d354587d42cfe9/LICENSE)

```text
MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## AIScientists-Dev / Academic Humanizer

[上游许可原文](https://github.com/AIScientists-Dev/academic-humanizer/blob/94b88b23703bed7df507acae7d6d5876209a0cdf/LICENSE)

```text
MIT License

Copyright (c) 2026 AIScientists-Dev

This work builds on "humanizer" by blader (https://github.com/blader/humanizer, MIT) and adopts
standards from "ARMS" (https://github.com/koaeraser/ARMS); see the Acknowledgments in README.md.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
associated documentation files (the "Software"), to deal in the Software without restriction,
including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial
portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED.
```
