# 自分リリースノート (Myself Release Notes)

* [0.35](old/RELEASENOTES_35.md)
* [0.34](old/RELEASENOTES_34.md)

## 0.36.8.11 (2022/11)

### iutest 関連

* ing
  * C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
  * Google Test 12.X 互換性対応

### OSS 関連

* git にパッチ送った https://github.com/gitgitgadget/git/pull/1406
* [GITHUB_OUTPUT](https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/) に対応中

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/11/) 
  * [git で新規ブランチ作成時の typo を防ぐ](https://srz-zumix.blogspot.com/2022/11/git-typo.html)
  * [【Make formerly Integromat】Twitter でいいねした画像を自動でクラウドストレージに保存する
](https://srz-zumix.blogspot.com/2022/11/make-formerly-integromattwitter.html)

### その他

* お絵かき
  * 絵ばっか書いててほとんどプログラミングしない、記事も書かない月だった
  * 仕事のコーディングが楽しいので趣味プログラミングが減ってきた
  * あれ、先月と同じこと言ってる


## 0.36.7.10 (2022/10)

### iutest 関連

* ing
  * C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
* done
  * Codefresh でテストデータ作成失敗してたのでスキップ可能に修正

### OSS 関連

* [GITHUB_OUTPUT](https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/) に対応中

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/10/) 
  * [【GitHub Actions】コンテキストダンプのススメ](https://srz-zumix.blogspot.com/2022/10/github-actions.html)

### その他

* お絵かき
  * 絵ばっか書いててほとんどプログラミングしない、記事も書かない月だった
  * 仕事のコーディングが楽しいので趣味プログラミングが減ってきた

## 0.36.6.9 (2022/09)

### iutest 関連

* ing
  * C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
* done
  * 2GB を超えるファイルサイズの取得 https://github.com/srz-zumix/iutest/pull/663 

### OSS 関連

* [gh-act][]
  * 0.2 をリリースしました
* [tails-of-words][]
  * [補助動詞の漢字・ら抜き言葉の検出を実装](https://github.com/srz-zumix/tails-of-words/pull/22) 

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/09/) 
  * [CEDEC でやってた補助動詞の漢字・ら抜き言葉の検出を実装してみた](https://srz-zumix.blogspot.com/2022/09/cedec.html)
  * [Dagger 使ってみた](https://srz-zumix.blogspot.com/2022/09/dagger.html)
  * [Homebrew と git fsmonitor の相性が悪かったので対策した](https://srz-zumix.blogspot.com/2022/09/homebrew-git-fsmonitor.html) 
* [Zenn][]
  * [GitHub Actions のローカル実行ツール（nektos/act）を便利にする gh extension を作った](https://zenn.dev/srz_zumix/articles/gh-act-first-released) 

### その他

* お絵かき
  * デジタルお絵かき初めて一ヶ月、多少上達したかな
  * 手軽に消したり、修正できるのでどこが悪かったのか、どうすればよかったのかがやりやすくてアナログで枚数描くより効率的に思えた
  * お絵かき用の twitter アカウントも作った
  * なぜかどんどんおっぱいが大きくなっていく
* 趣味=プログラミングと言ってきたけど、できないことにできるようにするのが好きなのかも

## 0.36.5.8 (2022/08)

### iutest 関連

* ing
  * 2GB を超えるファイルサイズの取得を修正中 https://github.com/srz-zumix/iutest/pull/663 
  * C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627

### OSS 関連

* [gh-act][]
  * [nektos/act][] の補助ツールを開発しています 
* [wandbox-api][]
  * ファイルの自動追加機能を、1行に複数の statement ある場合にも対応
* いくつか OSS に軽微な PR をしました

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/08/) 
  * [GitHub Actions の Composite Action で post 処理を実現する方法](https://srz-zumix.blogspot.com/2022/08/github-actions-composite-action-post.html)
  * [Git で今のブランチ名を取得するコマンドの違いを確認してみた](https://srz-zumix.blogspot.com/2022/08/git.html)
  * [nektos/act で GitHub Actions のワークフローをローカル実行](https://srz-zumix.blogspot.com/2022/08/nektosact-github-actions.html)

### その他

* CEDEC に参加しました
* お絵かきように Galaxy Tab S8 Ulta を買いました
* リリースノート書いてて気づいたけど最近 Git やら GitHub Actions のことばっかりやってるな
* 画像生成 AI まだ 1 つもやってません。Waifu Lab を昔使ったことはある。来月は触ってみたい

## 0.36.4.7 (2022/07)

### iutest 関連

* ing
  * 2GB を超えるファイルサイズの取得を修正中 https://github.com/srz-zumix/iutest/pull/663 
  * C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
* done
  * CMake を更新
    * Visual Studio の場合の対応を更新
    * /std=c++latest 対応
    * テスト結果のアウトプットに対応
  * Earthly 導入 https://github.com/srz-zumix/iutest/pull/667
  * Dagger の更新 https://github.com/srz-zumix/iutest/pull/666
  * Bitrise に iOS ビルドを追加（今までのは MacOS ビルドだった）
  * sider/wercker のリンク削除

### OSS 関連

* [Wandbox Status][] に Zig を追加
* [wandbox-api][]
  * wandbox-status コマンドを未知の言語にも対応
  * Zig を追加
  * ; で statement 区切られた場合のファイル自動追加処理を修正中
    * 1行に複数 import とかに対応してなかった 
  * require version を python >3.5 に変更
    * 3.5 ない機能を使うためにそうしたけど、結局使わなかった。が、まぁ古いし上げてしまう
* [amaterasu][]
  * dependency の問題を修正 
* [ci-specs][]
  * メンテナンス
  * Sider 削除
  * Wercker 削除

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/07/) 
  * [Git 2.37.0 で FSMonitor daemon が追加されたことで status が早くなったそうです](https://srz-zumix.blogspot.com/2022/07)
  * [Integromat migrate to Make (formerly Integromat)](https://srz-zumix.blogspot.com/2022/07/integromat-migrate-to-make-formerly.html)
  * [Slack の過去の投稿を再投稿して 90 日制限を回避する](https://srz-zumix.blogspot.com/2022/07/slack-90.html)

### その他

* Dagger 見てたけど Earthly のほうがいいじゃんってなってる
* Make formeryl Integromat 特に変わらず使えてる、というか変わったところがわからんくてなんで一新したのがわからん
* 最近お絵かきしてます。人に見せられるレベルになったらなんか考える
* バイナリ列見てこれは〜だねといえるようになりたかった

## 0.36.3.6 (2022/06)

### iutest 関連

* ing
  * 2GB を超えるファイルサイズの取得を修正中 https://github.com/srz-zumix/iutest/pull/663 
  * C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
* done
  * [Dagger][] https://github.com/srz-zumix/iutest/pull/653
  * alpine linux でのビルドエラー修正 https://github.com/srz-zumix/iutest/pull/653

### OSS 関連

* [setup-service-jenkins][]
  * v2 released
    * node の登録対応
    * サービスコンテナの指定を name のみに簡略化
* [jenkinsfile-shellcheck][] released
  
### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/06/) 
  * [Jenkinsfile の sh ブロックの shellcheck をする GitHub Action をリリースしました](https://srz-zumix.blogspot.com/2022/06/jenkinsfile-sh-shellcheck-github-action.html)
  * [Jenkinsfile の checkout gitSCM で LFS Pull のタイムアウト設定](https://srz-zumix.blogspot.com/2022/06/jenkinsfile-checkout-gitscm-lfs-pull.html)
  * [【DockerHub】typo して間違った repository に push してしまった Docker image を正しい repository にコピーした](https://srz-zumix.blogspot.com/2022/06/dockerhubtypo-repository-push-docker.html) 

### その他

* 6月クソ暑
* Netflix 飽きてきた
* Dagger をもうちょっと使って記事にしたいと思ってるんだけどわからないことが多い

## 0.36.2.5 (2022/05)

### iutest 関連

* ing
  * [Dagger][] 導入中 https://github.com/srz-zumix/iutest/pull/653
  * alpine linux でのビルドエラー修正中 https://github.com/srz-zumix/iutest/pull/653
  * C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
* done
  * clang-tidy を実行するワークフロー作成と警告対応 https://github.com/srz-zumix/iutest/pull/646

### OSS 関連

* [setup-service-jenkins][]
  * setup wizard 対応
  * secrets 登録対応
* [docker-zapcc][]/[docker-iwyu][]
  * actions 向けに新しめの git をインストールするように修正 

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/05/) 
  * [GitHub Actions で export-ignore 指定したパスがワークスペースになくて composite action が実行できなかった話](https://srz-zumix.blogspot.com/2022/05/github-actions-export-ignore-composite.html)
  * [AppVeyor で cygwin setup に失敗するようになったので対応した](https://srz-zumix.blogspot.com/2022/05/appveyor-cygwin-setup.html)

### その他

* ゴールデンウィーク
  * 例年はカレンダー通りのことが多いが今年はつなげて連休にした
  * ちょー久しぶりにクソ休んだって感じ
* 健康寝台
  * 会社移転してから初めて出社した
  * といっても向かいのビルなので地理的には殆ど同じだけど
* Netflix 2ヶ月目
  * 最初は見たことあるアニメをよく見てたけど、最近は気になってはいたが見てなかったのを見てた
    * ヴァイオレット・エヴァーガーデン：泣けると聞いてたけどまあ泣けた。もともと涙腺弱いが年とってから完全崩壊、CM ですら泣ける体質なので大体の作品で泣いてるけど。。
    * はたらく細胞：アニメでわかりやすく勉強になっていいですね。
    * SHIROBAKO：ライバル企業の機材の愛称。。じゃなくてアニメの方ね。NEW GAME! も好きだけどこれも良いですね。
  * 完全ファンタジーよりも現実世界の延長で、へーそうなんだーと知識欲を満たしつつ、明日への気力が湧くものが好きなのかもしれない。
  * 泣ける系は、、最近泣くために見てる感もあって心の汚れがヤバい

## 0.36.1.4 (2022/04)

### iutest 関連

* [Dagger][] 導入中 https://github.com/srz-zumix/iutest/pull/653
* alpine linux でのビルドエラー修正中 https://github.com/srz-zumix/iutest/pull/653
* clang-tidy を実行するワークフロー作成と警告対応中 https://github.com/srz-zumix/iutest/pull/646
* C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
* gcc -fanalyzer の実行環境を模索中

### OSS 関連

* [setup-service-jenkins][]
  * JCasC 対応中
* [jenkinsfile-shellcheck][] : Jenkinsfile 中 sh のスクリプトに対して shellcheck を行うツールを開発中

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/04/) 
  * [Jenkinsfile がでかすぎてエラーになる場合の対処方法](https://srz-zumix.blogspot.com/2022/04/jenkinsfile.html)

### その他

* タイバニ2のために Netflix 入った
  * ジョンジョンいい名前だ
  * せっかく入ったので動画をちょこちょこ見てるのだが、知らない作品より過去に見た作品を懐かしんで見てしまうことが多い
  * twitter で見かけてた着せ恋あったので見たけど良かった。漫画欲しくなった。デジタルより物理のほうがいいけど、置き場ないから悩む
* いろいろ停滞してるんだけど、仕事とウマの影響ですな・・

## 0.36.0.3 (2022/03)

### iutest 関連

* clang-tidy を実行するワークフロー作成と警告対応中 https://github.com/srz-zumix/iutest/pull/646
* C++ Core Guidlines Check に対応中 https://github.com/srz-zumix/iutest/pull/627
* gcc -fanalyzer の実行環境を模索中

### OSS 関連

* Jenkins Configuration as Code Plugin の OverrideMergeStorategy の不具合がまだあったようなのでアドバイスしました
  * https://github.com/jenkinsci/configuration-as-code-plugin/pull/1914#issuecomment-1051429536
* [setup-service-jenkins][] : GitHub Actions で Jenkins service をセットアップするアクションをリリースしました
* [jenkinsfile-shellcheck][] : Jenkinsfile 中 sh のスクリプトに対して shellcheck を行うツールを開発しています
  * とりあえず sh スクリプトを抽出し shellcheck を実行するところまではできました 
* [docker-iwyu][] : マルチアーキテクチャ対応(amd64/arm64)、複数の base clang version と ubuntu version の組み合わせ対応

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2022/03/) 
  * [Include-What-You-Use の docker image を更新しました](https://srz-zumix.blogspot.com/2022/03/include-what-you-use-docker-image.html)
  * [GitHub Actions だけで Jenkinsfile の lint をする](https://srz-zumix.blogspot.com/2022/03/github-actions-jenkinsfile-lint.html)

### その他

* 最近ブログの執筆ペースが月２回ほどになってますが、ウマ娘のせいです。
* 今年も無事 minor バージョンアップしました

[amaterasu]:https://github.com/srz-zumix/amaterasu
[ci-specs]:https://github.com/srz-zumix/ci-specs
[Dagger]:https://dagger.io/
[docker-iwyu]:https://github.com/srz-zumix/docker-iwyu
[docker-zapcc]:https://github.com/srz-zumix/docker-zapcc
[gh-act]:https://github.com/srz-zumix/gh-act
[iutest]:https://github.com/srz-zumix/iutest
[jenkinsfile-shellcheck]:https://github.com/srz-zumix/jenkinsfile-shellcheck
[nektos/act]:https://github.com/nektos/act
[setup-service-jenkins]:https://github.com/srz-zumix/setup-service-jenkins
[tails-of-words]:https://github.com/srz-zumix/tails-of-words
[Wandbox]:https://wandbox.org/
[Wandbox Status]:https://srz-zumix.github.io/wandbox-status/
[wandbox-api]:https://github.com/srz-zumix/wandbox-api
[wandbox-builder]:https://github.com/melpon/wandbox-builder
[wandbox-status]:https://github.com/srz-zumix/wandbox-status
[yurumikuji]:https://github.com/srz-zumix/yurumikuji
[Zenn]:https://zenn.dev/srz_zumix
