---
title: stackdriver
date: 2018-10-07T08:49:34.805Z
description: test
---
## 初めて、この名前聞いた時
![smile.jpg](https://image.docbase.io/uploads/36c876be-1eeb-45ec-bb78-0f27b4414651.jpg =WxH)
<span style="font-size: 200%">技のイメージ</span>

実際はそんな暴力的なものではないです。
## GCPのモニタリングツール
https://cloud.google.com/stackdriver/

グーグルがゼロから作ったとまでいうその力作、見せてもらおうか。(´ｰ`)y-~~

## プロジェクト作成
アカウント上に「Traial」プロジェクトを作成し、そこで有効化する。
![スクリーンショット 2018-10-06 19.04.37.png](https://image.docbase.io/uploads/8bcf2a1c-a0e1-41e5-ac95-fa31bd7c4c0e.png =500x)

## 監視するプロジェクトを選択
Traial一つを選択。
StackDriverというプロジェクトがあるけど無視。（その名前でプロジェクト作ったけど、プロジェクト名か機能名か区別しにくいのでやめた）
![image.png](https://image.docbase.io/uploads/48d2120d-b36c-4c55-99b4-aa698d0a05dc.png =500x)

## オプションでAWSアカウントを監視するか。
最初から表示するなんて完全に意識して作ってますね。
そういうツンデレ嫌いじゃないです。（*´ω｀*）使いやすいし。
![image.png](https://image.docbase.io/uploads/caa23281-bc62-4704-aa93-9bbe426d2dd3.png =500x)
![image.png](https://image.docbase.io/uploads/ab5d1d29-d9db-4458-9234-563cebbbe1fb.png =500x)

※尚、EXternalIDは本来「sd6517434」みたいな形でsdだけなのはなんらかの表示バグで登録できない。
　参考サイトもここは伏せるところなので、この形式ってわかりにくかったorz

AWS側はdev垢を利用する。
## dev側でロールの作成
![スクリーンショット 2018-10-06 19.29.35.png](https://image.docbase.io/uploads/c20024e5-9a85-495a-a9b2-91e610ee81ff.png =500x)

権限は「ReadOnlyAccess」

![image.png](https://image.docbase.io/uploads/39513c17-71f4-4b88-8e1b-f35547a0b591.png =500x)

![image.png](https://image.docbase.io/uploads/4390252d-ea80-4786-b0b9-1aa43f982111.png =500x)

※そのあとレポートを日次で出すかというページあったけど、スクショ撮り忘れた。

## 設定完了後
リソースにdevで使用している環境の情報が列挙されている。
![image.png](https://image.docbase.io/uploads/0a55f2df-064e-4753-9da6-a4a995820628.png =500x)

## Dynamoの一例
取れてる取れてる。
![image.png](https://image.docbase.io/uploads/2e0575a3-d631-447a-abc2-03eb27a75bf6.png =500x)

次は、グラフの作成とアラート通知あたりを設定してみたい。


今回は以上。
