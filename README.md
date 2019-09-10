Kristallweizen（評価関数のみ）  
  
これは第29回世界コンピュータ将棋選手権で準優勝したKristallweizenの評価関数です。  
評価関数はNNUE型で作成されており、やねうら王にマージされているNNUEのディフォルトの  
NN構成と同じ、HalfKP-256x2-32-32となっています。  
  
使用環境  
  
やねうら王Ver4.83のNNUE版を実行できる環境であれば、評価関数をそのまま差し替えるだけで  
動作します。  
  
もしものために、実行バイナリも用意しました。 
   
Kristallweizen-wcsc29-avx2.exe  
Kristallweizen-wcsc29-sse42.exe  
  
この実行バイナリを利用する際には、評価関数ファイル名をnn.binからbeer.binに変更して  
ご利用ください。（ささやかなネタですｗ）  
  
～avx2.exeのほうで動かなかったら、～sse42.exeのほうで試してみてください。  
  
その他  
  
強さに関しては、選手権ギリギリまで学習を粘っていた関係で正直よくわかっていません。w  
まぁ、準優勝するぐらいは強かったのでしょうが……。^^;  
選手権後にほんのちょっとだけ illqha4 + やねうら王と1億ノード指定、定跡なしで対局させて  
みましたが、10局やって 4勝 4敗 2分、どちらの評価関数も勝ったのは先手番のみという極端な  
結果が出ました。これは私の計測条件がおかしい可能性もありますので、どなたか検証して  
いただけると助かります。  

また、短時間対局では異様に弱いことも付記しておきます。最低でも5000万ノードは読ませないと  
ダメダメでした。  
  
弱くてがっかりしたらすみません。そうだったらそれは探索部がちょ～優秀だったせいで準優勝  
したのだと思ってください。  
  
  
2019.9.6  
Kristallweizen改（評価関数のみ）リリース  
  
ちょっとした実験で作成してみた評価関数です。思いの外いい感じだったので公開します。  
  
Kristallweizen_kai.zip  
  
細かく検証したわけではないのですが、試しに水匠改と定跡なし1600万ノードで10局やって  
7勝2敗1分だったので、潤沢なリソースをお持ちの有志の方々に検証いただけると幸いです。  
  
  
2019.9.10  
Kristallweizen改（評価関数のみ）その２ リリース  
  
Kristallweizen_kaiV0.2.zip  
  
ちょっと怪しげなツールができたので、実験ししています。  
実験内容に関しては、今はまだ明かさないでおきます。^^;  
みんな気になってたことをやってみてます。  
今回アップしたのはGrampus3に7勝2敗1分したものです。前回のとは違うことをしたものです。  
  
  
以上  
