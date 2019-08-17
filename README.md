本プロジェクトは Ruby on Rails 6 の開発を行うために必要となるDockerコンテナの定義ファイルを収録したものです。

Dockerの公式サイトの Rails 用のサンプル が載っている 下記URLのQuickstartにあるDockerfileやdocker-compose.ymlをベースに、Ruby やNode 等、Ruby on Rails 6 を実行する上で必要となる各種パッケージのインストールも行います

https://docs.docker.com/compose/rails/

以下のコマンドで即時にbuildが可能です。

```bash
$ docker-compose build --no-cache
```
