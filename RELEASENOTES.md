# 自分リリースノート (Myself Release Notes)

* [0.35](old/RELEASENOTES_35.md)
* [0.34](old/RELEASENOTES_34.md)

## 0.36.1.4 (2022/04)

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

[docker-iwyu]:https://github.com/srz-zumix/docker-iwyu
[iutest]:https://github.com/srz-zumix/iutest
[jenkinsfile-shellcheck]:https://github.com/srz-zumix/jenkinsfile-shellcheck
[setup-service-jenkins]:https://github.com/srz-zumix/setup-service-jenkins
[Wandbox]:https://wandbox.org/
[Wandbox Status]:https://srz-zumix.github.io/wandbox-status/
[wandbox-api]:https://github.com/srz-zumix/wandbox-api
[wandbox-builder]:https://github.com/melpon/wandbox-builder
[wandbox-status]:https://github.com/srz-zumix/wandbox-status
[yurumikuji]:https://github.com/srz-zumix/yurumikuji
