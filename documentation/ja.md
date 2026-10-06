<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · ja · no clinical/professional/rights approval -->

# Maddrey判別関数

[条件・出典・許諾](https://elucenia.org/ja/tools/funcao-discriminante-de-maddrey)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 患者のプロトロンビン時間

`tp`

s · 範囲: 5–150

### 対照プロトロンビン時間

`tpc`

s · 範囲: 5–30

### 総ビリルビン

`bili`

mg/dL · 範囲: 0.1–80

## 方法の版

修正Maddrey/Carithers 1989：4.6×(患者PT−対照PT)+ビリルビン；1978の絶対PT原式を含まない

## 記載された計算式

判別関数 = 4.6 ×（患者PT − 対照PT，秒）+ 総ビリルビン（mg/dL）。

## 限界・対象集団

1978年の原関数はアルコール性肝炎で研究されました。プロトロンビン時間の差と閾値32を用いるローカルの修正版は、後の1989年版に対応する必要があります。合計点は、治療判断の前に行う禁忌、感染、他の診断の評価に代わるものではありません。

## 参考文献

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

FD < 32: この基準では重症ではないアルコール性肝炎


### 2

FD ≥ 32: 重症アルコール性肝炎、コルチコステロイドを考慮


### 3

FD ≥ 32: 重症アルコール性肝炎、コルチコステロイドを考慮

