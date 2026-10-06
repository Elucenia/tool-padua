<!-- ELUCENIA technical documentation · padua · ja · no clinical/professional/rights approval -->

# Paduaスコア

[条件・出典・許諾](https://elucenia.org/ja/tools/padua)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 活動性がん（転移、または過去6か月以内の化学療法・放射線療法）

`cancer`

### 静脈血栓塞栓症の既往（表在静脈血栓症を除く）

`tev`

### 活動性低下（トイレ移動のみ可能な床上安静が ≥ 3日）

`mobilidade`

### 既知の血栓性素因

`trombofilia`

### 過去1か月の外傷または手術

`trauma`

### 年齢 ≥ 70 歳

`idade`

### 心不全および／または呼吸不全

`icc`

### 急性心筋梗塞または虚血性脳卒中

`iam`

### 急性感染症および／またはリウマチ性疾患

`infeccao`

### 肥満（BMI ≥ 30 kg/m²）

`obesidade`

### 現在ホルモン治療中

`hormonio`

## 方法の版

Padua Prediction Score/Barbar 2010：11因子，0–20；入院内科患者

## 記載された計算式

3点：活動性がん，VTE既往，移動制限，血栓性素因 · 2点：最近の外傷または手術 · 1点：年齢≥70，心不全/呼吸不全，心筋梗塞または虚血性脳卒中，急性感染症またはリウマチ性疾患，肥満，ホルモン療法。最大：20。

## 限界・対象集団

Paduaスコアは内科の入院患者で研究され、症候性血栓塞栓症を90日まで追跡しました。血栓のリスク層別化には、出血、禁忌、予防プロトコルの評価を伴わせる必要があります。合計点はその検討に代わるものではなく、外科患者に自動的に適用されることも意味しません。

## 参考文献

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

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

低リスク：予防なしでTEV 0.3%

薬物予防は適応されない。歩行を促す。


### 2

高リスク：予防なしでTEV 11%

高い出血リスクがなければ、薬物による血栓予防（LMWH、未分画ヘパリンまたはフォンダパリヌクス）を行う。


### 3

高リスク：予防なしでTEV 11%

高い出血リスクがなければ、薬物による血栓予防（LMWH、未分画ヘパリンまたはフォンダパリヌクス）を行う。

