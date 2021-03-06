# 自分リリースノート (Myself Release Notes)

[0.34](old/RELEASENOTES_34.md)

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
[ci-specs]:https://github.com/srz-zumix/ci-specs
[iutest]:https://github.com/srz-zumix/iutest
[JFrog Pipelines]:https://www.jfrog.com/confluence/display/JFROG/JFrog+Pipelines
[Jinja2]:https://jinja.palletsprojects.com/en/2.11.x/
[Julia]:https://github.com/JuliaLang/julia
[JuliaLang]:https://julialang.org/
[kamidana]:https://github.com/podhmo/kamidana
[Travis CI]:https://travis-ci.com/
[unity-yaml-normalize]:https://github.com/srz-zumix/unity-yaml-normalize
[Wandbox]:https://wandbox.org/
[wandbox-api]:https://github.com/srz-zumix/wandbox-api
[wandbox-builder]:https://github.com/melpon/wandbox-builder
[wandbox-status]:https://github.com/srz-zumix/wandbox-status
[yurumikuji]:https://github.com/srz-zumix/yurumikuji
