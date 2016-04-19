# はじめてのGitHub

# はじめに
GitHubはソースコードのバージョンをWeb上で管理することができるため，チームで共同でプログラムを作ることができます．また，ソースコードを配布することもできます．

# 始め方
## GitHub登録
  - https://github.com/
    - 学生の場合
      - http://blog.falconsrv.net/articles/471

## 使用するアプリケーション
  - GitHubとのやり取り
    - Windowsの場合
      - Git Bashをダウンロード
        - https://git-for-windows.github.io/

    - Mac OSの場合
      - ターミナルを使用

  - Markdown Editor
    - atom
      - https://atom.io/

# リポジトリの作り方
  1. Repositoriesを選択
  2. New
  3. Repository nameを登録
  4. Public or Privateを選択
  5. Create repository

# ローカル環境での管理
任意のフォルダで以下を入力

    $ cd (folder_name/)
    $ git init
    $ touch README.md
    $ touch .gitignore
    $ git add --all
    $ git commit -m "initial commit"

# リポジトリにアップロード
GitHubにアップロード

    $ git remote add origin https://github.com/(username)/(repogitory_name).git
    $ git push origin master

# その他
## Markdownについて
Markdown方式に慣れよう
  - サンプル
    - https://github.com/iwanao731/Test

## プロキシの設定
大学にいる間はプロキシの設定が必要かもしれないです．以下の情報を打ち込んでください．

    $ git config --global http.proxy www-proxy.waseda.jp:8080
    $ git config --global https.proxy www-proxy.waseda.jp:8080

家で使う用に設定を戻す時は以下

    $ git config --global --unset http.proxy
    $ git config --global --unset https.proxy
## 特定ファイルの除去(.gitignoreを使う)
.exeや.objといったファイルなどアップロードする必要のない場合は，.gitignoreファイルを生成して，中身を逐次書き加えていく．

1. gitignoreの自動生成ツールを使用
  - [gitignore.io](https://www.gitignore.io/)
2. 統合開発環境を検索(Visual Studio or openFrameworks等)
3. .gitignoreに内容をコピー/ペースト

## openFrameworksのaddon
openFrameworks addons (ofxaddons)
  - http://ofxaddons.com/categories


