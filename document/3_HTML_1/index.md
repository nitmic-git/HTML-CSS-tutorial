# HTMLの書き方　構造編
HTMLの書き方を、コードを書きながら学んでいきます。

## ファイルの作成
前回の最後で、フォルダをVSCodeで開いたところで終わっていると思います。

左側にある、エクスプローラータブにカーソルを持って行くと、フォルダ名の横に、記号が出てくると思うので、フォルダを作りたいなら、フォルダマークを、ファイルを作りたいならファイルマークをクリックしてください。

今回は、ファイルマークをクリックしてファイルを作成してください。

ファイル名は、index.htmlとしてください。HTMLのファイルの拡張子は、.htmlです。

## 実際に書いてみよう！

ファイルを作成すると、自動的にそのファイルの編集画面が開かれたかと思います。

そこに、次のコードをコピーして貼り付けしてみてください。

```html
<!DOCTYPE html>
<html>
    <head>
    </head>

    <body>
        <h1>Hello, World!</h1>
    </body>
</html>
```

コードが少し崩れてしまったなと思ったら、そのままでも問題ありませんし、Alt+Shift+Fでコードを整形することもできます。

そしたら、コードの書いてある場所を右クリックして、Open with Live Serverをクリック！ 

すると、ブラウザが立ち上がって、Hello, World!の文字が！成功です！

これが、あなたのHTMLの第一歩！

出てこなかったら、しっかりコピーできているかなど、確認してみてください。

ちなみに、"Hello, World!"部分の文字"Hello, Sora!"などに変えると、再読み込みしなくても自動で反映されます。便利。

## 説明

とりあえず表示ができたところで、HTMLの説明に移ります。

### HTMLの構造

htmlタグ、headタグ、bodyタグの3つで構成されています。

それぞれの役割や、タグって何？ということを解説していきます。

### <>?
<>でかこまれたものは、タグと言われます。これがHTMLの特徴で、このタグを駆使してウェブサイトを作っています。

```html
<html>
<!-- この上のタグは、開始タグと言われるタグ。かっこで囲むだけ。 -->

<!-- これはコメント、これで囲むと、ページには表示されない。 -->

<!-- この下ののタグは、終了タグと言われるタグ。かっこにスラッシュで囲む。 -->
</html>
```
わかりましたか？開始タグと終了タグ。
しかし、すべてのタグに終了タグがあるわけではなく、一部終了タグが存在しないタグもあります。注意。

### DOCTYPE
```html
<!DOCTYPE html>
```
これは、"この文章が、HTML5で作成されたものです！"と宣言するものです。
昔は
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```
とか宣言されていたんですね。これは、HTML 4.01 Transitionalの宣言です。大分シンプルになりました。

これにより、HTMLのバージョンを宣言できるわけです。

この子は、終了タグないです。

### \<html>\</html>
```html
<html>

～～～

</html>
```

これは、この文書がHTMLです！と宣言しています。DOCTYPEはあくまでもバージョンを宣言するタグです。DOCTYPEを除く要素は、このタグの内側に配置されます。

### \<head>\</head>

```html
<head>

～～～

</head>
```

このタグの中には、この文書のタイトルや、著者、説明などなど、文書に関する情報を記述していきます。
タイトル以外は、あまりブラウザに表示されないけれど、検索エンジンのためにいろいろ書いておく感じです。

### \<body>\</body>

```html
<body>

～～～

</body>
```

このタグの中には、この文書の本体を記述していきます。実際にブラウザに表示される部分は、ここに入れます。

## もう一回コードをみてみよう
もう一度先ほどのコードを見てみましょう。

たしかに、説明の通りに、html、head、bodyタグから構成されています。

\<h1>\</h1>のタグに関しては今回説明しませんでした。後に説明します。

前の記事:[2.開発環境を整える](../2_environment_setup/index.md)
次の記事:[3.2.HTMLの書き方 bodyの構造編](../3_HTML_2/index.md)

[目次に戻る](../../README.md)