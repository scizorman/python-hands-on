# チュートリアル

このチュートリアルでは，基本的な Git, GitHub の使い方について学習する。

### `Git` とは

プログラムソースなどの変更履歴を管理する分散型のバージョン管理システム。
最大の特徴は，ローカル環境 (自分の PC) に，全ての変更履歴を含む完全なレポジトリの複製が作成される。
そのため，ローカル環境にもコードの変更履歴を保存 (コミット) することが出来るので，リモートサーバーに常に接続する必要がなく，ネットワークに接続していなくても作業が出来る。

> 参考：[Git 公式サイト](https://git-scm.com/)

> 参考：[サルでも分かる Git 入門](http://www.backlog.jp/git-guide/)

### `GitHub` とは

Git の仕組みを利用して、世界中の人々が自分の作品(プログラムコードやデザインデータなど)を保存、公開することができるようにしたウェブサービス。

> 参考：[GitHub](https://github.com/)

## 手順

#### 1. GitHub アカウントを作成する

[GitHub](https://github.com) にアクセスし，アカウントを作成する。

#### 2. `python-hands-on` をフォークする

[python-hands-on](https://github.com/scizorman/python-hands-on) にアクセスし，右上にある `Fork` ボタンを押してこのレポジトリをフォークする。

#### 3. フォークしたレポジトリをクローンし，クローンしたディレクトリに移動する

```bash
$ git clone https://github.com/[アカウント名]/python-hands-on
$ cd python-hands-on
```

#### 4. チュートリアル用のブランチを作成する

```bash
$ git checkout -b feature/tutorial
```

#### 5. `sample.py` を更新する

`main 関数` を自由に書き換える。(e.g. 出力する文字列の変更)

#### 6. Git に変更を追加する

```bash
$ git add ./tutorial/sample.py
```

#### 7. Git にコミットする

```bash
$ git commit -m "[コミットメッセージ]"
```

##### 例：main 関数の出力する文字列を変更した場合

- [change] 出力する文字列を変更
- [change] Change the string to output

> 参考：[Git のコミットメッセージの書き方](https://qiita.com/itosho/items/9565c6ad2ffc24c09364)

#### 8. GitHub にプッシュする

```bash
$ git push origin feature/tutorial
```

#### 9. 本家レポジトリの master ブランチにプルリクエストを送る

口頭で説明する。
