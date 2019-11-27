# classes-memo

## なにこれ

講義メモや講義資料へのリンクをまとめて置くためのリポジトリ.  
まじめに講義を受けよう！

## 使い方

緑色のボタンから"clone"をしてね.  
cloneはリモートリポジトリ(Web上にある保存場所的な)から自分のローカルリポジトリ(手元のパソコンにある保存場所)にダウンロードすることやで.  

そのあとcloneしたリポジトリが自分のパソコンのどこかにディレクトリとして存在してるので、ターミナルでそこに行ってくれ.  

あとはそのディレクトリでgitコマンドを使っていろいろ操作ができるぞ！  

主に使う奴はadd, commit, pushだ.  

### add
手元で変更したファイルを「このファイルをcommitする準備しまーす」的なことをやるぞ.commitしたいファイルを細かく調整可能だ.面倒臭かったら
```
git add -A
```
で全ファイルのcommit準備が整うぞ.  
addは準備をするだけなので特に目立った変更はないぞ.

### commit
このコマンドで変更履歴を保存するぞ.作業の区切り(よく見るのは,新しい機能を追加した〜とか仕様を変えた〜とか).  
commitする時は何かメッセージをつけるのが普通や!  
-mオプションをつけることで、commitメッセージを記述できるぞ.  
```
git commit -m "commit message"
```
ちなみに,addされたファイルしかcommitされないので,変な奴をcommitしないようにaddする時から気をつけるヨロシ!  
(.gitignoreというファイルを用意するとaddした際に無視するファイルを指定できるぞい)  

commitされた変更分はあくまでローカルリポジトリの中でだけ有効で,まだリモートリポジトリには反映をしていない段階なので,commitだけしててもGitHubは何も更新されないゾ.  

### push
commitされたローカルの変更分をリモートリポジトリに反映するぞい!  
GitHub上で変更が反映されているのが確認できればおっけーや！  
pushはこんな感じや!  
```
git push origin master
```
ところでこのorigin,masterというのはそれぞれ

- origin: リモートリポジトリのoriginという名前のブランチ
- master: ローカルリポジトリのmasterという名前のブランチ

を表していて,ローカルリポジトリのmasterブランチの作業内容を,リモートリポジトリのoriginブランチに反映する,ということをしているぞ!  

## あとはLINEください


