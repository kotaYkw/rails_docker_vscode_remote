# README

vscodeのRemote Contanersを使ってdocker containerに接続をするために必要なファイル構成です。

環境構築にあたって重要なファイルは以下の通りです。

* .devcontainer

  * devcontainer.json

  * Dockerfile

* config

  * database.yml

* docker-compose.yml

* entrypoint.sh

* Gemfile

* Gemfile.lock

# 手順

1. vscodeの拡張機能、Remote Contanersをインストールして再起動する。

`git clone https://github.com/kotaYkw/rails_docker_vscode_remote.git`  

でリポジトリをクローンする。

1. vscode左下の`><`のマークを押して、
> Remote-Containers: Open Folder in Container...  

からクローンしたファイルを開く。

1. `bundle install`を実行する。

1. `rails db:create`を実行する。

1. `rails s -b 0.0.0.0`を実行し、[localhost](http://localhost:3000/)に接続できれば成功。

