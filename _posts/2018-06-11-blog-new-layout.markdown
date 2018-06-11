---
layout: post
title:  "ブログのデザインとレイアウトを更新 / CSSの醍醐味はレイアウトと配置かも"
date:   2018-06-11 03:00 +0100
categories: blog
tags: dev
author: Yuki Sato
description: 新しいブログのレイアウトで使ったhtmlとcssをシェアします。
image: "blog-new-layout.png"
---
![bootcamp](/img/blog-new-layout.png){:width="95%"}
上：トップページの新デザイン

ブログのデザイン、レイアウトを大幅にアップデートしました。  
以前は1コラムで、上からブログのリスト、ABOUT、WORKとだーーっと羅列するだけだったのですが、ブログ記事のサムネイル画像を使ったリストにしたり、2コラムにするなど、よりブログデザインぽくしてみました。

今回のアップデートで特に意識したのは **モバイル端末でもレイアウトが崩れにくくすること、かつ見やすさを保つこと** でした。

ブログのヘッダー、メインセクション、サイドバー、フッターといった主な構成要素を、崩れにくい形でどう配置すべきかどうか考え、CSSエキスパートの友人からもアドバイスをもらった結果、flexboxを活用してレイアウトを組むことにしました。

以下は、ダミーのコンテンツを入れてますが、基本的に新しいブログレイアウトで活用しているCSSになります。  
ヘッダーと、メインセクションにそれぞれflexboxを使っています。  

<p data-height="265" data-theme-id="0" data-slug-hash="dKNaEO" data-default-tab="html,result" data-user="yukisato" data-embed-version="2" data-pen-title="Blog Layout" class="codepen">See the Pen <a href="https://codepen.io/yukisato/pen/dKNaEO/">Blog Layout</a> by Yuki (<a href="https://codepen.io/yukisato">@yukisato</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

CSSの最初で、@media(min-width:550px) の中でセクションとヘッダーのdisplayをflexに設定しておくことで、画面が550pxよりも小さくなったときにはflexboxの設定が外れて、1コラムになるようにしてみました。

ここ1週間ぐらいは、CSSのレイアウトとポジションを勉強してたのですが、奥が深いです。
gridなど割と新しいレイアウト方法も普及してきて、選択肢は増えていますが、どれを使うのがベストプラクティスなのかというのを、これからも意識したいと思いました！

ではでは！
