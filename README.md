# azure-container-dev-book

『Azure コンテナアプリケーション開発』（技術評論社，2023 年）のサンプルコード

## 書誌情報

Azure コンテナアプリケーション開発

- 真壁徹、東方雄亮、米倉千冬、谷津秀典、阿佐志保 著, 技術評論社, 2023, 978-4-297-13269-9
- https://gihyo.jp/book/2023/978-4-297-13269-9

本書に関するお問い合わせについては、技術評論社の書籍ページのフォームをご使用ください。

## ローカルで　 github workflow を実行する

- 1. act を devcontainer に設定する

  ```
  "features": {
   // Act is an open source project that allows you to run your github flow locally.
    "ghcr.io/devcontainers-contrib/features/act-asdf:2": {
      "version": "latest"
    },
  ```

- 2. ターミナルで GITHUB_TOKEN と ジョブ名 を指定して実行
  ```
  $ act -s GITHUB_TOKEN=ghp_xxxxxxxxxxxx -j test2
  ```
