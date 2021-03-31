# 自分リリースノート (Myself Release Notes)

[0.34](old/RELEASENOTES_34.md)

## 0.35.0.3 (2021/03)

### iutest 関連

* Bitrise の stack 更新
* CircleCI でテスト結果を集計

### OSS 関連

* [wandbox-builder]
  * いくつかの head 修正とバージョン追加をしました https://github.com/melpon/wandbox-builder/pulls?q=is%3Apr+author%3Asrz-zumix+
  * [Julia][] を足してみた https://github.com/melpon/wandbox-builder/pull/85
* [wandbox-api][]
  * glob 形式のコンパイラーバージョン指定に対応しました https://github.com/srz-zumix/wandbox-api/pull/35
  * compilers/versions サブコマンドの出力を言語名でソートしました https://github.com/srz-zumix/wandbox-api/pull/37
  * verbose オプションを追加しました https://github.com/srz-zumix/wandbox-api/pull/36
* [wandbox-status][]
  * [Wandbox] で実行可能になっているかのステータスページを作成しました

### ブログ/執筆

* [ブログズミ](https://srz-zumix.blogspot.com/2021/03/)
  * [\[Wercker\] DockerHub pull rate limit に対応する](https://srz-zumix.blogspot.com/2021/03/wercker-dockerhub-pull-rate-limit.html)
  * [wandbox-builder のテスト環境構築](https://srz-zumix.blogspot.com/2021/03/wandbox-builder.html)
  * [PyPI のリリースを検知して Dockerhub の image を更新する](https://srz-zumix.blogspot.com/2021/03/pypi-dockerhub-image.html)

### その他

* 今年も無事 minor バージョンアップしました

[iutest]:https://github.com/srz-zumix/iutest
[Julia]:https://julialang.org/
[Wandbox]:https://wandbox.org/
[wandbox-builder]:https://github.com/melpon/wandbox-builder
[wandbox-status]:https://github.com/srz-zumix/wandbox-status
