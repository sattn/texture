---
layout: post
title:  "QWIKLABSのGCP基礎コースをやってみた"
date:   2019-01-06
---

[GCP基礎コース](https://www.qwiklabs.com/quests/23)は合計８つのクエストで完了見込みは５時間１５分となっていますが、２時間くらいで全クエスト完了。内容が簡潔にまとめられているのでサクサク進みます。[QWIKLABS を使って GCP を学ぼう](https://developers-jp.googleblog.com/2018/12/japan-cloud-study-jams-trial-event.html)で無料のクーポンコードをゲットしたので、料金を気にせず試すことができたのが良かった。「さわり」を学ぶには、とてもいい教材だと思います。

### 受講内容
1. Qwiklabs と Google Cloud Platform の概要
Google Cloud PlatformのメニューとCloud Shellの説明。ハンズオンというかハンズオフな内容でした。
1. 仮想マシンの作成
実際にVM インスタンスを作成して、nginxのアクセス確認をするところまで行います。Cloud Shellでのインスタンス作成はコマンド文がやや長いけれど便利。
1. Compute Engine: Qwik Start - Windows
Windowsサーバを使うことは無いのでスキップしました。
1. Cloud Shell と gcloud のスタートガイド
gsutilツールを使ってCloud Storageバケットにバックアップします。gsutilというのがあるんだよ、ぐらい覚えておけば良い気がする。
1. GCP Marketplace を使用したサービスのプロビジョニング
Nginx スタックがデプロイされているVM インスタンスを作成する。便利そうですが、実務ではMarketplaceを使う機会は無いかなぁ、と思います。AnsibleやDockerを使いますし。
1. 永続ディスクの作成
VM インスタンスに対して永続ディスクをマウントします。スナップショット（コピーディスク）の作成方法までやってみたかった。
1. Hello Node Kubernetes
k8sでクラスタとポッドを作成してWebサーバを公開します。残念ながらKubernetes ダッシュボードが表示されませんでした。手順間違ったのかな・・・。k8sの予備知識がないとチンプンカンプンな内容になると思います。
1. Stackdriver: Qwik Start
VM インスタンスのヘルスチェックでインシデント通知を確認するところまで行います。GCPでサービス構築するなら確実に使いますね。
1. ネットワーク ロードバランサと HTTP ロードバランサを構成する
L3,L7のロードバランサの作成を行います。HTTP(s) ロードバランサのSSL証明書設定方法も知りたかった。
