# はじめてのGitHub

# はじめに
GitHubはソースコードのバージョンをWeb上で管理することができるため，チームで共同でプログラムを作ることができます．また，ソースコードを配布することもできます．

# 始め方
## GitHub登録
  - https://github.com/
    - 学生の場合
      - http://blog.falconsrv.net/articles/471

## 使用するアプリケーション
  - Windowsの場合
    - Git Bashをダウンロード
      - https://git-for-windows.github.io/

  - Mac OSの場合
    - ターミナルを使用

# リポジトリの作り方
  1. Repositoriesを選択
  2. New
  3. Repository nameを登録
  4. Public or Privateを選択
  5. Create repository

# ローカル環境での管理
任意のフォルダで以下を入力

    cd (folder_name/)
    git init
    touch README.md
    git add --all
    git commit -m "initial commit"

# リポジトリにアップロード
GitHubにアップロード

    git remote add origin https://github.com/(username)/(repogitory_name).git
    git push origin master
