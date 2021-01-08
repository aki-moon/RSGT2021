テストに関するQ&A～RSGT2021のOSTメモ～

本記事は、RSGT2021のOSTにてディスカッションした内容のまとめになります。



# 忍者式テストはどう定着していった？

http://www.jasst.jp/archives/jasst04/pdf/A7ah.pdf

# テストに対する意識や興味を会社で高めるために最初にすると良さそうなことは？

お客さんから報告があった(お客さんの業務に影響があった)不具合の分析からスタートすると良い。

# テストを端折りたくなった時、どうする？

テストをやりたくない時ほどやった方がいい。
テストをしたくない場所はテスタビリティが低い可能性が高い。

https://blogs.itmedia.co.jp/hiranabe/2005/08/post_e66c.html

# 新卒一年目はテスト関連のことについてどう勉強していくと良い？

## 書籍

https://swquality.jp/?p=1180
に記載のある書籍がおすすめ。

## コミュニティ・イベント

- http://jasst.jp/

- https://wacate.jp/
- https://ost-zatu.connpass.com/
- https://autotest-lab.connpass.com/

# 探索的テストのチャーターってどんなものが使われるの？

Explore It！(https://www.amazon.co.jp/Explore-Increase-Confidence-Exploratory-Testing/dp/1937785025)
の例が参考になる。
チャーターは正解がないが、 テストの実行者がテスト実施（手順）をイメージできる粒度にしておくと良い。

# もし世界からテスト外注会社が消えたら？

完全に任せきりにしているところから、部分的に（上流から）抑えるようにしていくという手もある

# 外部会社のQAチームと距離を感じてる。距離の近いやりとりをうまくやっているチームがあるのだろうか？

やり方次第で距離を縮められるはず。
ブロッコリーさん(https://twitter.com/nihonbuson)
の会社も外部会社と協働している。

# 非エンジニアがテストスキルを習得するには？

https://note.com/mishizuka/n/n5bb083dc8716

# 受入テストの自動化をしたいが自動化のコストが高い。ノウハウはあるか？

受け入れテストの自動化（おそらくE2E自動テスト）で目指したい部分を絞った方が良い。ポイントはいくつかある。

1. 自動化をできる体制になるまでの初期コストがある程度存在することを理解する
概念としては、以下スライドを参考。
https://speakerdeck.com/yoshikiito/tesutozi-dong-hua-toosao-chu-robotuto

2. 本当にE2Eで確認したい部分なのか考える
E2Eよりも下の段階（APIレベルやUnitレベル）で確認できないのか考えた方が良い。
本当にE2Eで見たい部分を考えることについては下記の記事を参照。
https://nihonbuson.hatenadiary.jp/entry/2018/10/29/210000

3. 特に不具合が発生したらまずいところから自動化を検討する
どこから自動化を検討するかについては下記資料を参考。
http://www.jasst.jp/symposium/jasst16tokyo/pdf/D4.pdf

4. E2Eテストの自動化では、手動のテストとは別の気にする部分が複数存在することを理解する
テスト自動化研究会が書いた「テスト自動化の8原則」を参考にすると良い。
https://sites.google.com/site/testautomationresearch/test_automation_principle