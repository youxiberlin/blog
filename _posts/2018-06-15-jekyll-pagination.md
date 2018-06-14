---
layout: post-layout
title:  "Jekyll Paginationプラグインを追加してみました"
date:   2018-06-14 03:00 +0100
categories: blog
tags: dev jekyll
author: Yuki Sato
description: ブログの投稿が増えた時に自動的にページが追加されるように、Paginationプラグインを追加してみました。
image: "journal.jpg"
---
![code](/img/journal.jpg){:width="100%"}
<small style="color: #777;">Photo by [Jess Watters](https://unsplash.com/photos/cvUIv9j5wDg?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on Unsplash</small>

JekyllのPaginationプラグインを追加してみました。  
この機能を追加すると、ブログの投稿が増えた時に自動的にページが追加されるようになります。
たとえば、このブログでは1ページの投稿数を6件と設定しており、それを越えると自動的に次のページに表示されるようにしました。

Pagination 機能については、こちらが[公式の説明](https://jekyllrb.com/docs/pagination/)になります。

やったことをおおまかに書くとこんな感じです：
* jekyll-paginate プラグインを追加
* 新たにルートに「blog」フォルダを作り、その中にindex.htmlファイルをつくる
* [Render the pagination posts](https://jekyllrb.com/docs/pagination/#render-the-paginated-posts)を参考に、コードを書く。

プラグインの追加についての説明は[こちら](https://jekyllrb.com/docs/plugins/)です。
configファイルやGemfileにプラグインを書き加える必要があります。

ちなみに、私の /blog/index.html のソースは[こちらから](https://github.com/youxiberlin/blog/blob/master/blog/index.html)見れます。

少しずつブログが良くなってきて、うれしいです！

それでは！
