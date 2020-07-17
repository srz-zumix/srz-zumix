# 自分リリースノート (Myself Release Notes)

## 0.34.4.7 (2020/07)

### iutest 関連

* NE_RANGE/NE_COLLECTIONS アサーションを追加しました
* [Wandbox](https://wandbox.org/) の API 制限開始に伴い iutest.min.wandbox.hpp の圧縮を強化しました [PR485](https://github.com/srz-zumix/iutest/pull/485)


### CI 関連

* [LGTM.com](https://lgtm.com/) を使ってみました
* [Appcircle](https://appcircle.io/) を使ってみたいリストに登録しました
* [Twitter の CI/CD リスト](https://twitter.com/i/lists/1037699078723854336)を更新しました （+Appcircle）
* iutest
  * [AzurePipelines](https://azure.microsoft.com/ja-jp/services/devops/pipelines/) でパスフィルターを設定
  * [RazorOps](http://razorops.com/) のトライアルが終わったためか [CentOS 5 + gcc 3.4.6 な Docker image]() での CI ができなくなっていたので別 CI サービス ([Drone.io](https://drone.io/)) に移動しました
  * [Wandbox](https://wandbox.org/) に依存していたコンパイラマトリックス検証を [Wercker](https://app.wercker.com/)/[Shippable](https://app.shippable.com/) から [Drone.io](https://drone.io/) に引っ越しました  
Wandbox を使わず gcc/clang の Docker image を使って検証しています
  * [Bitrise](https://www.bitrise.io/) のワークフローをリポジトリの yaml を実行するようにしたことで fork された PR が失敗するようになっていたのを修正 [PR476](https://github.com/srz-zumix/iutest/pull/476)
  * どの OS でなんのコンパイラのどのバージョンで C++ バージョンは何を指定してテストしたかの集計を始めました
* [ci-specs](https://github.com/srz-zumix/ci-specs)
  * [ci-trigger](https://github.com/srz-zumix/ci-trigger)
    * ブランチフィルターの調査中

### OSS 関連

* 7月以前ですが・・
  * コードメトリクスツール [Lizard](https://github.com/terryyin/lizard) を Docker コンテナ化した[docker-lizard](https://github.com/srz-zumix/docker-lizard) を公開
  * [Wandbox API](https://github.com/melpon/wandbox/blob/master/kennel2/API.rst) の CLI ツール [wandbox-api](https://github.com/srz-zumix/wandbox-api) を公開

### ブログ

* [ブログズミ](https://srz-zumix.blogspot.com/2020/07/)
  * [[Travis CI] Segmentation fault したときにスタックトレースを出力する設定](https://srz-zumix.blogspot.com/2019/10/wiptravis-ci-segmentation-fault.html)
  * [[CI][CodeReview] LGTM.com 始めました](https://srz-zumix.blogspot.com/2020/06/cicodereview-lgtmcom.html)

### 仕事

* 3月からずっと自宅で仕事してます

### その他

* GitHub のプロフィールをリポジトリ化できるようになっていたので、やろうと思ってできてなかった自分リリースノートを開始しました
* StrongTypedef を使いたいなと思いつつもできてない。
  * ところで [C++ 不透明エイリアス(opaque alias) ってどうなったんだろ？ - ずみっくす@あつまれCIサービス (@srz_zumix)](https://twitter.com/srz_zumix/status/1283669007871033344)
  * [本の虫: C++1yに提案されている不透明エイリアス(opaque alias)](https://cpplover.blogspot.com/2013/09/c1yopaque-alias.html)
* システムヘッダーの警告を有効にして遊んでました [https://github.com/srz-zumix/iutest/pull/465](https://github.com/srz-zumix/iutest/pull/465)
