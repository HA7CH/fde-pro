<div align="center">

# fde-pro

**成为 FDE。**

上传简历,诚实诊断你是不是 FDE、缺哪半、走土路线还是大厂路线、未来 30 天该干什么。

[进入 HA7CH School](https://school.ha7ch.com) · [FDE 全息卡片（兼容保留）](https://fde.ha7ch.com/c/lawted) · [深大讲座](https://fde.ha7ch.com/course)

<sub>HA7CH PRO · Build in the field, hatch into impact.</sub>

</div>

---

> [!IMPORTANT]
> **fde-pro 已并入 [HA7CH School](https://school.ha7ch.com)。** FDE 诊断现在是 School 的 FDE 课程内置实验 Skill，不需要再单独安装。本仓库进入兼容维护期：现有全息卡片与讲座链接继续可用，新的课程与诊断规则以 `HA7CH/ha7ch-school` 为准。

## 新入口

安装或更新 HA7CH School：

```bash
npx -y @ha7ch/school@latest
```

加载后选择「FDE」，进入第 3 课即可运行内置诊断。仓库与课程更新请前往 [HA7CH/ha7ch-school](https://github.com/HA7CH/ha7ch-school)。

---

## 这是什么

一台 **FDE 适配诊断器**,不是职业鸡汤机,也不是"AI 帮你规划人生"。

背后是一个真正驻过场的 FDE 的一手判断力——给货代公司做过提单解析、跟过一线跟单员、踩过"卖整体系统卖不动"的坑。它看完你的简历 / 经历 / 访谈回答,**诚实判断你现在是不是 FDE,敢说"你现在不适合"**。

> **FDE = Echo + Delta,缺一半都不是。**
> - **Echo** — 进现场摸真需求,主动推翻老板的表面需求(按文档拆需求、销售式顺着签单,都不算 Echo)。
> - **Delta** — 本人零依赖端到端做出能跑的东西(用 Cursor / Claude Code 算合格 Delta)。

**满分尺子**:把一张真实提单 PDF 拖进去当场解析成字段,让一线脱口而出"这绝对能帮到我"。

---

## 旧版独立安装（仅兼容）

旧的 `fde-pro` Skill 仍可运行，但不再作为推荐入口。新用户请从 HA7CH School 开始；下面只为已有安装者保留：

```
# 1. 先装 RedSkill 商店(按官方指引)
#    redskill.xiaohongshu.net/install.md

# 2. 一行口令装上 fde-pro
redskill install fde-pro

# 3. 把简历 / 经历丢给它,直接说:
#    "帮我看看我适不适合做 FDE"
```

装好后它会带你走一条完整路径:

```
选路线  →  探索问答  →  七维打分  →  缺口处方  →  找在招岗  →  出卡片
土/大厂     不是一次性     够不够格      缺哪半补哪半    调 job-pro    FDE 全息卡
```

- **选路线**:土 FDE(对接中小企业 / FDOPC)还是大厂平台型 FDE(飞书 / 钉钉 / Google / OpenAI / Anthropic)。
- **七维打分**:薄切片 30 / Echo 20 / 经济账 15 / Conduct 15 / ToB 10 / 案例 10 / 现场入口 10,带硬地板和 11 条红旗,不只是给个分数。
- **找在招岗**:接 [job-pro](https://job.ha7ch.com),按你的画像捞国内在招的 FDE / 解决方案 / AI 落地工程师岗。
- **出卡片**:生成一张可分享的 FDE 全息卡片(见 [fde.ha7ch.com/c/lawted](https://fde.ha7ch.com/c/lawted))。

---

## 仓库结构

```
skill/                 ← skill 源码(可直接读)
  SKILL.md               诊断引擎:选路线 / 七维评分 / 象限处方 / 路线判定
  references/
    dachang-fde-interview.md   大厂线面试参考(双读者:海外实战手册 / 国内迁移能力模型)

src/app/
  page.tsx             落地页(fde.ha7ch.com)
  c/[handle]/          FDE 全息卡片
  course/              深大讲座 PPT(18 页全屏 slide deck)
```

skill 本体是纯文本 `SKILL.md`,不依赖任何运行时——RedSkill 装的就是它。网页部分是 Next.js,部署在 Vercel。

---

## 为什么不一样

满大街的"AI 职业规划"给的是鼓励;这个给的是**驻场踩坑攒出来的四条现场真相**:

1. **反平台是生死线**——做 AI 增量插件 / 数字员工,不做换系统 / 重做 ERP,"整体切换"卖不动。
2. **经济账自己算**——老板常算错,用「砍掉的人力工时 × 单位成本 × 10–20%」估价值。
3. **价值在一线高频用户**,不在拍板的主管。
4. **护城河是领域正确 + 端到端落地**,不是表面功能(把在线托书 / OCR 当杀手锏 = 扣分)。

三套子系统必须对齐:**分数**判够不够格,**象限**(Echo × Delta)判缺哪半、发什么处方,**路线**判走土还是大厂。

---

<div align="center">
<sub>

一个 [HA7CH](https://ha7ch.com) 出品 · the world's first FDE Accelerator

</sub>
</div>
