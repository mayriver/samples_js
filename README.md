# samples_js
JS samples

---
index_moto

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*



   */

   </script>
</body>
</html>
---
<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*
01_Java Script

* 概要
- ブラウザに実装されているスクリプト言語
- 動きのあるウェブサイトやインタフェイスを作るのによく使う

* リファレンスは、man javascriptで検索
https://developer.mozilla.org/ja/docs/Web/JavaScript

—
* 文の区切りと終りはセミコロン ;

* 変数： データにつけるラベル
- 変数を使うには必ず宣言をする
  宣言をする際には var
  = は代入演算子と呼ばれる。右辺のものを左辺に代入する　という意味

JavaScriptで扱える数値は
　数値
　　10 整数値
　　2.5　実数値
　　-2.5　マイナス値
　演算子
　　+ - * / %（余りを表す）
　　+= 代入を伴う演算子
　　++ — 単行演算子

* Windows 版の Chrome では「Ctrl + Shift + J」キーで JavaScript コンソールを起動できる。
　もしくはブラウザ右上にある横3本線のアイコンをクリックし、「その他のツール」-「デベロッパーツール」-「Console」


   */

   </script>
</body>
</html>
---
03_index_hensuu

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*
     変数： データにつけるラベル
	 
	 データ型
	 　- 文字列
	 　- 数値
	 　- 真偽値 (true / false)
	 　- オブジェクト
	 　　- 配列
	 	 　- 関数
	 　　- 組み込みオブジェクト
　　- undefind （アンデファインド）定義されていない
　　- null 何もない 
   */
   var msg;
   msg = "hello world!";
   console.log(msg) ;
   
   // 以下のように一気に書くことも可能
   var msg = "hello world!!";
   console.log(msg) ;
	
	//複数の変数があったときに以下のように一気に書くこともできる
	x = 20,
	y = 10;
   </script>
</body>
</html>
---
04_index_suuchi

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*
     変数： データにつけるラベル
	 
	 データ型
	 　- 文字列
	 　- 数値
	 　- 真偽値 (true / false)
	 　- オブジェクト
	 　　- 配列
	 	 　- 関数
	 　　- 組み込みオブジェクト
　　- undefind （アンデファインド）定義されていない
　　- null 何もない 
   */

   var x;
   x = 10 * 2; // 20
   x = 10 % 3 // 1（10を3で割った余り）
   x = x + 5; // 以下のように短く書くこともできる
   // x = x + 5;
   x += 5; // 6
   x++; // 7 1を足しなさい
   x--; // 6 1を引きなさい
   console.log(x);
   var msg;
   msg = "hello world!";
   console.log(msg) ;
   
   // 以下のように一気に書くことも可能
   var msg = "hello world!!";
   console.log(msg) ;
	
	//複数の変数があったときに以下のように一気に書くこともできる
	x = 20,
	y = 10;
   </script>
</body>
</html>
---
05_index_mojiretsu

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*
　　　文字列　"ダブルコーテーションで囲うか" 'シングルコーテーションで囲う'　どちらでも違いはない
　　　　　表現方法
　　　　　特殊文字
　　　演算子
   */
　　var s;
　　s = "hello";
　　s = 'hel\'lo';
   // \n 改行　Windowsだと ¥ 
   // \t タブ
   s = 'it\’s\n a pe\tn.';

   s = "hello " + "world";
   s = "5" + 5; //"55" なぜなら文字列と数値だから
   console.log(s);
   </script>
</body>
</html>
---
06_index_if

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*
    条件分岐によって処理を振り分けたいとき
    if (条件) {
        真
    } else {
        偽
    }

    比較演算子
    > <
    >= <= 〜以上、〜以下
    === 〜と等しい
    !== 〜と等しくない

    論理演算子
    AND &&
    OR ||
    NOT !
    score > 60 && score < 80 スコアが60より大きくて80より小さい
   */
var score = 50;
if(score > 60) {
    console.log("ok!");
} else if (score > 40 ) {
    console.log("soso...");
}
else{
    console.log("ng!")

}
   </script>
</body>
</html>
---
07_index_shingichi_sankouenzanshi

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*
      真偽値
         文字列：空文字以外だったらtrue
         数値： ０　か NaN（not a number）以外だったらtrue
         true / false
         object: null 以外だったらtrue
         undefind, null -> false
   */
   
   if (x) {
       // 処理
   }

   if (x !== '') {
       // 処理
   }

        /*
            三項演算子

            var a,b,c;
            if (条件) {
                a = b;
            } else {
                a = c;
            }
            a = （条件） ? b : c;
        */
        var max, x, y;
        max = (x > y) ? x : y;
        // この場合は、yより大きかったらxの方がmax、そうじゃなかたらyの方がmax　という意味

   </script>
</body>
</html>
---
08_index_switch

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
   <script>
   /*
        条件分岐
        switch
            ある変数が取りうる値が複数あって、それに応じて処理を振り分けたい場合にすっきり書くことが出来る構文
   */
   var signal = "red";

   switch(signal) {
        case "red":  // case : 選択肢
            console.log("stop!");
            break;  // break : 処理が終わった合図
        case "green": 
        case "blue": 
            console.log("go!");
            break;  
        case "yellow":  
            console.log("slow down!");
            break;  
        default:
            console.log("wrong signal");
            break;           
   }

   
   </script>
</body>
</html>
---
18_index_method_this

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
    <script>
        /*
            オブジェクト
                名前と値
        */
        var user = {
            email: "taguchi@gmail.com", // プロパティ
            score: 80,
            greet: function(name) { // メソッド
                console.log("hello, " + name + " from " + this.email);
            }
        };
        //console.log(user["email"]);
        //console.log(user.email);
        //user.score = 100;
        //console.log(user);
        user.greet("Tom");


    </script>
</body>
</html>
---
19_index_string

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
     <script>
        /*
            組み込みオブジェクト

            - String
            - Array
            - Math
            - Date
        */
        // var s = new String("taguchi");
        var s = "taguchi"; // 文字列リテラル
        console.log(s.length);
        console.log(s.replace("t", "T"));
        console.log(s.substr(1, 3));


    </script>
</body>
</html>
---
22_index_dom6

<!DOCTYPE html>
<html lang="ja">
<head>
   <meta charset="UTF-8">
   <title>JavaScript :D</title> 
</head>
<body>
    <h1>見出し</h1>
    <p id="msg">こんにちは！</p>
   <script>
   /*
   ブラウザを扱うためのwindowオブジェクト、それからDOMについても。
    windowオブジェクト
    DOM

        // console.dir(window);
        // console.log(window.outerHeight);
        // window.location.href = 'http://dotinstall.com';

        // document - 今開いているページ

        // document object model (DOM)



   */

   </script>
</body>
</html>
---
23_index_dom

<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="utf-8">
    <title>JavaScriptの練習</title>
    <style>
        .myStyle {
            font-weight: bold;
            border: 1px solid gray;
        }
    </style>
</head>
<body>
    <h1>見出し</h1>
    <p id="msg">こんにちは！</p>
    <script>

    /*
    DOMを使ってページ内の要素を操作してみます。
        document.getElementById
    createElement
    createTextNode
    appendChild
    */

        var e = document.getElementById('msg');
        e.textContent = 'hello!';
        e.style.color = 'red';
        e.className = 'myStyle';

        /*
            body
                p
                    text
        */
        var greet = document.createElement('p'),
            text = document.createTextNode('hello world');
        document.body.appendChild(greet).appendChild(text);

    </script>
</body>
</html>
---
24_index_event

<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="utf-8">
    <title>JavaScriptの練習</title>
    <style>
        .myStyle {
            font-weight: bold;
            border: 1px solid gray;
        }
    </style>
</head>
<body>
    <h1>見出し</h1>
    <p id="msg">こんにちは！</p>
    <button id="add">Click!</button>
    <script>

/*

ページ内の要素にクリックイベントを設定する方法について見ていきます。
addEventListener

*/

        var e = document.getElementById('msg');
        e.textContent = 'hello!';
        e.style.color = 'red';
        e.className = 'myStyle';

        /*
            body
                p
                    text
        */

        document.getElementById('add').addEventListener('click', function() {
            var greet = document.createElement('p'),
                text = document.createTextNode('hello world');
            document.body.appendChild(greet).appendChild(text);
        });

    </script>
</body>
</html>
---



