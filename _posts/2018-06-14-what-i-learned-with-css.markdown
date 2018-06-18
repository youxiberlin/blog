---
layout: post-layout2
title:  "CSSの学び"
date:   2018-06-14 03:00 +0100
categories: blog
tags: dev css
author: Yuki Sato
description: ここ10日間ほどCSSを学んでいて、気づいたことなど。
image: "css-code.jpg"
---
![code](/img/css-code.jpg){:width="100%"}
<small style="color: #777;">Photo by [Marc Mueller](https://unsplash.com/photos/Lg8xTZjs6Lg?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on Unsplash</small>

ここ10日間ほどCSSを集中的に学んでいたのですが、そのプロセスでいろいろ得られた気づきを備忘録もかねて書いておきます。

* 最初に骨格をつくって、全体のレイアウトを決めること
* コードを書くときに意識したいのは「シンプルであり、協業・メンテナンスがしやすいこと」
* 色や細かな装飾は最後に

### レイアウトとポジショニングが醍醐味

今回、このブログのレイアウトの組み方を大幅にアップデートしたり、
練習のために他のサイトのトップページをいくつかコピーして作ってみました。
CSSは外見を調整するためのものということで、フォントスタイルだったり、カラーだったり    
そういった細かいビジュアルを整える技が注目されることが多いですが、
やはり一番難しく、かつ学びがいがあるのはレイアウトとポジショニングだと思いました。

前回の記事でもシェアしましたが、ブログのアップデートの際に作った、このブログのおおまかなレイアウトはこちらになります。
<iframe height='265' scrolling='no' title='Blog Layout' src='//codepen.io/yukisato/embed/gKgqyG/?height=265&theme-id=0&default-tab=html,result&embed-version=2' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>See the Pen <a href='https://codepen.io/yukisato/pen/gKgqyG/'>Blog Layout</a> by Yuki Sato (<a href='https://codepen.io/yukisato'>@yukisato</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### シンプルであり、協業・メンテナンスがしやすいコードを書く

ブログのアップデートを重ねていたら、気づくとコードがとても冗漫で、見にくいものとなっていました。

一つの部位に対して、a タグ、 headingのタグ、 div タグなど複数のタグが被さって、それぞれのタグで設定しているものが被っていたりとか。。後から見直すと、ほんとにこの divタグは必要なの？ というような部分が散見されました。

あと、クラスやID名も最初は適当につけていたので、とても分かりにくくなってしまっていました。  
まだ自分一人で管理しているブログだからよいものの、このままじゃ他の人と協業したりすることは難しい状態で。  
自分だけで管理するにしても、メンテナンスがしにくいのは長期的に考えるととても非効率です。

なので、今回のアップデートを機に、それぞれの要素の役割を見直し、プロパティも被りがないようにし、クラス名も機能に応じた名前にして、コードを見るだけでそのアウトプットが想像しやすいような形にしました。

### 色や細かな装飾は最後に
CSSをいじるとなると、どうしても色やグラデーションなど、ビジュアルに凝りたくなってしまいがちなのですが、
統一感のあるサイトをデザインするにあたっては、最初に全体の構成を考えて、骨組みをつくり、細かい仕上げは最後にするのが流れとしてはベストだと思いました。  
インテリアやファッションにしても同じことが言えますね・・・

以上が、CSS初学者の気づきです！

それでは！

PS：このブログのコードはこちらの[githubレポジトリー](https://github.com/youxiberlin/blog)で公開しています。
