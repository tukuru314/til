## privateとpublicの切り替え方法

ブラウザ上でgithubを開く

リモートレポジトリ内で
setting->General->Danger Zone->change visible
で変更する

https://yu-report.com/entry/githubprivate/


## VSCODEでGITを使うには

基本的にはまずプロジェクトにあたるフォルダを作成して
そこでgit init　をCLI上でうってGITの基本を作成する

それでローカルレポジトリが作られる。

GITHUBのアカウントにそのローカルレポジトリを
リモートレポジトリへと追加したい場合はCtrl+Shift+PでGITHUBに公開を選べば
追加することができる

もちろんローカルレポジトリだけでバージョン管理してもよい


## GITでブランチを切るには

基本的にはソース管理の中のレポジトリを選択してすぐ右のmainなどをクリックすれば
コマンドパレットに新しくブランチを切るなどが出てくるのでそれを選択すればブランチを
切ることができる
それが終わったらリモートレポジトリに反映させるようにそのさらに隣の変更の同期を押して
あげればリモートレポジトリに反映させることができる

これによってブランチをきって作業することができて便利

## JAVAの開発環境では

エクリプスにもGITを入れられる
ウインドウのタブ＞パースペクティブ＞パースペクティブを開く＞その他＞GIT でGITを管理するのに適した画面にすることができる
そして普段の画面にカスタマイズでGITを追加することもできる
基本はそちらになるはず


## .gitatrributesファイル

LINUXとMACとWINの改行をうまいこと調整するためのファイルらしい　

https://qiita.com/nacam403/items/23511637335fc221bba2


## GITに個人情報をあげると大変らしい

消す方法は下記参照

https://ashitamo-net.com/git-github-remove-history-including-sensitive-data/#:~:text=git%20filter%2Dbranch%E3%81%BE%E3%81%9F%E3%81%AFthe,%E3%81%8C%E3%81%8A%E3%81%8A%E3%81%BE%E3%81%8B%E3%81%AA%E6%89%8B%E9%A0%86%E3%81%A7%E3%81%99%E3%80%82
