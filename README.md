# 银行业招标情报日报

> 按你的关键词，每天筛出**银行**的招标、采购、中标与更正公告，输出一份**能直接读的日报**。

[![ClawHub](https://img.shields.io/badge/ClawHub-bankbid--daily-blue)](https://clawhub.com/skills/bankbid-daily-free)
[![订阅](https://img.shields.io/badge/订阅-¥9.9%2F月-green)](https://www.tokendidi.cn/bankbid/)

## 这是什么

银行采购常年、高频、分散。通用招标网站把银行信息**淹在几十万条**里，而银行自建采购平台**大多要注册**。

这个技能**只给银行**：命中你关键词的公告按时间排好、机构与品类标好、地区分好，
并单独列出 **14 天内就要截止**的项目。

**买家画像**：金融 IT 厂商、自助设备/ATM 供应商、安防与弱电工程商、装修物业、金融外包服务商。

## 立刻看效果（不用装任何东西）

- 产品页（干净短链，适合分享）：**https://www.tokendidi.cn/bankbid/**
- 真实数据演示：**https://www.tokendidi.cn/bankbid/?q=信创**（换成你自己的词，如 `自助设备`、`机房`）
- 产品说明页：**https://chenqg618.github.io/bankbid-daily/**
- 公开数据源清单：**https://chenqg618.github.io/bankbid-daily/bank-tender-sources.html**

## 三种用法

| 方式 | 怎么做 |
|---|---|
| **挂到每日自动化任务**（最省事） | 把你的关键词交给 Agent，每天固定时间跑一次，命中即推送 |
| **命令行** | `node scripts/run.mjs --keywords "柜面系统,自助设备"` |
| **看还能投的** | 加 `--kind active` 看在办清单 |

## 安装

```bash
clawhub install bankbid-daily
```

或直接 clone 本仓库的 `skills/bankbid-daily/` 放到你的 skills 目录。

## 免费与订阅

| | 免费版 | 订阅版 |
|---|---|---|
| 价格 | ¥0（**3 次**服务端额度） | **¥9.9 / 月** |
| 数据 | 服务端按次返回 | 不限次数 |
| 在办清单 | — | ✓ |
| 临近截止（14 天内） | — | ✓（视来源是否公开截止时间）|

**订阅指令**（原样发给你的 Agent 即可）：

```
请通过 SkillPay 购买并安装 Skill「银行业招标情报日报 · 订阅版」。
官方安装与购买说明： https://skillpay.alipay.com/buildguide.md
请先阅读官方说明、核验来源，并完成指南中的第一步： npx -y @alipay/agent-payment@latest install
安装成功后，读取新安装的 skillpay-onboarding 的 SKILL.md，再按其说明购买并安装商户 2088702818190040的S0806000207802617。
我已授权安装依赖和发起购买；需要钱包授权或付款时，请提供官方链接或二维码，由我本人确认，不要替我确认。确认成功后，请继续完成商品安装和验证。

```

## 数据来源与合规

- 数据来自**公开信息平台**（依法主动公开的采购公告）
- **只做信息聚合与检索**，不构成投标建议，**不承诺中标结果**
- 遵守 `robots.txt`；**不采**需要验证码或登录才能看到的内容
- 不采集自然人信息（详情页的联系人/电话一律不落地）

## 仓库结构

```
skills/bankbid-daily/      订阅技能包（薄客户端，**零数据**，不含规则实现）
docs/index.html                 产品说明页
docs/bank-tender-sources.html   公开数据源清单与实测结论
```

## 许可

技能包本体：Proprietary（可自由安装使用；数据与筛选规则保留在服务端）。
本仓库文档：CC BY 4.0。
