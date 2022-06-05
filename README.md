# 課題
Mermaidを触ってみよう

マークダウンファイルを編集して、Mermaidで図を描いてみよう

# 取り組み方
* 本プロジェクトをforkしてください。
* README.mdを編集して、Mermaidを使いこなしてください
* できたらプルリクエストを出します

# 課題項目
## 流れ図
### 条件
- 開始と終了ノードをつける
- 条件分岐を組み込む
- 5ノード以上
- カッコいいほど高得点

## 解答
```mermaid
flowchart TB
  START-->A(購入者が現れる)
  A(購入者が現れる)-->B{お金を入れたか}
  B-->|YES|C(金額を表示)
  B-->|NO|START
  C-->[[返却ボタンの処理]]-->E{購入ボタンが押されたか}
  E{購入ボタンが押されたか}-->|YES|F{指定以上の金額が入っているか}
  E-->|NO|[[返却ボタンの処理]]
  F-->|YES|G(飲み物を出す)
  F-->|NO|[[返却ボタンの処理]]
  G-->END

```

## シーケンス図
### 条件
- 3人以上
- メッセージをやり取りしない人がいないように
- 自己呼び出しを含むこと
- カッコいいほど高得点

## 解答
```mermaid
```

## クラス図

### 条件
- 3つ以上
- 汎化と集約を含むこと
- カッコいいほど高得点

## 解答
