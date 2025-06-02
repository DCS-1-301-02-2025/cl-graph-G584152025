# 課題

## 課題 3.1 有向グラフ

![ex01.png](ex01.png)

プレビュー結果が上の図のようになるように，下記の記述を完成させよ．(接続関係が正しければ，上下が入れ替わっても構わない)

※ 日本語の文字列に対する箱の大きさが適切でない場合には，前後に空白を入れて調整せよ

```graphviz
digraph {
    rankdir = "LR";
    node [shape=box];

    "     コンピュータリテラシー    " -> "   プログラミングI  " -> "   プログラミングII  ";
     "     コンピュータリテラシー    " -> "　プログラミング基礎I　" -> "　プログラミング基礎II ";
     "　基礎ゼミ　" -> "　プログラミング基礎I　" ;
     "　情報工学概論　" -> "　計算機工学　" -> "　論理回路　";
     "　情報工学概論　" -> "　プログラミング基礎I　"
}
```

## 課題 3.2 WBS

![ex02.png](ex02.png)

プレビュー結果が上の図のようになるように，下記の記述を完成させよ．(色や影などの違いは気にしなくてよい)

```plantUML
@startwbs ex02
* 拓殖大学
** 商学部
*** 経営学科
*** 国際ビジネス学科
*** 会計学科
** 政経学部
*** 法律政治学科
*** 経済学科
*** 社会安全学科
** 外国語学部
*** 英米語学科
*** 中国語学科
*** スペイン語学科
*** 国際日本語学科
** 工学部
*** 機械システム学科
*** 電子システム学科
*** 情報工学科
*** デザイン学科
** 国際学部
*** 国際学科
@endwbs
```

## 課題 3.3 ユースケース図

![ex03.png](ex03.png)

プレビュー結果が上の図のようになるように，下記の記述を完成させよ．ただし，別名については適当に設定してよい．(色や影などの違いは気にしなくてよい)

```plantUML
@startuml ex03
left to right direction
actor 学生 as student
actor 教員 as teacher
rectangle {
    usecase "提出の採点" as grade
    usecase "レモートリポジトリにpush" as push
    usecase "修正のコミット" as commit
    usecase "修正をステージに上げる" as up
    usecase "課題ファイルの修正" as do
    usecase "リポジトリのクローン" as clone
    usecase "課題の受領" as recieve
    usecase "課題の登録" as register
}
register <-- teacher
student --> recieve
student --> clone
student --> do
student --> up
student --> commit
student --> push
grade <-- teacher
@enduml
```

## 課題 3.4 オリジナルの図解

「有向グラフ」「WBS」「ユースケース図」のどれかを使って，
独自の図解を作成せよ．対象は自由に決めてよいが，
誰かのコピーにならないように留意せよ．

```plantUML
@startwbs 
* 今日のスケジュール
** 朝
*** 工学日本語I
*** トレーニング演習
** 昼
*** 昼ご飯
*** コンピュータリテラシー
*** 課題をやる
** 夜
*** バレーボール
*** 帰宅
@endwbs
```




## チェック
- [ ] 課題 3.1 有向グラフ
- [ ] 課題 3.2 WBS
- [ ] 課題 3.3 ユースケース図
- [ ] 課題 3.4 オリジナルの図解
