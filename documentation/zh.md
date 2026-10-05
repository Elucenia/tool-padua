<!-- ELUCENIA technical documentation · padua · zh · no clinical/professional/rights approval -->

# Padua 评分

[条件、来源与许可](https://elucenia.org/zh/tools/padua)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 活动性癌症（转移或过去 6 个月内化疗/放疗）

`cancer`

### 既往静脉血栓栓塞（不含浅静脉血栓）

`tev`

### 活动受限（卧床，允许如厕，≥ 3 天）

`mobilidade`

### 已知易栓症

`trombofilia`

### 过去一个月有创伤或手术

`trauma`

### 年龄 ≥ 70 岁

`idade`

### 心力衰竭和/或呼吸衰竭

`icc`

### 急性心肌梗死或缺血性卒中

`iam`

### 急性感染和/或风湿病

`infeccao`

### 肥胖（BMI ≥ 30 kg/m²）

`obesidade`

### 正在接受激素治疗

`hormonio`

## 方法版本

Padua Prediction Score/Barbar 2010：11项因素，0–20；住院内科患者

## 已记录的公式

3分：活动性癌症、既往静脉血栓栓塞、活动减少、易栓症 · 2分：近期创伤或手术 · 1分：年龄≥70、心力/呼吸衰竭、心肌梗死或缺血性卒中、急性感染或风湿病、肥胖、激素治疗。最高：20。

## 限制与适用人群

Padua评分在内科住院患者中研究，随访症状性血栓栓塞事件至90天。血栓风险分层应同时评估出血、禁忌证和预防方案。总分不能代替该分析，也不意味着可自动应用于外科患者。

## 参考文献

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
