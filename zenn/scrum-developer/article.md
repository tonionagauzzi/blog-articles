# はじめに
先日、**認定スクラムデベロッパー**の研修コースに参加し、無事認定をいただきました！
![](https://storage.googleapis.com/zenn-user-upload/5b0dd74d1897-20231027.png)
https://bcert.me/sguviirle

この記事では、そのスクラムデベロッパーコースを受講した所感を述べます。

# コースを受けた経緯
10年近く**ウォーターフォール**モデルで請負型の開発をしてきてから、スクラムベースの開発チームに移り、約4年間さまざまなプロジェクトを渡り歩いてきて、最初は懐疑的だった**アジャイル**やスクラムの良い部分を徐々に体感してきました。
そこで、今後もよりよいスクラムを追究する足掛かりになればと思い、この度スクラムデベロッパーコースを受講しました。

最初は**認定スクラムマスター**コースの受講を考えていました。
しかし現在、大規模なプロダクトの1チームにいる身なので、スクラムマスターになると**チームを跨いでの会話が増えすぎる懸念**がありました。
また、**他者との会話よりも具体的な作業を手を動かして進める方が好き**で、その役割が今の私に合っているとも感じていました。
さらに、スクラムデベロッパーはスクラムマスターを開発者として補佐する立場だ、みたいな誤解も持っていました。

それらをふまえて、私はスクラムデベロッパーを選択しました。

# スクラムマスターと何が違うの？
ここが最もみなさんの気になるところだと思いますが、明確な線引きはありません。しかし、研修を受けての私の解釈は以下の通りです。

## スクラムマスター
- スクラムイベントが機能してることに責任を持つ
  - **プロダクトのあらゆる面に関わる**
  - コードを書く、POの仕事を手伝う、チーム外の組織と対話するなど

## スクラムデベロッパー
- スクラムの3つの鍵となる要素が機能していることに責任を持つ
  - **開発チーム内で働きかける**

最終的なゴールは両者とも同じだと思います。スクラムマスターのゴールは、自身がいなくなってもチームがスムーズに機能することであり、逆にスクラムデベロッパーであってもスクラムマスターの役割を一切果たさないというわけではありません。

## スクラムの3つの鍵
- **検査**
- **適応**
- **透明性**

検査と適応を継続的に繰り返すことで、プロジェクトを最適な状態に保ちます。
スプリントをグルグル繰り返すなかで、検査して情報を手に入れ、最新の情報で最新の計画を立て直します。
そして、透明性を維持するためには、インクリメントを継続的に生み出すことが重要なルールとなっています。
**透明性がない状態とは、インクリメントを作れない状態**だそうです。スキル不足だったり、スキルが足りていても知識不足だったり。
このプロセスと考え方を開発チーム内で根付かせることが、スクラムデベロッパーの主な役割であると私は理解しました。

スクラムデベロッパーの認定バッヂには次のように書かれています。

:::message
CSD認定者
- ツールとテクニックを使用して、スクラムに必要な反復的かつ増分的な方法で高品質のソフトウェアを構築します
- テスト駆動開発、受け入れテスト駆動開発、リファクタリング、および継続的統合を実行します
:::
:::message
認定要件
- 認定された CSD インストラクターが指導する教育サービスに24時間を超えて参加した
- 高価値製品をより早く市場に提供する能力を証明するためのクラス内の技術スキル評価を完了した
:::

# 研修でどんなことしたの？

研修期間は3日間でした。
1. 座学: アジャイルとは？スクラムとは？の話、TDDの話
2. 課題1: FizzBuzz問題をTDDでペアプロする
3. 課題2: より複雑な問題
4. 座学: スクラムの各イベントの話、CI/CDの話、ATDDの話
5. 課題2の続き
6. 課題3: レガシーコードでTDDを始める
ここでいうレガシーコードとは、テストを書いてないコードのこと 
7. 認定！

使用言語はJavaでした。エディタとしてはcyber-dojoを使用しました。
10人の参加者が、2人1組のペアプログラミングで課題に取り組みました。

エディターのコード補完が効かなかったため、コードの記述に時間がかかり、作業効率が低下しました。特に、長いメソッド名や変数名を正確に記入しなければならなかったことが課題となりました。
それでも、ビルドとテストの実行頻度をトレーナーが逐一確認できるように、cyber-dojoを使用する必要がありました。
ローカルのエディタで課題をしていたら、何も提出してないことになってしまいます。かと言って、ローカルで書いてコピー＆ペーストしていたら、TDDのサイクルを適切に回していないとみなされてしまう可能性があります。TDDでは、テストの実行とコードの実装を短いサイクルで繰り返すことが重要だからです。
それでも、Intellijでコードを書いてからcyber-dojoにコピペするという方法は効果的でした。

# 研修の難易度

課題は5割ほどしかできませんでしたが、認定してもらえました。これはトレーナー次第だと思いますが、課題をできる限り先に進めるよりも、全体を通してまじめに取り組むほうが大事な気がしました。

Javaの知識が必要でしたが、Javaの予習はゼロで挑みました。経験はあるがブランクが長いという状態です。ペアプロの相方はJava 7の頃には無かったStreamを使いこなしており、だいぶ助けられました。

宿題は出なかったので、忙しい時期でも3日間ぶんの予定さえ空けられれば問題なく受講可能でした。ただし、講義のテンポはとても早くてワークショップも多いので、受講中は複業などせず一点集中したほうがよいです。また、その日に理解しきれなかった部分は翌日の朝にノートを読み返したりすると、スムーズに理解が進む感じでした。

# スクラムデベロッパーの振る舞い
ここからは、研修から帰ってきて今後どうしていくかの所感です。

## 適応駆動の開発をリードする
- ❌計画駆動
- TDDやCIを導入
- Just in Timeにモノを届ける仕組みづくり
- 一番優先順位の高いものをただやり続ける
- What(作りたいもの)をHow(作る方法)に落とし込む

とくにTDDは今まで「最初にテストを書く手法」だと思い込んでいたので、なかなかやってみる気になれませんでした。
実際はテストと実装とリファクタをとても短いスパンで繰り返す手法だと知ったり、テストのないレガシーコードに対しても次に追加する部分から小さくテストを書いていけばよいと知ったりして、今からやってみようというハードルがだいぶ下がりました。

# 個人的な感想
## 私にとってのスクラムとは
自分の限界を引き上げるフレームワークだと感じました。

これまでは、予想外なことが起きたとき修正の振れ幅が大きいほどストレス値が高く、適応に時間がかかるのが課題でした。
検査と適応を小さく繰り返す習慣を得たことにより、普段やれることが増えるかもという期待の気持ちです。

# 自社で共有した反響
研修から帰って自社で情報共有しました。
寄せられた質問と回答です。

## 普段テスト書いてない人は対象外？
対象です。実際テスト書いてない方も参加されてましたし、そういう方でもTDDを始めやすい研修内容でした。

## 計画駆動より適応駆動が良いと思ったのはどの辺？
あらかじめ全部決めてその目標に向かうみたいなウォーターフォールを長くやってきて、予想外のことに対して弱いと感じていました。
その予想外に対して、開発者以外も巻き込みながら軌道修正をしやすいのが適応駆動の良いところだと感じています。
そしてまだまだアジャイルのほうが歴が短いので夢を見ている感じはありますが、小さく検査と適応を繰り返すほうが好みだと感じています。
ふだん目先の最優先のことに全力で向き合っているうちに状況が変わることが多いので、私の置かれている立場やチームにおいても、適応駆動のほうがマッチすると感じています。

## SMやSDは役割というよりスキルの名前？
これは私以外の方から「スキルよりも素質の有無で認定を貰う気がする」という回答がありました。
私自身もスクラムデベロッパーを受けてみて、認定を取ったことよりも私の適性やこれからどう振る舞えばよいかのヒントを持ち帰れたことが大きいなと感じました。

## 洞窟の宝箱全部拾いますか？
これはおもしろい質問でした。
私は全部集めるよりも目的地に早く着くほうを優先しますが、参加者からは全部拾うという意見が多く出ました。
もっと多くの方に聞いてみたいと思い、Xでアンケートしました！
https://x.com/tonionagauzzi/status/1718928479155351631?s=20

# 研修のまとめと今後の抱負
研修の最後に、スクラムはこうだから私の現場はよくない！みたいに思うのはNGだ、というお話がありました。
スクラムはチームの透明性を高め、コミュニケーションを促進し、持続可能なペースで作業を進めることを目指すアジャイルな方法論であり、問題を解決してくれるわけではないからです。

それをふまえてですが、実際仕事に戻って思ったのは、研修中に見聞きした多くのことを既にチーム内でも取り組んでおり、あるいは過去に取り組んだ経緯があって、私の現場へのスクラム浸透度の高さを感じました。
ただ、その一方で課題感がないわけではなく、私はここを忘れていたなとか、選択肢としてあらためて並べてみたいこともいくつかあると感じました。

具体的な例を挙げると、各プロダクトバックログアイテムの小タスクの1つで「テストを書く」というタスクを積んで、テストを書くことを忘れないようにしていました。その手法だとテストを書くのが最後になり、考慮漏れや手戻りが起きやすい状況でした。
早速TDDを取り入れてみたところ、テストして実装したらすぐに設計上の問題点に気づくことができて、検証の頻度が明らかに高くなりました。

こういった挑戦を繰り返してみて、私のチームのベストに近づいていきたいなと思います。
とにかく「やってみる」という私のスタンスに対して、私のチームがとてもオープンに歓迎してくれたのがうれしかったです。

## さいごに
私はウォーターフォールの経験が長く、最初からアジャイルという方々とは違う位置からのスタートを切ったため、研修で得た学びもまた違った特有のものだったと感じています。

とくにキャリアの初期は、自社が親会社から委託を受けて協力会社に再委託を行う、みたいな立場にいました。そのときはスケジュール的にも金銭的にも余裕がなく、その余裕のなさが学びの不足だったりメンタルバランスの崩れに直結していました。
詳しくは書けませんが、今ではおおよそ考えられないような体験も数多くしました。今思うとおかしいなと思う判断でも、当時は働くとはこういうものだと思っていました。
そのような状況を少しずつ変えてきて今に至るので、検査と適応を今まで以上に小さく回すことができるようになるのかと、研修を通して驚きと前向きな気持ちが得られました。

私のエンジニア人生もプロダクト寿命もまだまだ序盤戦のはずなので、メンタル的な余裕を持ち、全ての気づきをポジティブに捉えられるマインドとチームづくりを目指して行きたいです。

それぞれの方で感じ方は違うと思いますが、CSDを受けようか受けまいか悩んでいて受けるチャンスがある方には、受けることで私はこのように前向きに感じられたということだけお伝えしたいと思います。
