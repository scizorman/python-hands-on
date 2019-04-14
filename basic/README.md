# 基本課題

JupyterLab を用いて，ノートブックに書かれている課題に取り組もう。

### `JupyterLab` とは

プログラムを実行し，実行結果を記録できる Web アプリケーション。
データ解析や機械学習に最適な統合開発環境である。

> 参考：[JupyterLab 公式ドキュメント](https://jupyterlab.readthedocs.io/en/stable/)

### セットアップ

#### 1. Pipenv を用いて，実行環境の構築・必要なパッケージのインストールを行う

```bash
$ pipenv --python 3.7.2
$ pipenv install -d
```

#### 2. JupyterLab を実行する

```bash
$ pipenv run jupyter lab
```

#### 3. JupyterLab 上で課題に取り組む

JupyterLab 上で `basic.ipynb` を開く。
