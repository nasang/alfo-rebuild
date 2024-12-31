---
layout: post
title: 美国 FICA 税详解
date: 2024-12-29 15:36:00
description: 
tags: 税务
categories: 掷金钱
languages: ["zh"]
thumbnail: assets/img/finance/fica/fica.webp
pretty_table: true
toc:
  sidebar: left
---

## 什么是 FICA 税？

FICA 全称为 Federal Insurance Contributions Act（联邦保险供款法案），是美国联邦工资税的重要组成部分。其内容有两部分，即“社保”（社会保障）和“医保”（医疗保险）：
1. Social Security taxes，更常见的名字为 OASDI (Old-Age, Survivors, and Disability Insurance) tax
2. Medicare taxes

法律要求雇主从雇员工资中扣留一定比例，以资助“社保”和“医保”。
- 注：若税务身份为 NRA，则免除 FICA 税。

## 税率
### Social Security
公司和员工各缴纳 6.2%。但是，应缴税的工资收入是有上限的。
- 2025年：$176,100，即最多缴纳 $10,918.2
- 2024年：$168,600，即最多缴纳 $10,453.2

### Medicare
公司和员工各缴纳 1.45%。但是，超过一定金额的工资还将继续缴纳额外的税，即 additional medicare tax，税率为 0.9%，基准如下：
- $250,000 for married filing jointly;
- $125,000 for married filing separately; and
- $200,000 for all other taxpayers.

假设共同报税，且总年收入为 x（x > 25万），则**员工**缴纳医保的金额为 
- $250,000 * 1.45% + (x - $250,000) * (1.45% + 0.9%) = x * 2.35% - $2,250

即等效税率 y = 2.35% - 2,250 / x。例如，当 x 为 $300,000，等效税率是 1.6%。

### 总结
<table id="table" data-toggle="table">
  <thead>
    <tr>
      <th data-field="id"></th>
      <th data-field="employee">员工支付</th>
      <th data-field="employer">雇主支付</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>社会保障税（又称 OASDI）</td>
        <td>
            6.2% <br><br>
            <i>仅限 2024 年的前 168,600 美元和 2025 年的前 176,100 美元。</i>
        </td>
        <td>
            6.2% <br><br>
            <i>仅限 2024 年的前 168,600 美元和 2025 年的前 176,100 美元。</i>
        </td>
    </tr>
    <tr>
        <td>医疗保险税</td>
          <td>1.45%</td>
          <td>1.45%</td>
    </tr>
    <tr>
        <td>全部</td>
          <td>7.65%</td>
          <td>7.65%</td>
    </tr>
    <tr>
        <td>额外的医疗保险税</td>
        <td>
            0.9％ <br><br>
            <i>仅限单身申报者收入超过 200,000 美元的部分；联合申报者收入超过 250,000 美元的部分；已婚单独申报者收入超过 125,000 美元的部分。</i>
        </td>
        <td></td>
    </tr>
    </tbody>
</table>

<p></p>

### 旁注
1. 税收优惠账户中，员工自己存入 pre-tax 401(k) 的本金不能免去 FICA（[IRS 说明](https://www.irs.gov/retirement-plans/retirement-plan-faqs-regarding-contributions-are-retirement-plan-contributions-subject-to-withholding-for-fica-medicare-or-federal-income-tax)）；通过 paycheck 存入 HSA 的本金可以免 FICA，但自己直接存的不能。

## 福利
需要 40 分才能享受福利，每年最多积攒 4 分，规则如下：
- 每 $1,730 工资 = 1 分
- 达到 $6,920 工资即拿满该年的 4 分

可以在 [my Social Security](https://www.ssa.gov/myaccount/) 注册账号查看自己的积分。

## 参考
- [SSA： 什么是 FICA？](https://www.ssa.gov/marketing/assets/materials/CH-S-05-10297.pdf)
- [NerdWallet: FICA Tax: Definition and How It Works in 2024-2025](https://www.nerdwallet.com/article/taxes/fica-tax-withholding)
- [IRS: Topic no. 751, Social Security and Medicare withholding rates](https://www.irs.gov/taxtopics/tc751)
- [IRS: Topic no. 560, Additional Medicare tax](https://www.irs.gov/taxtopics/tc560)