+++ 
draft = false
date = 2022-03-20T23:08:24+09:00
title = "プログラミング言語 Met のお知らせ"
description = "プログラミング言語 Met のお知らせ"
slug = ""
authors = []
tags = ["news"]
categories = ["news"]
externalLink = ""
series = []
+++

所長 Met 氏を雰囲気を持つプログラミング言語が欲しいという有志達の要望にお答えして、

Brainfuck系プログラミング言語 Met が公開されました。

※ ジョーク言語です。

## Brainfuckとは
> [Brainfuck - Wikipedia](https://ja.wikipedia.org/wiki/Brainfuck "Brainfuck - Wikipedia")

## GitHub 
[https://github.com/MetLaboratory/metlang](https://github.com/MetLaboratory/metlang "GitHub metlang")

## 説明
* 「にゃうね」 ポインタをインクリメントする
* 「にゃう」 ポインタが指す値をインクリメントする
* 「にゃん」 ポインタをデクリメントする
* 「にゃ？」 ポインタが指す値をデクリメントする
* 「ポチった」 ポインタが指す値が0なら、対応する 「ねる」 の直後にジャンプする
* 「ねる」 ポインタが指す値が0でないなら、対応する 「ポチった」 にジャンプする
* 「これになりたい」 ポインタが指す値を出力に書き出す
* 「これすき」 入力から1バイト読み込んで、ポインタが指す先に代入する

## 例

### hello.met
```
にゃうねにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうポチったにゃんにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうねにゃ？ねるにゃんこれになりたいにゃうねにゃうにゃうにゃうにゃうにゃうにゃうにゃうポチったにゃんにゃうにゃうにゃうにゃうにゃうねにゃ？ねるにゃんにゃうこれになりたいにゃうにゃうにゃうにゃうにゃうにゃうにゃうこれになりたいこれになりたいにゃうにゃうにゃうこれになりたいポチったにゃ？ねるにゃうねにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうポチったにゃんにゃうにゃうにゃうにゃうにゃうねにゃ？ねるにゃんこれになりたいにゃうねにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうポチったにゃんにゃうにゃうにゃうにゃうにゃうにゃうねにゃ？ねるにゃんこれになりたいにゃうねにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうポチったにゃんにゃうにゃうにゃうにゃうねにゃ？ねるにゃんこれになりたいにゃうにゃうにゃうこれになりたいにゃ？にゃ？にゃ？にゃ？にゃ？にゃ？これになりたいにゃ？にゃ？にゃ？にゃ？にゃ？にゃ？にゃ？にゃ？これになりたいポチったにゃ？ねるにゃうねにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうポチったにゃんにゃうにゃうにゃうにゃうにゃうねにゃ？ねるにゃんにゃうこれになりたいポチったにゃ？ねるにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうにゃうこれになりたい
```

### 実行
```
./met examples/hello.met
```

### 結果
```
Hello World!
```
