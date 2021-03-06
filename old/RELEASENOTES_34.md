# 自分リリースノート (Myself Release Notes)

## 0.34.11.2 (2021/02)

### iutest 関連

* C++20 対応を開始 https://github.com/srz-zumix/iutest/pull/565
* DockerHub pull rate limit 対応 ([Wercker][]) https://github.com/srz-zumix/iutest/pull/566 

### CI 関連

* [ci-trigger][]
  * [AppVeyor][]/[Azure Pipelines][] 更新
* [ci-skip][]
  * [GitHub Actions][] が skip comment 対応してたので更新

### OSS 関連

* [awesome-cpp-warning][]
  * -Wnull-arithmetic, -Wambiguous-reversed-operator を追加 
* [wandbox-builder][] にいくつか修正 PR をしました
* [wandbox-api][]
  * erlang,haskell,php に対応しました
  * リストアップ系サブコマンドが動作していなかった不具合を修正しました
  * template,run-template サブコマンドを追加
  * コンパイラーバージョンの指定に fnmatch が指定可能にしました
* [review-retrovert][]
  * IRD 組版エミュレートスタイルを追加（Experimental）

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/02/)
  * [古い gcc が欲しくて CentOS 5 の docker image を作った話](https://srz-zumix.blogspot.com/2021/02/gcc-centos-5-docker-image.html)
  * [\[CodeShip\]\[Drone.io\] DockerHub pull rate limit に対応する](https://srz-zumix.blogspot.com/2021/02/codeshipdroneio-dockerhub-pull-rate.html)
  * [Wekan サーバーの引っ越しで mongoDB のバックアップ・リストアした（docker-compose 編）](https://srz-zumix.blogspot.com/2021/02/wekan-mongodb-docker-compose.html)
  * [cppcheck html report](https://srz-zumix.blogspot.com/2021/02/cppcheck-html-report.html)


## 0.34.10.1 (2021/01)

### iutest 関連

 * Google Test 互換性対応の issue 片付け中 https://github.com/srz-zumix/iutest/labels/compatibility
   * Google Test 互換性テストで xml 出力しようとするとクラッシュする問題を修正 https://github.com/srz-zumix/iutest/pull/563
 * final おじさん https://github.com/srz-zumix/iutest/pull/559
   * [［C++］final指定子と最適化 - 地面を見下ろす少年の足蹴にされる私](https://onihusube.hatenablog.com/entry/2018/11/23/022618)
 * ::std::filesyste::file_stats の operator == は C++20 以降 https://github.com/srz-zumix/iutest/pull/556
 * GitHub Actions でイメージ指定する場合の docker login 対応 https://github.com/srz-zumix/iutest/pull/557

### CI 関連

 * [Travis CI のクレジット枯渇](https://blog.travis-ci.com/2020-11-02-travis-ci-new-billing)に対応中
 * [Appcircle][] お試し中
   * Appcircle の xcode build のポスト処理で失敗してるのの解決に時間かかってる（一旦自前でビルドにするかも）
   * [ci-specs][]/[ci-normalize-envvars][] に追記
 * [AppVeyor][] でテスト結果の集計対応中 https://github.com/srz-zumix/iutest/issues/239

### OSS 関連

 * Go 言語で Google カレンダーの操作をするコードを書いてました https://github.com/srz-zumix/go963
   * 書いたはいいけど別手法のものを採用することにしたので、これ以上いじることはない見込み
 * [Re:VIEW Starter][] -> [Re:VIEW][] ツール [review-retrovert][] の更新
 * Re:VIEW (Starter) の画像ファイルのフォーマットチェック用 GitHub Actions [actions-book-image-check][] 更新
 
### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/01/)
  * [【技術書典10】「あつまれ CI サービス 2020冬」の販売を開始しました](https://srz-zumix.blogspot.com/2021/01/10-ci-2020.html)
  * [\[Re:VIEW\] mapfile 中の table が正しく表示されない場合の対応方法](https://srz-zumix.blogspot.com/2020/12/review-mapfile-table.html)
  * [\[review-retrovert\] Re:VIEW Starter → Re:VIEW 4/5 に対応しました](https://srz-zumix.blogspot.com/2021/01/review-retrovert-review-starter-review.html)
* [技術書典10][]
  * [詳解 Integromat iPaaS 完全入門][] 販売
  * [あつまれ CI サービス 2020冬][] 販売
  * [Booth 虎空棘魚][] での販売開始

### 仕事

* ansible やったり terraform やったり
* JCasC やったり JobDSL やったり

### その他

 * findy やってみた
   * Python の偏差値が C++ の偏差値超えてて、そんなもんかと思った
   * Javascript とか書いてる記憶がないんだけどな
   * https://twitter.com/srz_zumix/status/1355149364939767811

## 0.34.9.12 (2020/12)

### iutest 関連

* wine 上の msvc でのテストを追加 https://github.com/srz-zumix/iutest/pull/545
* DockerHub の pull 制限に対応中 https://github.com/srz-zumix/iutest/issues/519
  * Drone の対応が不完全だったのを修正 https://github.com/srz-zumix/iutest/pull/550
* RazorOps v2 に移行 https://github.com/srz-zumix/iutest/pull/541
  * Thanks dsyoi https://github.com/srz-zumix/iutest/pull/546

### CI 関連

* [Travis CI のプラン変更](https://blog.travis-ci.com/2020-11-02-travis-ci-new-billing)に対応中
  * とりあえず 50,000 クレジットもらった
  * OSS クレジットはまだ
  * 公式にリツイートされたら・・  
    https://twitter.com/srz_zumix/status/1334360672549761024
    https://www.reddit.com/r/programming/comments/k8v6u2/travis_ci_is_no_longer_providing_ci_minutes_for/
  * 信じて待つのみ・・
* [Appcircle][] お試し中
  * なぜか一ヶ月経っても制限解除されなかったのでお問い合わせして対応してもらった

### ブログ/執筆

* [C++ Advent Calendar 2020](https://qiita.com/advent-calendar/2020/cxx) に参加しました
* [ブログズミ](https://srz-zumix.blogspot.com/2020/12/)
  * [\[C++\] Concepts で外部ライブラリの template よりも優先されるオーバーロード関数を書く](https://srz-zumix.blogspot.com/2020/03/wipc-concept-template.html)
  * [Zapcc を使った複数プログラムの並列ビルドでハマった話](https://srz-zumix.blogspot.com/2020/12/zapcc.html)
  * [\[DockerHub\] AutomatedBuild でバージョンタグを自動でつける](https://srz-zumix.blogspot.com/2020/12/dockerhub-automatedbuild.html)
  * [\[C++\] Clang ではオーバーロードされた private 関数に明示的な実体化時のアクセスができない？](https://srz-zumix.blogspot.com/2020/12/c-clang-private.html)
  * [【技術書典10】「詳解 Integromat iPaaS 完全入門」の販売を開始しました](https://srz-zumix.blogspot.com/2020/12/10-integromat-ipaas.html)
* [技術書典10][]
  * [詳解 Integromat iPaaS 完全入門][] 販売

### 仕事

* Jenkins おじさんおじさん

### その他

* 英語わからん

## 0.34.8.11 (2020/11)

### iutest 関連

* Xcode 向けの CMake 設定を修正
* DockerHub の pull 制限に対応中 https://github.com/srz-zumix/iutest/issues/519
* RazorOps v2 に移行中 https://github.com/srz-zumix/iutest/pull/541

### CI 関連

* DockerHub の pull 制限に対応中 https://github.com/srz-zumix/iutest/issues/519
* [Appcircle][] お試し中（１ヶ月のビルド回数制限使い切ったので来月再開）
* [Travis CI のプラン変更](https://blog.travis-ci.com/2020-11-02-travis-ci-new-billing)に対応中
  * OSS クレジットを申請中

### OSS 関連

* [TampermonkeyUserScripts][]
  * [ページを iframe に分割するスクリプトを追加](https://github.com/srz-zumix/TampermonkeyUserScripts#iframe-splitter)

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2020/11/)
  * [Docker login しているか確かめる方法](https://srz-zumix.blogspot.com/2020/11/docker-login.html)
  * [Travis CI の新プランについて](https://srz-zumix.blogspot.com/2020/11/travis-ci.html)
  * [\[CI\] TeamCity Cloud OpenBeta を使ってみた](https://srz-zumix.blogspot.com/2020/11/ci-teamcity-cloud-openbeta.html)
  * [\[C++\] -Weverything で得たもの](https://srz-zumix.blogspot.com/2020/11/c-weverything.html)
* [技術書典10][] に参加申し込みしました https://twitter.com/srz_zumix/status/1332570611374116869

## 0.34.7.10 (2020/10)

### iutest 関連

* 例外発生時にも SCOPED_TRACE のメッセージを出力できるように修正 https://github.com/srz-zumix/iutest/pull/264
  * ただし、ユーザーがハンドリングした場合に対応してないので良い方法模索中
* Wandbox の API 制限を考慮し Wandbox 上で iutest を使うテストマトリックスを廃止  
上記に伴い iuwandbox を deprecated に変更  
ファイルサイズ削減 https://github.com/srz-zumix/iutest/pull/513
* より厳しい警告オプションを設定 https://github.com/srz-zumix/iutest/pull/517


### CI 関連

* TeamCity Cloud Open Beta を使い始めました
* DockerHub の pull 制限に対応中 https://github.com/srz-zumix/iutest/issues/519
* GitHub Actions の set-env コマンドは deprecated になったので対応しました https://github.com/srz-zumix/iutest/pull/516/files

### OSS 関連

* [wandbox-api][]
  * [v0.9.16](https://github.com/srz-zumix/wandbox-api/releases/tag/v0.9.16)
    * D に対応
* [awesome-cpp-warning][]
  * ときどき更新してます
* [textlint-plugin-review-starter][]
  * [Re:VIEW Starter][] 用の [textlint][] プラグインをリリースしました  
   [textlint-plugin-review-starter - npm](https://www.npmjs.com/package/textlint-plugin-review-starter)
* Docker
  * [docker-gilot](https://github.com/srz-zumix/docker-gilot)
    * 最新版のビルド失敗に対応
    * バージョンタグに対応
  * [docker-zapcc](https://github.com/srz-zumix/docker-zapcc)
    * Ubuntu のバージョンに対応（latest, bionic）
    * 定期ビルドに対応
  
### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2020/10/)
  * [GitHub Actions のコンテナに setup-python したときの error while loading shared libraries 対応](https://srz-zumix.blogspot.com/2020/10/github-actions-setup-python-error-while.html)
  * [OpenSTF を Windows の Docker 上で動かす](https://srz-zumix.blogspot.com/2020/10/openstf-windows-docker.html)
  * [lizard で C++ コードメトリクス](https://srz-zumix.blogspot.com/2020/10/lizard-c.html)
  * [\[C++\]\[IWYU\] Include What You Use CL を VS2019 対応しました](https://srz-zumix.blogspot.com/2020/10/ciwyu-include-what-you-use-cl-vs2019.html)
* [Zenn][]
  * [Zenn の @\[tweet\] の挙動調査](https://zenn.dev/srz_zumix/articles/4db858c9776081d3191e)
  * [Zenn の記事を private/public repository で同期する GitHub Actions](https://zenn.dev/srz_zumix/articles/d67dd4d082794929902a)

### 仕事

* 健康診断しました
  * 体重は思ったほど落ちてませんでした。おそらく肉体の限界なのでしょう
  * 視力はまたさらに落ちたかも
* リモートデスクトップで OpenGL が使えない問題を解決した
  * いちいち VNC で起動してから RDP に戻ったりしてたのですが助かりました
  * [OpenGLを使えるリモートデスクトップを構成する – すらりん日記](https://blog.techlab-xe.net/enable-opengl-rdp-nvidia/)

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
  * [\[AppVeyor\] fatal: reference is not a tree が出る場合の対応](https://srz-zumix.blogspot.com/2020/09/appveyor-fatal-reference-is-not-tree.html)
  * [\[Re:VIEW Starter\]\[Re:VIEW\] 訳あって Starter から素の Re:VIEW に戻すツールをリリースしました](https://srz-zumix.blogspot.com/2020/09/review-starterreview-starter-review.html)
  * [GitHub Sponsor のバッジを付ける方法](https://srz-zumix.blogspot.com/2020/09/github-sponsor.html)
  * [\[C++\] 警告のコンパイラー対応表を作り始めました](https://srz-zumix.blogspot.com/2020/09/c.html)
  * [Zenn とブログズミ](https://srz-zumix.blogspot.com/2020/09/zenn.html)
* 執筆
  * [無料で始める！CIサービスカタログ](https://nextpublishing.jp/book/12228.html)
* [Zenn][]
  * [Zenn][] での執筆を始めました
  * [CI サービスを活用して Zenn の執筆環境を作る - 序章 | Zenn](https://zenn.dev/srz_zumix/articles/9404b45e22cdf0f65ddd)
  * [\[C++\] GCC/Clang/VisualStudio の警告をまとめているので紹介 | Zenn](https://zenn.dev/srz_zumix/articles/4c72e544b0034cc796da)
  * [\[textlint\] Zenn 独自記法への警告を除外する | Zenn](https://zenn.dev/srz_zumix/articles/cb21af1a86fc01cb829d)
  * [\[C++\] override すべき関数の名前 typo に気づける idiom | Zenn](https://zenn.dev/srz_zumix/articles/ae351b73da285447fdc0)

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
  * [\[GitHub Actions\] Actions の PR 時に自分自身をアクションとして実行する](https://srz-zumix.blogspot.com/2020/08/github-actions-actions-pr.html)
  * [\[iutest\] ドキュメントの置き場を GitHub Pages に集約した](https://srz-zumix.blogspot.com/2020/08/iutest-github-pages.html)
  * [\[Doxygen\] @page の名前には小文字を使おう](https://srz-zumix.blogspot.com/2020/08/doxygen-page.html)
  * [\[技術書典\] Re:VIEW Starter でクローバー「♣」を別の文字に変更する](https://srz-zumix.blogspot.com/2020/03/wip-review-starter.html)
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
  * [\[Travis CI\] Segmentation fault したときにスタックトレースを出力する設定](https://srz-zumix.blogspot.com/2019/10/wiptravis-ci-segmentation-fault.html)
  * [\[CI\]\[CodeReview\] LGTM.com 始めました](https://srz-zumix.blogspot.com/2020/06/cicodereview-lgtmcom.html)
  * [\[技術書\] 画像のフォーマットチェックを GitHub Actions でしてみた](https://srz-zumix.blogspot.com/2020/07/github-actions.html)
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

[actions-book-image-check]:https://github.com/srz-zumix/actions-book-image-check
[Appcircle]:https://appcircle.io/
[AppVeyor]:https://www.appveyor.com
[AzurePipelines]:https://azure.microsoft.com/ja-jp/services/devops/pipelines/
[Azure Pipelines]:https://azure.microsoft.com/ja-jp/services/devops/pipelines/
[awesome-cpp-warning]:https://github.com/srz-zumix/awesome-cpp-warning
[Bitrise]:https://www.bitrise.io/
[Booth 虎空棘魚]:https://srz-zumix.booth.pm/
[ci-normalize-envvars]:https://github.com/srz-zumix/ci-normalize-envvars
[ci-specs]:https://github.com/srz-zumix/ci-specs
[ci-trigger]:https://github.com/srz-zumix/ci-trigger
[ci-skip]:https://github.com/srz-zumix/ci-skip
[cpprefjp]:https://cpprefjp.github.io/
[Drone.io]:https://drone.io/
[GoogleTest]:https://github.com/google/googletest
[GitHub Actions]:https://github.co.jp/features/actions
[iutest]:https://github.com/srz-zumix/iutest
[LGTM.com]:https://lgtm.com/
[Lizard]:https://github.com/terryyin/lizard
[RazorOps]:http://razorops.com/
[Re:VIEW]:https://reviewml.org/
[review-retrovert]:https://github.com/srz-zumix/review-retrovert
[Re:VIEW Starter]:https://kauplan.org/reviewstarter/
[Shippable]:https://app.shippable.com/
[Sider]:https://sider.review/
[TampermonkeyUserScripts]:https://github.com/srz-zumix/TampermonkeyUserScripts
[textlint]:https://github.com/textlint/textlint
[textlint-plugin-review-starter]:https://github.com/srz-zumix/textlint-plugin-review-starter
[Wandbox]:https://wandbox.org/
[wandbox-builder]:https://github.com/melpon/wandbox-builder
[Wandbox API]:https://github.com/melpon/wandbox/blob/master/kennel2/API.rst
[wandbox-api]:https://github.com/srz-zumix/wandbox-api
[Wercker]:https://app.wercker.com/
[zapcc]:https://github.com/yrnkrn/zapcc
[Zenn]:https://zenn.dev/srz_zumix
[あつまれ CI サービス 2020冬]:https://techbookfest.org/product/6709381972361216?productVariantID=5598210112356352
[技術書典10]:https://techbookfest.org/event/tbf10
[詳解 Integromat iPaaS 完全入門]:https://techbookfest.org/product/5328534149005312?productVariantID=6553683770736640
