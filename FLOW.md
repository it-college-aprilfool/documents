# 作業の進め方

## 更新作業を行なう時に

最新版のソースコードを取得します。

    git checkout master
    git pull origin master

必ずcheckout -b (作業の名前)を行なってから作業しましょう。
今回は作業の名前をfix-titleにしています。

    git checkout -b fix-title

編集したところがきちんと動いているかブラウザで確認を行なってください。

作業が終ったら動作確認をして、gitにadd/commit/pushします。

    git add -A
    git commit -m '変更箇所を伝えるメッセージ'
    git push origin fix-title

上記コマンドは作業が完了するまで何回やってもかまいません。

作業が完了し、内容を反映してほしい場合はGithubのサイトからPull Requestを投げてください。

## サーバーへの反映

リーダーはPR(Pull Request)を確認し、問題なければmergeしてください。

mergeされると自動的にS3へアップロードされます。

## その他

githubへのpushやマージ後のデプロイ(サーバーへの反映)はSlackの#notifyに通知が行きます。
