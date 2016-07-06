_test_
__test__
*test*
**teat**
`test`

* te
* st

# H1
## H2
###### H6

=====
-----



＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊  
  
以下[]内を指定のものに変えてください。  
基本的に以下に書いたコマンド以外は使いません。  
  
＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊＊  

マスターブランチに移動
    git checkout master

作業をするときはブランチを作る
branch名は、スクリプト/モデル名にしてください。

    git branch [branch名]


    例) git branch MainObjectMenuManager
    例) git branch model_ball


作成したブランチに移動する
    git checkout [branch名]

ブランチを作ったら、指定の場所にスクリプト/モデルを作る。その後、

    git add [ファイルの場所]
    git commit -m “[branch名]の制作”
    git push origin [branch名]

ブラウザ上の [escapeVR_3Gのページ](https://github.com/shihoooox/escapeVR_3G "escapeVR_3G")で
「Compare & pull request」を押す。移動先のページで、

    ーーーーーーーーーーーーーーーーーーー
    タイトル : [スクリプト名]の制作
    コメント : 
    - [ ] メソッド名（モデルの場合必要無し）
    - [ ] メソッド名
    	　：
    ーーーーーーーーーーーーーーーーーーー 
> ーーーーーーーーーーーーーーーーーーー
> @@@@@@@@@@
> @@@@@@@
> ーーーーーーーーーーーーーーーーーーー 
＊＊ - [ ] はチェックボックスのコマンドです ＊＊

    例)
    ーーーーーーーーーーーーーーーーーーー
    タイトル : MainObjectMenuManagerの制作
    コメント : 
    - [ ] Start
    - [ ] Update
    - [ ] setObject
    - [ ] unsetObject
    ーーーーーーーーーーーーーーーーーーー 

を入力し、Create pull request を押す
これで作業を行うブランチの準備ができました。

メソッドを作り終えるたびに、ブラウザ上の `Pull requests` でチェックボックスにチェックを入れる
それにより進捗確認を行う
*チェックボッスクスは同期されているため、他人のページのチェックボックスは触らない*


ある程度作業が進む or 作業が終わったら、

    git add [ファイルの場所]
    git commit -m “[進捗状態]”
    git push origin [branch名]

を行う

全ての作業を終えたら、LINEグループでその旨を伝える
岡本さんがプログラム/モデルをチェックして、合格したら岡本さんがmergeする

次の作業を始める時は上に戻る
＊＊＊ masterブランチに戻るのを忘れないように ＊＊＊