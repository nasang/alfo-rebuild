---
layout: post
title: 美国税收优惠投资账户总结
date: 2024-12-24 11:26:00
description: 
categories: 掷金钱
languages: ["zh"]
thumbnail: assets/img/finance/tax-advantaged-accounts/tax-advantaged-accounts.jpg
pretty_table: true
toc:
  sidebar: left
---

> **DISCLAIMER（声明）**
> I am not a financial expert and the infomation I provide is for infomational purposes only. It should not be taken as investment or tax advice.
> 本人非金融专家，此处所包含的信息仅供参考，而非投资或税收建议。
{: .block-warning }

## 401(k)

> `401(k)` 一词源自于 IRC (Internal Revenue Code) [Section 401 Qualified pension, profit-sharing, and stock bonus plans](https://uscode.house.gov/view.xhtml?hl=false&edition=prelim&req=granuleid%3AUSC-prelim-title26-section401&num=0&saved=%7CZ3JhbnVsZWlkOlVTQy1wcmVsaW0tdGl0bGUyNi1zZWN0aW9uNDAx%7C%7C%7C0%7Cfalse%7Cprelim) 中的条款 [(k) Cash or deferred arrangements](https://bradfordtaxinstitute.com/Endnotes/IRC_Section_401k.pdf).

401(k)以创建它的税法部分命名，是一项雇主资助的退休储蓄计划，具有特殊的税收优惠。具体的税收优惠取决于所缴纳的401(k)类型。

### 子账户类型
#### Pre-tax
- **存**：当年存入的钱可以从“可税收入”（taxable income）中减去
- **取**：本金和收益都将计入该年普通类型 taxable income
- **罚**：不<u>符合条件</u>*的取钱操作将有额外10%的“早取”（early distribution）税


#### Roth
- **存**：无税收优惠
- **取**：本金无税；<u>符合条件</u>*取出的收益无税，否则计入该年普通类型 taxable income
- **罚**：不<u>符合条件</u>*的取钱操作将把本金和收益按照等比例取出，其中本金无税，收益有额外10%的 early distribution 税

#### After-tax
- **存**：无税收优惠
- **取**：本金无税；收益计入该年普通类型 taxable income
- **罚**：不<u>符合条件</u>*的取钱操作将把本金和收益按照等比例取出，其中本金无税，收益有额外10%的 early distribution 税

*符合条件的解释：取钱时持有人满足59.5岁，如果是 Roth 账户还需满足账户已持有至少5年。[这些情况](https://www.irs.gov/retirement-plans/plan-participant-employee/retirement-topics-exceptions-to-tax-on-early-distributions)可以免除额外 10% early distribution 税。

综上所述：

|| Pre-tax | Roth | After-tax |
|:-----------| :----------- | :------------- | :------------ |
|本金| 延迟交税   |    当下交税    |       当下交税 |
|收益| 延迟交税   |    符合条件免税    |       延迟交税 |
|罚金| 10%*(本金+收益)    |    10%*收益    |       10%*收益 |

<p></p>

如此看来，After-tax 在本金上不如 Pre-tax，在收益上不如 Roth，为什么还会存在呢？这就要说到 401(k) 的缴纳上限。

### 缴纳上限
401(k)计划是跟着雇主走的，一对雇佣关系对应一个401(k)计划；而存放至401(k)计划的钱既可以来自员工的 paycheck，也可以来自雇主的 match。
- **Elective Deferral**: 401(k)最开始是一个延税计划，elective deferral（选择性延期）指的是员工自愿缴纳的延税款。IRC Sec. 402(g) 规定了 elective deferral 的限额，即 402(g) limit。Pre-tax 和 Roth 共享此限额。
- **Annual Addition**：整个401(k)的存入金额称为 annual addition（年度增量），首先不能超过这份工作的总收入，其次 IRC Sec. 415(c) 规定了 annual addition 的限额，即 415(c) limit。
- **Catch Up**：50岁以上的员工可以额外存的钱，不受制于上面两种限额。

因此，402(g) limit 规定了一位员工`本人`每年可以存的 Pre-tax + Roth 额度，而 415(c) limit 规定了`每个401(k)计划`每年可以存的额度。

|Year| Elective Deferral | Annual Addition | Catch Up |
|-----------| :----------- | :------------- | :------------ |
|2025| $23,500   |    $70,000    |       $1,000  |
|2024| $23,000   |    $69,000    |       $1,000  |

<p></p>

因此，After-tax 的优势在于可以突破 Elective Deferral 的限制，使得一部分（未来）收益达到延税的目的。不过，其好处远不止于此，那就是 Mega backdoor Roth（Roth大后门）。

### Mega backdoor Roth
> 并非所有 401(k) 计划都提供 Mega backdoor Roth，并且这个方法随时有可能被废止。
{: .block-warning }

简单来说，Mega backdoor Roth 就是先存 After-tax，然后将其转化为 Roth 的策略。
- **In-plan Roth conversion**：即将 After-tax 401(k) 转为 Roth 401(k)。
- **Roll over to Roth IRA**：即将 After-tax 401(k) 转入 Roth IRA。

若 After-tax 401(k) 中存在收益，则收益部分在转化当年需要交税。

### 取钱要求
- Elective Deferral 的部分在 Sec. 401(k)(2)(B)(i)统一限制了取出条件（没达到条件，即使愿意付罚金也无法取出）：
  - 员工离职/去世/残疾，或
  - 员工年龄达到59.5岁，或
  - 其他一些困难条件等
- 59.5岁是最常见的qualified distribution条件，不达该年龄从401(k)中取钱，计算收入税的部分会有10%的罚金。
- RMD（Required Minimal Distribution）：在持有人年龄超过72岁时，须按照 IRS 提供的预期寿命表格计算每年最低取出的比例，少取部分有50%的罚金。

### 推荐阅读
#### Fidelity
- [What's a 401(k)?](https://www.fidelity.com/learning-center/smart-money/what-is-a-401k)
- [Traditional or Roth account? 2 tips to help you choose ](https://www.fidelity.com/viewpoints/retirement/spender-or-saver)
- [What to do with after-tax 401(k) contributions](https://www.fidelity.com/viewpoints/retirement/401k-contributions)
- [What is a "mega backdoor Roth"?](https://www.fidelity.com/learning-center/personal-finance/mega-backdoor-roth)

## IRA
IRA 全称 Individual Retirement Account（个人退休账户），是与 401(k) 类似的税收优惠投资账户，无需雇主提供。其类型主要分为 Traditional 和 Roth，对比如下：

|| Traditional| Roth |
|-----------| :----------- | :------------- |
|谁可以存？| 本人或配偶（在联合报税的前提下）有可税收入。| 本人或配偶（在联合报税的前提下）有可税收入，且 MAGI（Modified Adjusted Gross Income）低于指定要求。|
|存入本金否减税？| [满足要求](https://www.irs.gov/retirement-plans/ira-deduction-limits)可减   |    否    |
|取钱顺序|本金和收益按比例取出|先取本金，再取收益|
|取钱如何交税？|任何存入时免税的本金和收益都要交税。|本金随时无税取走，收益在[满足条件](https://www.irs.gov/publications/p590b#en_US_2023_publink100089543)的情况下无税。|
|早取税|若不满足59.5岁，需付额外10%早取税（除非满足[这些情况](https://www.irs.gov/retirement-plans/plan-participant-employee/retirement-topics-exceptions-to-tax-on-early-distributions)）|同左|
|RMD|同401(k)|无|

<p></p>

### 缴纳上限

2024年和2025年均为 $7,000。

### Backdoor Roth
因为 Roth IRA 有收入限制，所以收入超出范围的人无法直接存 Roth IRA，但可以通过先存 Traditional IRA 再将其转入 Roth IRA，即 Backdoor Roth（Roth后门）。

### Roth IRA vs Roth 401(k)
Roth IRA 具有本金随时可取，且取出顺序为先本金后收益的优势，因此将 Roth 401(k) 转入 Roth IRA 不失为一种选择。这个操作是免税的。

## HSA
HSA 全程 Health Savings Account（健康储蓄账户），存入时可减税，中间的资本利得不用交税，取出时也免税（用于报销医疗支出的前提下）。报销医疗支出没有任何时间限制。若到 65 岁时还没有足够的医疗帐单需要报销，依然可以从中取钱，不过需按当年收入交税。

存 HSA 的条件是保险为 HDHP（High Deductible Health Plan，高自负额保险）。

|Year| 个人 | 家庭 |
|-----------| :----------- | :------------- |
|2025| $4,300  |    $8,550    | 
|2024| $4,150   |    $8,300    | 

<p></p>