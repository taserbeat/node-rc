# VSCode Remote Container のサンプル

VSCode の Remote Container で React 環境を整えてみた。

# 個人メモ

- リポジトリの[.devcontainer](./.devcontainer)に Remote Container でコンテナの起動設定や Dockerfile を格納する

- Git の設定は接続元であるホストの設定が継承される

- コンテナ内で`yarn start`などのコマンドの処理時間がが長い (Mac)

  - 解決への参考: [Mac で使う VS Code と Remote Container の性能を大幅改善](https://www.keisuke69.net/entry/2021/09/15/104532)

- コンテナ内から SSH 接続で GitHub に push するときに、アクセス権がないと怒られた

  - コンテナ内では SSH の秘密鍵を持っていないので当然といえば当然

- コンテナ内から HTTPS で GitHub に push することはできる

  - ただし、認証がめんどい
