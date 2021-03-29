# twcu-online.github.io

このページの内容は，以下のサイトに移転しました．

https://sites.google.com/cis.twcu.ac.jp/cisqa/distance-lecture-student?authuser=0  
https://sites.google.com/cis.twcu.ac.jp/cisqa/distance-lecture-teacher?authuser=0

<br />
<br />
<hr>
以下は古い情報です．

https://twcu-online.github.io/
<br />
<br />

## サイトの構成

（今後，変更する可能性あり）

- トップページ：新入生用ページ  
- student配下：在学生用ページ  
- teacher配下：教員用ページ

## ページの更新方法

- git, GitHubの設定を行っていることが前提です．  
```
$ git clone https:....
$ cd twcu-online
$ git checkout -b 適当なブランチ名

編集作業を行う

$ git commit -m '編集した内容' -a
$ git push -u origin ブランチ名

GitHub上で pull request を作成する
```

- mergeは管理者が行います．merge後はローカルで以下を実行してください．
```
$ git checkout master
$ git pull
$ git branch -d ブランチ名
```
<br />

## その他の参考情報

### GitHubの設定・使い方

- [Getting started with GitHub](https://help.github.com/en/github/getting-started-with-github)  
- [SSHによるGitHubへのアクセス](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)  
- [pull requestの作成](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests)

### 利用しているテーマ（Slate）のデモページ

- [Slateデモページ](https://pages-themes.github.io/slate/)  
- [Slateのソースコード](https://github.com/pages-themes/slate)

### localでページの見た目を確認するための手順

- 環境により異なると思いますのでその都度調べてください．以下はmacOS Catalinaの場合です．  
- 最初にやっておくこと．  
```
command line toolsのインストール

$ cd twcu-online.github.io
$ gem install bundler
$ bundle init
$ vim Gemfile (他のテキストエディアでも可)
Gemfileを開いて，一番下に以下の行を追記する
gem "github-pages", group: :jekyll_plugins

$ bundle install
```

- 以下を実行するとローカルでサーバが立ち上がるので，ブラウザでhttp://localhost:4000/ にアクセスする．  
```
$ cd twcu-online.github.io
$ bundle exec jekyll serve
```
<br />

ご質問，ご要望は遠隔授業プロジェクトチームまでお願いします．
