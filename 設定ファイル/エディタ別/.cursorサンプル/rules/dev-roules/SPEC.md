# システム仕様書

## システム概要

本システムは、xxxxxxシステムです。

## ドキュメント

- 技術スタック: Gemfile
- データベース設計: db/schema.rb


## シナリオ

### ユーザー登録シナリオ

#### 新規登録画面へのアクセス
- ログイン画面から「こちら」リンクをクリックして遷移
- ログイン中はトップページにリダイレクト


## バッチ一覧

```
crontab -l
00 9,11,13,15,17 * * * /bin/bash -l -c 'cd /var/www/short_url/git/short_url && bin/rails runner -e production Hoge.new.run 2>> log/crontab.log 1>/dev/null'
```