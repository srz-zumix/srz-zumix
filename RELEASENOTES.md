# 自分リリースノート (Myself Release Notes)

[0.34](old/RELEASENOTES_34.md)

## 0.35.7.10 (2021/10)

## 0.35.6.9 (2021/09)

### iutest 関連

* [std::complex に対応](https://github.com/srz-zumix/iutest/pull/621)

### OSS 関連

* [tails-of-words v0.3.0](https://github.com/srz-zumix/tails-of-words/releases/tag/v0.3.0) をリリースしました

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/09/)
  * [GitHub Actions でペアな値のマトリックスを組む](https://srz-zumix.blogspot.com/2021/09/github-actions.html)
  * [CEDEC でやってた表記ゆれ検出をお試し実装してみた](https://srz-zumix.blogspot.com/2021/09/cedec.html)
  * [GitHub Actions Composite Action で uses が使えるようになった！ ](https://srz-zumix.blogspot.com/2021/09/github-actions-composite-action-uses.html)

### その他

* シルバーウィークから Tales of ARISE をやってます（もうちょいでクリアだと思う）

## 0.35.5.8 (2021/08)

### iutest 関連

* [CircleCI の Matrix](https://circleci.com/blog/circleci-matrix-jobs/) を使うように更新
* [RazorOps][] が失敗し続けていたのを修正
* [TeamCity][] のベータライセンス期限切れにより google test 互換性検証を GitHub Actions へ

### OSS 関連

* Docker Automated Build から GitHub Actions に移行
* [wandbox-status][] にステータスページを追加 [Wandbox Status][]
* [review-retrovert][] の　[v0.9.11](https://github.com/srz-zumix/review-retrovert/releases/tag/v0.9.11) を公開

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/08/)
  * [ゲーム開発者のための SRE](https://srz-zumix.blogspot.com/2021/08/sre.html) 
  * [DockerHub Automated Build の Webhook の代わりに GitHub Actions workflow_dispatch を使う](https://srz-zumix.blogspot.com/2021/08/dockerhub-automated-build-webhook.html)
  * [【JFrog Pipelines】Cron Trigger を設定する](https://srz-zumix.blogspot.com/2021/08/jfrog-pipelinescron-trigger.html)

### その他

* [CEDEC2021][] に参加しました
  * [ゲーム制作効率化のためのAIによる画像認識・自然言語処理への取り組み](http://cedec.cesa.or.jp/2021/session/detail/s6049c15401f23) を聞いて、形態素解析・編集距離による表記ゆれ検出を実装してみました [tails-of-words][]

## 0.35.4.7 (2021/07)

### iutest 関連

* CI メンテナンス

### ブログ/執筆

* [技術書典11](https://techbookfest.org/event/tbf11)
  * [あつまれCIサービス 2021夏](https://techbookfest.org/product/6495998996119552?productVariantID=4991051045535744)
* [ブログズミ](https://srz-zumix.blogspot.com/2021/07/)
  * [技術書典11お疲れ様でした＆ブログのこれから](https://srz-zumix.blogspot.com/2021/07/11.html)
  * [Re:VIEW Starter から Re:VIEW のプロジェクトに戻すツール review-retrovert 0.9.9 リリース](https://srz-zumix.blogspot.com/2021/07/review-starter-review-review-retrovert.html)
  * [【技術書典11】 CI サービス本の増補・改訂版をリリースしました](https://srz-zumix.blogspot.com/2021/07/11-ci.html)
  * [\[Azure Pipelines\] DockerHub pull rate limit に対応する](https://srz-zumix.blogspot.com/2021/07/azure-pipelines-dockerhub-pull-rate.html)

### その他

* ワクチン接種２回目を終えました
  * 腕の痛みは全然なかった（刺された場所が良かった？）
  * 熱が１回目よりも出ていた気がする 38.4 までは計ったけど、以降はしんどくてぶっ倒れてた
  * 副反応でダウンしててそのせいか気持ちもダウンしてる

## 0.35.3.6 (2021/06)

### iutest 関連

* ミリ秒出力対応
* CI パイプライン更新（GitHub Actions/Bitrise）

### CI 関連

* [JFrog Pipelines][]　はじめました
* [ci-specs][] 追記

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/06/)
  * [JFrog Pipelines はじめました](https://srz-zumix.blogspot.com/2021/06/jfrog-pipelines.html)
  * [iutest の CircleCI ワークフローにパスフィルターを適用した](https://srz-zumix.blogspot.com/2021/06/iutest-circleci.html)
  * [Blogger の投稿を Integromat でツイートする Ver.2](https://srz-zumix.blogspot.com/2020/03/wip-rpa-blogger-integromat-ver2.html)

### その他

* 職域接種で1回目のワクチン接種しました
  * 38.2 度まで熱上がったけど

## 0.35.2.5 (2021/05)

### iutest 関連

* ARM 対応 https://github.com/srz-zumix/iutest/pull/584
* VS2010 サポート終了対応
* Shippable から [JFrog Pipelines][] に引っ越し
* [Travis CI][] 再開対応

### CI 関連

* [JFrog Pipelines][] の調査中
* Shippable EoS 対応

### OSS 関連

* docker
  * https://github.com/srz-zumix/docker-arm-none-eabi
  * https://github.com/srz-zumix/docker-unityhub
* [wandbox-api][]
  * バグ修正

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/05/)
  * [DockerHub / GitHub Actions での docker build が No space left on device だったので CircleCI でビルドした話](https://srz-zumix.blogspot.com/2021/05/dockerhub-github-actions-docker-build.html)
  * [\[技術書典\] Re:VIEW Starter で印刷・電子書籍版で config.yml を使い分ける](https://srz-zumix.blogspot.com/2020/03/wip-review-starter-configyml.html)
  * [XCode ビルド時に codesign で errSecInternalComponent エラーが発生した場合に最初に確認すべきこと in 2021](https://srz-zumix.blogspot.com/2021/05/xcode-codesign-errsecinternalcomponent.html)
  * [\[Debian\] pyenv install で Missing the OpenSSL lib? で失敗する場合の対応と 3.0~3.10 全部入り Dockerfile 書いた](https://srz-zumix.blogspot.com/2021/05/debian-pyenv-install-missing-openssl.html)
  * [Linux版 UnityHub の headless に対応した Docker image](https://srz-zumix.blogspot.com/2021/05/linux-unityhub-headless-docker-image.html) 
* 技術書典11 に応募しました

## 0.35.1.4 (2021/04)

### iutest 関連

* CircleCI で path filter に対応

### OSS 関連

* [wandbox-builder][]
  * いくつかの head 修正とバージョン追加をしました https://github.com/melpon/wandbox-builder/pulls?q=is%3Apr+author%3Asrz-zumix+
* [wandbox-api][]
  * 現在 [Wandbox][] で提供されている言語すべての CLI に対応
  * ndjson/user api に対応
* [Julia][] に出してた [PR](https://github.com/JuliaLang/julia/pull/40136) がマージされた
* [Jinja2][]
  * [kamidana][] の additionals な Slack API 拡張 [yurumikuji][] を公開
  * [kamidana][] に Wandbox API additionals を追加した wrapper [amaterasu][] を公開
* Unity
  * Unity のファイルの YAML 要素を正規化するツールを公開 [unity-yaml-normalize][]
* docker
  * [docker-onepai-hpckit](https://github.com/srz-zumix/docker-oneapi-hpckit)
  * [docker-oneapi-cxx](https://github.com/srz-zumix/docker-oneapi-cxx)
 　
### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/04/)
  * [ウマ娘にハマってしまっていた](https://srz-zumix.blogspot.com/2021/04/blog-post.html)
  * [【Ruboty】Slack のリアクションに反応できるようにするプラグインを公開](https://srz-zumix.blogspot.com/2021/04/rubotyslack.html)
  * [Jinja2 cli な kamidana の additonals として slack 拡張を書いてみた](https://srz-zumix.blogspot.com/2021/04/jinja2-cli-kamidana-additonals-slack.html)
  * [docker build ログを今まで通りに表示する](https://srz-zumix.blogspot.com/2021/04/docker-build.html) 
  * [CircleCI でモノレポ上の指定パスに変更があったらテストを走らせる](https://srz-zumix.blogspot.com/2021/04/circleci.html)

### その他

* ウマ娘
  * 時間泥棒だというのはパワプロのときから知ってるんだけどやっちゃうな 

## 0.35.0.3 (2021/03)

### iutest 関連

* Bitrise の stack 更新
* CircleCI でテスト結果を集計

### OSS 関連

* [wandbox-builder][]
  * いくつかの head 修正とバージョン追加をしました https://github.com/melpon/wandbox-builder/pulls?q=is%3Apr+author%3Asrz-zumix+
  * [JuliaLang][] を足してみた https://github.com/melpon/wandbox-builder/pull/85
* [wandbox-api][]
  * glob 形式のコンパイラーバージョン指定に対応しました https://github.com/srz-zumix/wandbox-api/pull/35
  * compilers/versions サブコマンドの出力を言語名でソートしました https://github.com/srz-zumix/wandbox-api/pull/37
  * verbose オプションを追加しました https://github.com/srz-zumix/wandbox-api/pull/36
* [wandbox-status][]
  * [Wandbox][] で実行可能になっているかのステータスページを作成しました

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/03/)
  * [\[Wercker\] DockerHub pull rate limit に対応する](https://srz-zumix.blogspot.com/2021/03/wercker-dockerhub-pull-rate-limit.html)
  * [wandbox-builder のテスト環境構築](https://srz-zumix.blogspot.com/2021/03/wandbox-builder.html)
  * [PyPI のリリースを検知して Dockerhub の image を更新する](https://srz-zumix.blogspot.com/2021/03/pypi-dockerhub-image.html)

### その他

* 今年も無事 minor バージョンアップしました

[amaterasu]:https://github.com/srz-zumix/amaterasu
[CEDED2021]:https://cedec.cesa.or.jp/2021/
[ci-specs]:https://github.com/srz-zumix/ci-specs
[iutest]:https://github.com/srz-zumix/iutest
[JFrog Pipelines]:https://www.jfrog.com/confluence/display/JFROG/JFrog+Pipelines
[Jinja2]:https://jinja.palletsprojects.com/en/2.11.x/
[Julia]:https://github.com/JuliaLang/julia
[JuliaLang]:https://julialang.org/
[kamidana]:https://github.com/podhmo/kamidana
[RazorOps]:https://razorops.com/
[review-retrovert]:https://github.com/srz-zumix/review-retrovert
[tails-of-words]:https://github.com/srz-zumix/tails-of-words
[TeamCity]:https://www.jetbrains.com/ja-jp/teamcity/cloud/
[Travis CI]:https://travis-ci.com/
[unity-yaml-normalize]:https://github.com/srz-zumix/unity-yaml-normalize
[Wandbox]:https://wandbox.org/
[Wandbox Status]:https://srz-zumix.github.io/wandbox-status/
[wandbox-api]:https://github.com/srz-zumix/wandbox-api
[wandbox-builder]:https://github.com/melpon/wandbox-builder
[wandbox-status]:https://github.com/srz-zumix/wandbox-status
[yurumikuji]:https://github.com/srz-zumix/yurumikuji
