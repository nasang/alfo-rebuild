---
layout: post
title: 简易税务计算器
date: 2024-12-31 23:25:00
description: 
categories: 掷金钱
tags: 税务
languages: ["zh"]
thumbnail: assets/img/finance/income-tax/cover.jpg
---

最近在写其他博文的时候，经常需要手动计算预估税率，低效且重复。于是想着写一个简易版的收入税计算器：

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/TaxCalculator.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/TaxCalculator.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
{% jupyter_notebook jupyter_path %}
{% else %}
<p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}