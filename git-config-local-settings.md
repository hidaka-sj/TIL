# Gitで複数アカウントを使い分ける際の `git config --local` の設定方法

## 学んだ内容
複数の GitHub アカウントを使い分けている環境で、特定のリポジトリ（例: 学習用の TIL リポジトリ）だけは常に個人用のアカウントでコミット・プッシュできるように設定する方法を学んだ。

## 発生したエラー
リポジトリのローカル設定を行う際、以下のようにコマンドを誤入力してエラーが発生した。

```bash
$ git config local user.name "Your Name"
error: key does not contain a section: local

## 解消方法
-- の付け忘れだったため、正しく--localを利用する