---
title: デモ記事作成しました
description: NetlifyCMSの使い心地を知るためにテストしています
---
## 動作テストしています。見出し見出し

文字を打っています。文字を打っています。文字を打っています。文字を打っています。

文字を打っています。文字を打っています。文字を打っています。



## 見出しがいっぱい

対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。対岸の火事。

対岸の火事。対岸の火事。対岸の火事。

```js{1,4}\[posts.vue]
formatDate(dateString) {
  const date = new Date(dateString)
  return date.toLocaleDateString(process.env.lang) || ''
},
async fetchPosts(
    postType = this.postType,
    amount = this.amount,
    sortBy = this.sortBy,
  ) {
  return this.$content(postType)
    .sortBy(sortBy.key, sortBy.direction)
    .limit(amount)
    .fetch()
    .catch((err) => {
      error({ statusCode: 404, message: amount > 1 ? 'Posts not found' : 'Post not found' })
    });
}
```

## とりわけ見出し

テキストテキストテキストテキストテキストテキストテキスト

> 引用引用引用引用引用引用
>
> 引用引用引用引用引用引用引用引用引用

どうでしょうか使いやすいか。いまのところ普通にWordPressのほうがいい感じがする。。