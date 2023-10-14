
# NodejsとPostgresを接続した時に学んだこと

- psql + nodejsでAPI接続
    - 参考記事
        - https://teech-lab.com/node-express-postgres-pool/1243/
    - 基本的な流れ
        - npm install pg
        - conection poolを定義
            - postgresのポート番号は5432
        - 定義したconnection poolに対してsqlを実行
- フロントエンドとバックエンドでpackage.jsonを共有しているのはおかしい
    - バックエンドに一つ、フロントに一つ用意する
    - 親はあった方がいいのか分からない
        - 多分ない方が良さそう
- nodejsで環境変数を扱うには、process.env.環境変数名で呼び出す
    - https://maku77.github.io/nodejs/env/environment-variable.html

