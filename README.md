# SQL 学習用

このリポジトリは、MySQL と phpMyAdmin を使用した SQL 学習用の環境です。  
Docker Compose を使用して、簡単にセットアップできます。

## 前提条件

- Docker がインストールされていること

## セットアップ手順

1. このリポジトリをクローンします。

```bash
  git clone https://github.com/yourusername/sql-study.git
```

2. リポジトリのディレクトリに移動します。

```bash
  cd sql-study
```

3. Docker Compose を使用して、コンテナを起動します。

```bash
  docker compose up -d
```

4. MySQL と phpMyAdmin が起動したら、以下の URL から phpMyAdmin にアクセスできます。  
   http://localhost:3307

- ユーザー名: root
- パスワード: password

## DBeaver 設定方法

DBeaver を使用して MySQL に接続する場合は、以下の設定を使用してください。

- JDBC URL: jdbc:mysql://127.0.0.1:3306?protocol=tcp
- ユーザー名: root
- パスワード: password

## 注意事項

- このセットアップは学習用途を目的としており、本番環境では使用しないでください。
- データベースのデータは mysql_data ディレクトリに保存されます。  
  コンテナを削除する際は、このディレクトリを削除しないように注意してください。
