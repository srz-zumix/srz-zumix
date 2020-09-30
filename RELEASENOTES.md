# 自分リリースノート (Myself Release Notes)

## 0.34.6.9 (2020/09)

### iutest 関連

* `[[likely]]` `[[unlikely]]` 属性に対応しました [PR](https://github.com/srz-zumix/iutest/pull/503)
* Visual Studio における例外なしビルドのテストの追加と不具合を修正しました [PR](https://github.com/srz-zumix/iutest/pull/502)
* clang でオーバーロードされた private 関数にアクセスできない問題に対応しました [PR](https://github.com/srz-zumix/iutest/pull/501)
* zapcc でもコンパイルエラーを期待するテストをするようにしました [PR](https://github.com/srz-zumix/iutest/pull/509)
* Optional Matcher を追加 [PR](https://github.com/srz-zumix/iutest/pull/508)

### OSS 関連

* [wandbox-api][]
  * アクティブに更新してるのでリリースごとにまとめました
  * [v0.9.15](https://github.com/srz-zumix/wandbox-api/releases/tag/v0.9.15)
    * Java,Swift に対応
  * [v0.9.14](https://github.com/srz-zumix/wandbox-api/releases/tag/v0.9.14)
    * Bash,Elixir に対応
    * Elixir の mix 解釈に対応。ただし Wandbox 側での実行時に失敗するので実行はできない
* [awesome-cpp-warning][]
  * C++ の警告対応表を作り始めました
* [cpprefjp][]
  * [[[likely]][[unlikely]] の実装状況を更新 by srz-zumix · Pull Request #805 · cpprefjp/site](https://github.com/cpprefjp/site/pull/805)

### CI 関連

* [AzurePipelines][] で iutest に Visual Studio を使ったビルドとテストを追加しました [PR](https://github.com/srz-zumix/iutest/pull/502)
* このリリースノートの CI サービスに [Sider][] を導入しました
* Wercker で `Error provisioning Remote Docker Daemon from Remote Docker Daemon API service at rdd.default.svc.cluster.local:8888 for runID ...` で失敗する問題を調査中  

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2020/09/)
  * [[AppVeyor] fatal: reference is not a tree が出る場合の対応](https://srz-zumix.blogspot.com/2020/09/appveyor-fatal-reference-is-not-tree.html)
  * [[Re:VIEW Starter][Re:VIEW] 訳あって Starter から素の Re:VIEW に戻すツールをリリースしました](https://srz-zumix.blogspot.com/2020/09/review-starterreview-starter-review.html)
  * [GitHub Sponsor のバッジを付ける方法](https://srz-zumix.blogspot.com/2020/09/github-sponsor.html)
  * [[C++] 警告のコンパイラー対応表を作り始めました](https://srz-zumix.blogspot.com/2020/09/c.html)
  * [Zenn とブログズミ](https://srz-zumix.blogspot.com/2020/09/zenn.html)
* 執筆
  * [無料で始める！CIサービスカタログ](https://nextpublishing.jp/book/12228.html)
* [Zenn][]
  * [Zenn][] での執筆を始めました
  * [CI サービスを活用して Zenn の執筆環境を作る - 序章 | Zenn](https://zenn.dev/srz_zumix/articles/9404b45e22cdf0f65ddd)
  * [[C++] GCC/Clang/VisualStudio の警告をまとめているので紹介 | Zenn](https://zenn.dev/srz_zumix/articles/4c72e544b0034cc796da)
  * [[textlint] Zenn 独自記法への警告を除外する | Zenn](https://zenn.dev/srz_zumix/articles/cb21af1a86fc01cb829d)
  * [[C++] override すべき関数の名前 typo に気づける idiom | Zenn](https://zenn.dev/srz_zumix/articles/ae351b73da285447fdc0)

### 仕事

* [CEDEC2020](https://cedec.cesa.or.jp/2020/) に参加しました
* リモートワーク環境が完成した


## 0.34.5.8 (2020/08)

### iutest 関連

* [zapcc][] でのテストを GitHub Actions に追加しました [PR](https://github.com/srz-zumix/iutest/pull/493)
* [GoogleTest][] が将来的に TestCase が TestSuite に変わる点に対応しました（[iutest][] は TestCase を廃止せず両方サポートします）
* static_assert やコンパイルエラーが発生することを期待するテスト用の pyton プログラムを修正中 [PR](https://github.com/srz-zumix/iutest/pull/496)

### CI 関連

* [ci-normalize-envvars][] にブランチ情報を追加しました
  * ci-normalize-envvars は各CIサービスで定義される環境変数を透過的に使うためのシェルスクリプトです
* [Crowdin](https://crowdin.com/) を使ってみてました
  * 翻訳をするためのサービスであって、翻訳をしてくれるサービスではないのかな？（後者も期待してた）

### OSS 関連

* [GoogleTest][]
  * GTEST_REMOVE_LEGACY_TEST_CASEAPI_ を define したときのビルド・テスト失敗修正 PR
    * https://github.com/google/googletest/pull/2972
    * https://github.com/google/googletest/pull/2979
* [wandbox-api][]
  * wandbox-python で setup.py を認識できるようにしました [PR](https://github.com/srz-zumix/wandbox-api/pull/9)
  * wandbox-CPP（Cプリプロセッサ）と wandbox-cc（C言語）を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/11)
  * wandbox-ruby,wandbox-mruby を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/12)
  * wandbox-go を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/13)
  * wandbox-ssl を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/14)
  * wandbox-js を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/15)
  * wandbox-tsc を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/16)
  * wandbox-perl を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/17)
  * wandbox-nim を追加しました [PR](https://github.com/srz-zumix/wandbox-api/pull/18)
  * 一部のオプションが評価されていなかった不具合を修正しました [PR](https://github.com/srz-zumix/wandbox-api/pull/11)
* [JetBrains All Products Pack](https://www.jetbrains.com/ja-jp/community/opensource/#support) の OSS ライセンスを取得しました

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2020/08/)
  * [[GitHub Actions] Actions の PR 時に自分自身をアクションとして実行する](https://srz-zumix.blogspot.com/2020/08/github-actions-actions-pr.html)
  * [[iutest] ドキュメントの置き場を GitHub Pages に集約した](https://srz-zumix.blogspot.com/2020/08/iutest-github-pages.html)
  * [[Doxygen] @page の名前には小文字を使おう](https://srz-zumix.blogspot.com/2020/08/doxygen-page.html)
  * [[技術書典] Re:VIEW Starter でクローバー「♣」を別の文字に変更する](https://srz-zumix.blogspot.com/2020/03/wip-review-starter.html)
  * [wandbox-api の CLI に C/CPP/Go/JavaScript/Nim/OpenSSL/Perl/Python/Ruby/TypeScript を追加しました](https://srz-zumix.blogspot.com/2020/08/wandbox-api-cli-ccppgojavascriptnimopen.html)

### 仕事

* 約半年ぶりに出社した

### その他

* [CalorieMate to Programmer CUIモード](https://t.co/77LHLWVXel?amp=1) が面白かったです
* 準同型暗号について調べたりしてます
* [NEW GAME! 11巻](https://amzn.to/3hW0vYV)購入。癒やされる

## 0.34.4.7 (2020/07)

### iutest 関連

* [iutest 1.17.1](https://github.com/srz-zumix/iutest/releases/tag/v1.17.1) をリリースしました
* NE_RANGE/NE_COLLECTIONS アサーションを追加しました
* [Wandbox][] の API 制限開始に伴い iutest.min.wandbox.hpp の圧縮を強化しました [PR485](https://github.com/srz-zumix/iutest/pull/485)
* [Wandbox での make ビルド](https://github.com/srz-zumix/iutest/pull/491) に対応しました（v1.17.1 には含みません）
* [GoogleTest][] の TestCase -> TestSuite 移行への対応を開始しました


### CI 関連

* [LGTM.com][] を使ってみました
* [Appcircle][] を使ってみたいリストに登録しました
* [Twitter の CI/CD リスト](https://twitter.com/i/lists/1037699078723854336)を更新しました （+Appcircle）
* iutest
  * [AzurePipelines][] でパスフィルターを設定
  * [RazorOps][] のトライアルが終わったためか [CentOS 5 + gcc 3.4.6 な Docker image](https://hub.docker.com/repository/docker/srzzumix/gcc3) での CI ができなくなっていたので別 CI サービス ([Drone.io][]) に移動しました
  * [Wandbox][] に依存していたコンパイラマトリックス検証を [Wercker][]/[Shippable][] から [Drone.io][] に引っ越しました  
Wandbox を使わず gcc/clang の Docker image を使って検証しています
  * [Bitrise][] のワークフローをリポジトリの yaml を実行するようにしたことで fork された PR が失敗するようになっていたのを修正 [PR476](https://github.com/srz-zumix/iutest/pull/476)
  * どの OS でなんのコンパイラのどのバージョンで C++ バージョンは何を指定してテストしたかの集計を始めました
* [ci-specs][]
  * [ci-trigger][]
    * ブランチフィルターの調査中
  * [ci-normalize-envvars][]
    * 各種 CI サービスの環境変数の正規化を行うシェルファイルの開発を始めました
    * サービス名とコミットハッシュに対応済み
    * 現在ブランチ・タグに対応中

### OSS 関連

* [wandbox-api v0.9.6](https://github.com/srz-zumix/wandbox-api/releases/tag/v0.9.6) をリリースしました
  * [Wandbox API][] の CLI ツール [wandbox-api][] です
    * api ラッパーの他に、 c++ 用に include ファイルの自動追加や c++ 向けの wandbox オプションに対応した wandbox-cxx コマンドが使用できます
  * v0.9.6 では python 用のコマンドを追加しました
    * import に対応し自動で関連ファイルをファイルリストに追加します
* [zapcc][] の docker コンテナを作りました https://github.com/srz-zumix/docker-zapcc
* 7月以前ですが・・
  * コードメトリクスツール [Lizard][] を Docker コンテナ化した[docker-lizard](https://github.com/srz-zumix/docker-lizard) を公開

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2020/07/)
  * [[Travis CI] Segmentation fault したときにスタックトレースを出力する設定](https://srz-zumix.blogspot.com/2019/10/wiptravis-ci-segmentation-fault.html)
  * [[CI][CodeReview] LGTM.com 始めました](https://srz-zumix.blogspot.com/2020/06/cicodereview-lgtmcom.html)
  * [[技術書] 画像のフォーマットチェックを GitHub Actions でしてみた](https://srz-zumix.blogspot.com/2020/07/github-actions.html)
  * [iutest v1.17.1 をリリースしました](https://srz-zumix.blogspot.com/2020/07/iutest-v1171.html)
  * Blogger の公開日設定がいまいち使いこなせてなくておかしくなっていたのを修正しました（公開日ではなく最終更新日になってる？）
* 執筆
  * 新しい本の調整をしてました

### 仕事

* 3月からずっと自宅で仕事してます

### その他

* GitHub のプロフィールをリポジトリ化できるようになっていたので、やろうと思ってできてなかった自分リリースノートを開始しました
* StrongTypedef を使いたいなと思いつつもできてない。
  * ところで [C++ 不透明エイリアス(opaque alias) ってどうなったんだろ？ - ずみっくす@あつまれCIサービス (@srz_zumix)](https://twitter.com/srz_zumix/status/1283669007871033344)
  * [本の虫: C++1yに提案されている不透明エイリアス(opaque alias)](https://cpplover.blogspot.com/2013/09/c1yopaque-alias.html)
* システムヘッダーの警告を有効にして遊んでました [https://github.com/srz-zumix/iutest/pull/465](https://github.com/srz-zumix/iutest/pull/465)
  * システムヘッダーってテストされてて警告はなにもないと思いこんでいましたが、全然そんなことなかった・・

[Appcircle]:https://appcircle.io/
[AzurePipelines]:https://azure.microsoft.com/ja-jp/services/devops/pipelines/
[awesome-cpp-warning]:https://github.com/srz-zumix/awesome-cpp-warning
[Bitrise]:https://www.bitrise.io/
[ci-normalize-envvars]:https://github.com/srz-zumix/ci-normalize-envvars
[ci-specs]:https://github.com/srz-zumix/ci-specs
[ci-trigger]:https://github.com/srz-zumix/ci-trigger
[cpprefjp]:https://cpprefjp.github.io/
[Drone.io]:https://drone.io/
[GoogleTest]:https://github.com/google/googletest
[iutest]:https://github.com/srz-zumix/iutest
[LGTM.com]:https://lgtm.com/
[Lizard]:https://github.com/terryyin/lizard
[RazorOps]:http://razorops.com/
[Shippable]:https://app.shippable.com/
[Sider]:https://sider.review/
[Wandbox]:https://wandbox.org/
[Wandbox API]:https://github.com/melpon/wandbox/blob/master/kennel2/API.rst
[wandbox-api]:https://github.com/srz-zumix/wandbox-api
[Wercker]:https://app.wercker.com/
[zapcc]:https://github.com/yrnkrn/zapcc
[Zenn]:https://zenn.dev/srz_zumix
