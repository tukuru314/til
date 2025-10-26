
## 自宅で学ぶDockerで使ったコマンドを記載していく

基本的には自宅を使うdockerを見ながらすすめていこう。
Dockerのインストールは公式から最新を。CE(個人用)を使え。使うんや。

前提条件として

・コンテナIDは cd6... とします
・イメージIDは im0... とします

実践では本当のIDに変更して、コマンドを打とう



［イメージを取得］
docker pull ubuntu

［イメージ一覧を見る］
docker images -a

［イメージを消す］
docker rmi im0....

［イメージをすべて消す］
docker image prune

［イメージからコンテナを生成して起動］
docker run -it ubuntu /bin/bash

※itをつけ忘れるとシェルが起動しない、そのときは
docker stop cd6...で一旦コンテナをstopして再度
docker start -ai cd6...でコンテナを起動させよう

［コンテナ内でコンテナを終了する］
exit

［コンテナ一覧を見る］
docker ps -a

［コンテナを再び起動する］
docker start -ai cd6...

［コンテナを停止する］
docker stop cd6...

［コンテナを削除する］
docker rm cd6...

［コンテナを一括ですべて削除する］
docker container prune
※停止状態のデータボリューム・コンテナがあると削除されてしまうから注意

［コンテナの中のtmpにファイルをつくる］
touch tmp/hello-docker.txt

［ファイルができているか確認］
ls tmp/
確認できたら
exit

［もう一つコンテナを起動する　と違うコンテナIDで作られることがわかる］
docker run -it /bin/bash

［コンテナを一括ですべて削除する］
docker container prune
別IDでつくられることを確認したら全てのコンテナを消去する

［ubuntuコンテナにpingインストールしていく］
docker run -it --name=ping_in_ubuntu ubuntu /bin/bash

［aptをアップデート］
apt update

［pingをインストール］
apt install uputils-ping

［ping を実行する］
ping localhost
停止はCTRL+Cで、できる

［運用時に不必要なものを削除する］
apt clean
rm -rf /var/lib/apt/list/*


［attachはコンテナを全面で動かす、dettachはコンテナを背後で動かす］
docker attach cd6...

［コンテナをイメージ化する］
docker commit cd6... ping_in_ubuntu

ping_in_ubuntuはコンテナのイメージ名
ちなみにこれを二回繰り返すと新しいほうにping_in_ubuntuの名前が付与されて
古いほうはNONEになってしまうので注意が必要

［］