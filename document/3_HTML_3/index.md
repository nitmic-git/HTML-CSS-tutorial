# HTMLの書き方 よく使うタグ編
前回まででは、HTML全体やbodyの中の構造について学びました。

今回は、bodyの中で本文を記述するときに使われるタグについて学んでいきます。

## まずはみてみよう
とりあえず、サンプルを見ながら学習を進めたいので、先ほどのhtmlファイル(index.html)の中身を消去して、下のコードを貼り付けてください。

```html
<!DOCTYPE html>
<html>

<head>
</head>

<body>
    <h1>Hello, Sora!</h1>
    <h2>Hello, Sora!</h2>
    <h3>Hello, Sora!</h3>
    <h4>Hello, Sora!</h4>
    <h5>Hello, Sora!</h5>
    <h6>Hello, Sora!</h6>

    <p>My Name is Sora.</p>

    <p>Below is a link to my website.<br>You can check it out if you like.</p>

    <p><a href="https://sayagi.net">This is My Website</a></p>

    <img src="https://dummyimage.com/300" alt="dummy image">

    <!-- 番号つきのリスト -->
    <ol>
        <li>This is a list</li>
        <li>with</li>
        <li>numbers</li>
    </ol>

    <!-- 番号なしのリスト -->
    <ul>
        <li>This is a list</li>
        <li>without</li>
        <li>numbers</li>
    </ul>

    <p>You can find out more through <a href="https://developer.mozilla.org/ja/docs/Web/HTML/Reference">MDN Web Docs</a>.</p>

</body>

</html>
```

そして、ブラウザ(Live Server)が更新されていることを確認してください。何やらいろいろ映っていれば成功です。

## 説明
表示されたことが確認できたら、説明に移ります。

### hタグ
```html
    <h1>Hello, Sora!</h1>
    <h2>Hello, Sora!</h2>
    <h3>Hello, Sora!</h3>
    <h4>Hello, Sora!</h4>
    <h5>Hello, Sora!</h5>
    <h6>Hello, Sora!</h6>
```
h1、h2、h3などのタグの総称を、hタグといいます。これは、見出しを定義するのに使われます。
h1～h6タグまで存在して、h1が最も上位の見出しで、そこから数字が上がるに連れ順位が下がっていきます。

hタグの利用には、いくつかユーザーやサーチエンジン(GoogleやYahooなど)にうまく伝えるためのルールがあります。
1. h1タグから始める
    
    最初はh1タグから使っていったほうがいいです。たとえば、次のような書き方は好ましくありません。
    ```html
    <h2>大見出し</h2>
    <h3>中見出し</h3>
    <h4>小見出し</h4>
    ```
    この例では、h1タグを飛ばして、h2タグから始めています。このような記述方法だと、特にサーチエンジンに、うまく伝えたいことが伝わらない可能性が出てきます。あまり好ましくないと言えるでしょう。

1. 途中のタグを飛ばさない
    途中で、次のようにタグを飛ばしてしまうのは好ましくないです。
    ```html
    <h1>大見出し</h1>
    <h3>中見出し</h3>
    <h4>小見出し</h4>
    ```
    この例では、h1タグから始まっていますが、h2タグを飛ばしてh3タグを使っています。このような記述方法も、サーチエンジンがうまく解釈してくれない可能性が出てきてしまうため、あまり好ましくありません。

1. h1タグを乱用しない
    次のように、すべての見出しをh1で記述するのも好ましくありません。
    ```html
    <h1>大見出し</h1>
    <h1>中見出し</h1>
    <h1>小見出し</h1>
    ```
    このように記述してしまうと、サーチエンジンが、文の構造を正しく理解できない恐れがあるため、h1タグの利用は1ページには1つ程度にしておきましょう。

### pタグ
```html
    <p>My Name is Sora.</p>
```
pタグは、段落を定義するのに使われます。1段落をpタグで囲えば、段落の区切りで改行を行ってくれます

### brタグ
```html
    <p>Below is a link to my website.<br>You can check it out if you like.</p>
```
HTMLの中では、ソースコード側の改行は(1部のタグの中をのぞいて)、基本的に反映されません。
HTML文書中で、段落を分けずに改行を行いたい場合は、\<br>タグを使用します。

### aタグ
```html
    <p><a href="https://sayagi.net">This is My Website</a></p>
```
aタグは、ほかのウェブページなどのリンクを作成するのに使われます。

タグの中の"href"と書かれている部分は、href属性と呼ばれ、ここにリンク先を指定することで、リンクを作成できます。

例のようなテキストだけではなく、画像などもaタグの中に入れることができるので、大変便利です。

### imgタグ
```html
 <img src="https://dummyimage.com/300" alt="dummy image">
```
imgタグは、画像を表示するのに使用します。

srcやaltと書かれている部分は、それぞれ、src属性、alt属性と呼ばれ、src属性に画像のURL(もしくは相対パス)を設定します。alt属性に画像が表示されない際や、読み上げに使用する代替テキストを指定します。

### ol、ul、liタグ
```html
    <!-- 番号つきのリスト -->
    <ol>
        <li>This is a list</li>
        <li>with</li>
        <li>numbers</li>
    </ol>

    <!-- 番号なしのリスト -->
    <ul>
        <li>This is a list</li>
        <li>without</li>
        <li>numbers</li>
    </ul>
```
HTMLでリストを作成したいときは、ol、ul、liタグを使用します。
上のコードのようにすると、それぞれ番号あり、番号なしのリストが作成できます。
リストの見た目は変更できますが、olは順番があるリスト、ulは順番のないリストと考えておくといいと思います。

### そのほかいろいろなタグ

今回触れたのは、よくお世話になる基本的なタグたちです。[MDN Web Docs](https://developer.mozilla.org/ja/docs/Web/HTML/Reference)のHTMLリファレンスを見ると、たくさんのタグがあることがわかると思います。是非眺めて、こんなタグがあるんだな～と思いながら、実際に使ってみてください。

そのほかにも、"HTML タグ"や、"HTML 入門"などで検索すると、いろいろな情報が出てくるので、いろいろ確認してみるといいかと思います。

以上が、HTMLの入門になります。次は、CSSを用いてHTMLのスタイルを整えていこうと思います。

前の記事:[3.2.HTMLの書き方 よく使う要素編](../3_HTML_2/index.md)
次の記事:[4.1.CSSの書き方 構造編]()
