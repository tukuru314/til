markdownを使いこなそう
===


## 前提情報



[OmniMarkupPreview](https://pisuke-code.com/sublime-plugin-markdown-preview/#OmniMarkupPreview)

sublime textで使うとき  
HTMLでどう見えるのか確認するのに必要

>Ctrl  + Alt  + o(オー)  
>編集したマークダウンをプレビューできる 

>Ctrl+Alt+X  
>Markdown が HTML ファイルに変換され、Markdown ファイルと同じディレクトリに出力

>Ctrl+Alt+C  
>Markdown が HTML に変換され、クリップボードにコピー



これありきのページなのであしからず



## 見出し

```
# 見出し1
## 見出し2
### 見出し3
#### 見出し4
##### 見出し5
###### 見出し6
```


---

# 見出し1
## 見出し2
### 見出し3
#### 見出し4
##### 見出し5
###### 見出し6

---



## 改行


`半角スペース2つ`

改行を  
します

[HTMLを使って改行する場合]

```
hoge<br>
huga
```
hoge<br>
huga


### リスト（箇条書き）

```

`-` + 半角スペース  
`*` + 半角スペース  
`+` + 半角スペース

```

からのインデントをつける->階層構造を示す

```
- これ
	- ①
	- ②
	- ③
		- ①
		- ②
```

- これ
	- ①
	- ②
	- ③
		- ①
		- ②




## 番号付きリスト
```
1. わん
1. つー
1. ばきゅーん
```

1. わん
1. つー
1. ばきゅーん

```
1. わん
1. つー

1. ばきゅーん
```

1. わん
1. つー

1. ばきゅーん


## コード

~~~
これでコード化できる
~~~

こう`いうの`もある

上記のようなバッククオートはSHIFT + @ で出る

---

#### [リストのあとに繋げず書く方法](https://ja.stackoverflow.com/questions/2586/markdown%E3%81%A7%E3%83%AA%E3%82%B9%E3%83%88%E3%81%AE%E5%BE%8C%E3%81%AB%E7%B6%9A%E3%81%91%E3%81%A6%E3%82%B3%E3%83%BC%E3%83%89%E3%82%92%E6%9B%B8%E3%81%8D%E3%81%9F%E3%81%84%E5%A0%B4%E5%90%88)

```
- リスト１
- リスト２

<i />

    var x = 1;
```

- リスト１
- リスト２

<i />

    var x = 1;




## 参考先

1. [markdown（いち）](https://tatesuke.github.io/KanTanMarkdown/syntax.html)

	ここの編集・閲覧が一番見やすい

2. [markdown（に）](https://qiita.com/Qiita/items/c686397e4a0f4f11683d)

	その次に見やすい

3. [markdown（さん）](https://tech-blog.rakus.co.jp/entry/20200624/markdown)

	補足程度に
