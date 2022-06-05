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
  A([Start])-->B{お金を入れたか}
  B--Yes-->C[金額を表示]
  C-->D1
  D1-->E{購入ボタンが押されたか}
  E{購入ボタンが押されたか}--Yes-->F{指定以上の金額が入っているか}
  F--Yes-->G[飲み物を出す]
  G-->H([End])
  B--No-->A
  E--No-->B
  F--No-->B
    subgraph 返却ボタンの処理
    D1{返却ボタンは押されたか}--Yes-->D2[お金を返却する]
    D2-->D3[金額をリセットする]
    end

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
