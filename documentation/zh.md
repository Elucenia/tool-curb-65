<!-- ELUCENIA technical documentation · curb-65 · zh · no clinical/professional/rights approval -->

# CURB-65

[条件、来源与许可](https://elucenia.org/zh/tools/curb-65)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### C — 意识混乱（新出现的时间、地点或人物定向障碍）

`c`

### U — 尿素 \> 42 mg/dL（\> 7 mmol/L）

`u`

### R — 呼吸频率 ≥ 30 次/分钟

`r`

### 收缩压 \< 90 mmHg 或舒张压 ≤ 60 mmHg（B — 血压）

`b`

### 年龄 ≥ 65 岁

`i`

## 方法版本

CURB-65/Lim 2003：意识模糊、尿素\>7 mmol/L、呼吸频率≥30、血压、年龄≥65；0–5

## 已记录的公式

每项1分： C（意识模糊）, U（尿素） \> 7 mmol/L, R（呼吸频率） ≥ 30/min, B（低血压：收缩压\<90或舒张压≤60 mmHg）及年龄≥ 65. 最高5。

该CRB-65 为同一评分但不含尿素（0–4），可无实验室检测使用。

## 限制与适用人群

2003年的CURB-65在因社区获得性肺炎住院的成人中推导和验证，使用初始评估数据和30天死亡率。年龄≥ 65是评分组成项，并非最低适用年龄。原始阈值为尿素\> 7mmol/L、呼吸频率≥ 30/min，以及收缩压\< 90或舒张压≤ 60 mmHg。排除条件及其他人群中的应用须阅读完整方案。

## 参考文献

- [Lim WS et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax, 2003.](https://doi.org/10.1136/thorax.58.5.377)

- [Lim WS et al. BTS guidelines for the management of community acquired pneumonia in adults: update 2009. Thorax, 2009.](https://doi.org/10.1136/thx.2009.121434)

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

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

低风险：30天死亡率为1.5%

| 结果详情 | |
| --- | --- |
| CRB-65（不含尿素） | 0（低风险（死亡率 < 1%）） |
| 建议处理 | 如无其他住院原因，可考虑门诊治疗。 |


### 2

中等风险：30天死亡率为9.2%

| 结果详情 | |
| --- | --- |
| CRB-65（不含尿素） | 2（风险增加（1到10%）：考虑转诊至医院） |
| 建议处理 | 考虑住院（或短期监督观察）。 |


### 3

高风险：30天死亡率为22%

| 结果详情 | |
| --- | --- |
| CRB-65（不含尿素） | 3（高风险（> 10%）：紧急住院） |
| 建议处理 | 住院；4或5分时，评估是否需要ICU。 |


### 4

低风险：30天死亡率为1.5%

| 结果详情 | |
| --- | --- |
| CRB-65（不含尿素） | 0（低风险（死亡率 < 1%）） |
| 建议处理 | 如无其他住院原因，可考虑门诊治疗。 |

