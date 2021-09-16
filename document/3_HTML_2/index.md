# HTMLの書き方 bodyの構造編
前回は、HTML全体の構造を学びました。

今回は、そのなかでも特に本体であるbodyの構造について学んでいきます。

## まずはコード
さきほどのindex.htmlの中身を消去して、下のコードを貼り付けしてみてください。

```html
<!DOCTYPE html>
<html>

<head>
</head>

<body>
    <header>
        <h1>Sora's Website!</h1>
    </header>
    <main>
        <h1>Hello, Sora!</h1>
    </main>
    <footer>
        <p>&copy; 2021 Sora513</p>
    </footer>
</body>

</html>
```

そして、ブラウザ(Live Server)が更新されていることを確認してください。何やらいろいろ映っていれば成功です。

## 説明
表示されたことが確認できたら、説明に移ります。

## bodyの構造
header、main、footerなどから構成されます(ほかにasideなどが使われる場合もありますが、今はおいておきます。)。

### \<header>\</header>
名前の通り、ヘッダー(サイトの上部に表示される、サイトの名前や、ナビゲーションなど)を定義するのに使われます。
```html
    <header>
        <h1>Sora's Website!</h1>
    </header>
```

### \<main>\</main>
名前の通り、メインコンテンツを定義するのに使われます。ページが違っても共通のコンテンツ(ヘッダーやフッターに書く内容)は、mainの中には入れません。
```html
    <main>
        <h1>Hello, Sora!</h1>
    </main>
```
### \<footer>\</footer>
名前の通り、ヘッダー(サイトの下部に表示される、コピーライトやサイトマップなど)を定義するのに使われます。

```html
    <footer>
        <p>&copy; 2021 Sora513</p>
    </footer>
```

この"\&copy;"というのは、&copy;といった記号などを書くことができる特殊文字と言われるものです。気になる人は、HTML 特殊文字で検索してみると面白いでしょう。

### もう一度コードを見てみよう
たしかに、説明の通りに、header、main、footerタグから構成されています。

\<h1>\</h1>のタグに関しては今回も説明しませんでした。次回説明します。

前の記事:[3.1.HTMLの書き方　構造編](../3_HTML_1/index.md)
次の記事:[3.3.HTMLの書き方 よく使うタグ編](../3_HTML_3/index.md)

[目次に戻る](../../README.md)