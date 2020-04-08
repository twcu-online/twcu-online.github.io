# twcu-online.github.io

https://twcu-online.github.io/
<br />
<br />

### 更新の仕方

- gitはすでに設定済み，$ git cloneを行っていることを前提にします．  
- branchを切ったりしない非推奨の方法ですが，更新の容易さを優先しています．  
- Conflictが発生する可能性があります．

```
$ cd twcu-online.github.io
$ git pull

ファイルを更新

$ git add .
$ git commit -m '何を変更したかを記述'
$ git push -u origin master
```
<br />
<br />

## サイトの構成

今後変わる可能性がありますが，現状は以下のとおりです．

- トップページ：新入生用ページ  
- student配下：在学生用ページ  
- teacher配下：教員用ページ

## その他参考

### Githubの設定

- [Getting started with GitHub](https://help.github.com/en/github/getting-started-with-github){:target="_blank"}  
- [SSHによるGitHubへのアクセス](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh){:target="_blank"}

### 利用しているテーマ（Slate）のデモページ

- [Slateデモページ](https://pages-themes.github.io/slate/){:target="_blank"}  
- [Slateのソースコード](https://github.com/pages-themes/slate){:target="_blank"}

### localでの確認のための手順

- 環境により異なると思いますので，その都度調べてください．
以下はMac Catalinaの場合．

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

- 確認するときは，以下を実行するとローカルでサーバが立ち上がります．ブラウザでhttp://localhost:4000/ にアクセスすると確認できます．

```
$ cd twcu-online.github.io
$ bundle exec jekyll serve
```

ご質問，ご要望は遠隔授業プロジェクトまでお願いします．