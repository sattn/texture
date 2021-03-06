---
layout: post
title:  "この１冊でDocker/Kubenetesをキャッチアップ！【Docker/Kubernetes実践コンテナ開発入門】"
date:   2018-11-22
---

本番環境での重要なポイントであるホストマシンのセキュリティアップデートやクレデンシャルの扱い、アプリケーションのロギング管理、障害発生時の対策などが具体的に詰め込まれており、実務で活用できるレベルの内容。体型的にDocker/Kurbenetesを学べる。

[![Docker/Kubernetes実践コンテナ開発入門](http://image.gihyo.co.jp/assets/images/cover/2018/thumb/TH160_9784297100339.jpg)](https://gihyo.jp/book/2018/978-4-297-10033-9)

### 概要
* Dockerの基礎
  * Dockerの基礎概念であるコンテナ型仮想化技術とは
  * XenやKVMといったホスト型仮想化との違い
  * 環境差異問題やアプリケーションの構成管理のしやすさ
  * ローカル環境の構築方法
* Dockerコンテナのデプロイ
  * Dockerイメージの作成方法から操作方法
* 実用的なコンテナの構築とデプロイ
  * １コンテナ＝１プロセス？コンテナの粒度について考察
  * 永続化データの扱いやコンテナの配置方法
* Swarmによる実践的なアプリケーション構築
  * アプリケーションを構成するNginx、API Service、MySQLといった要素をSwarm上で構築する方法
* Kubernetes入門
  * Kubernetesの位置づけと基本的な概念、コンテナシステムを構成するリソース群
* Kubernetesのデプロイ・クラスタ構築
  * GKE（Google Kubernetes Engine）のセットアップ
  * GKE上にアプリケーションを構築
* Kubernetesの発展的な利用
  * 常駐のWebアプリケーション以外にもJob（バッチ処理）としての使い方
  * ユーザと権限の設定
* コンテナの運用
  * ロギング管理（Fluentd、Elasticsearch、kibanaを利用した可視化も併せて）
  * 障害対策
* より軽量なDockerイメージを作る
  * scratch, BusyBox, Alpine Linux
  * ビルドと実行用でコンテナを分ける
* Dockerの様々な活用方法
  * 開発環境を共有する
  * 負荷テストで利用する

### 本書で得られたポイント
* アプリケーションのプロパティ値は、環境変数で管理しましょう
* DockerHubにはセキュリティ的に怪しいイメージもあるので公式イメージの利用を推奨
* コンテナ内のアプリケーション実行ユーザは別に用意すること（デフォルトはrootユーザ）
* マイクロサービス化による懸念材料となるサービス間のルーティング管理、障害時のエラーハンドリングについては、Istio, Linkerdなどを利用すると良い
* 負荷テストはjmeterだけではない。シンプルなLocust（イナゴ）もある。
