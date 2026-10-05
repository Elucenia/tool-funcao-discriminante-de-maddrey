<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · zh · no clinical/professional/rights approval -->

# Maddrey 判别函数

[条件、来源与许可](https://elucenia.org/zh/tools/funcao-discriminante-de-maddrey)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 患者凝血酶原时间

`tp`

s · 范围: 5–150

### 对照凝血酶原时间

`tpc`

s · 范围: 5–30

### 总胆红素

`bili`

mg/dL · 范围: 0.1–80

## 方法版本

修正Maddrey/Carithers 1989：4.6×(患者PT−对照PT)+胆红素；不含1978原始绝对PT方程

## 已记录的公式

判别函数 = 4.6 ×（患者凝血酶原时间 − 对照时间，秒）+ 总胆红素（mg/dL）。

## 限制与适用人群

1978年的原始函数在酒精性肝炎中研究。本地修订形式使用凝血酶原时间差及32阈值，应与1989年的后续版本对应。在作出任何治疗决定之前，总分不能代替对禁忌证、感染和其他可能诊断的评估。

## 参考文献

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

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
