# 開発に使用する言語・ツールのセットアップ

## ツール類のインストール

    sudo aptitude install bundler

だけでいいはず(多分

## Github

リポジトリは https://github.com/it-college-aprilfool/site です。

### 最初にやる作業

    cd 自分の作業用ディクレトリ
    git clone https://github.com/it-college-aprilfool/site.git
    cd site
    bundle exec middleman server

上手く動いたら、ブラウザで http://localhost:4567 にアクセスする。 

初回実行時のみ、めっちゃ時間かかるかも…
