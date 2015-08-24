# Gitの使い方

## Gitとは

Gitは分散型バージョン管理システムの一つです。

# Git体験ツアー

## はじめてのコミット

### Gitリポジトリの作成

任意のディレクトリに移動します。

    $ cd xxx

カレントディレクトリにGitリポジトリを作成します。

    $ git init

> git initコマンドによって、.gitディレクトリが作成されます。もし、Gitリポジトリを破棄したい場合は.gitディレクトリを削除すれば良いでしょう。

### ステージング

まずはバージョン管理対象となるファイルを作成しましょう。

    $ echo Hello > README.md

作成したファイルをステージングします。

    $ git add README.md

> ステージングとはコミット対象のファイルを確定することです。

### コミット

ローカルリポジトリに更新を確定（コミット）する。

    $ git commit -m "add Hello.txt"

> コミット時にはコミットメッセージが必須です。-mオプションでコミットメッセージを指定します。

### ログの確認

ログを見てみましょう。

    $ git log
    commit 60f8a67bcc4fc6a766684546470acb6052271dee
    Author: murayama <murayama333@gmail.com>
    Date:   Mon Aug 24 15:14:53 2015 +0900

        add Hello.txt
