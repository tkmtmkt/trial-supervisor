study-supervisor
================

環境設定
--------

オンライン環境でインストールし、wheelパッケージをダウンロードする。

```sh
$ ./python/install.sh
```

オフライン環境でwheelパッケージからインストールする。

```sh
$ ./python/offline-install.sh
```


実行
----

作業用シェルを起動する。

```sh
$ ./python/shell.sh
```


補足
----

PyPiで配布されているsupervisorがpython3対応ではないため、
whlファイルは手動で作成する必要がある。
以下のコマンドで、distディレクトリ以下にwhlファイルが作成される。

```sh
$ git clone https://github.com/Supervisor/supervisor.git
$ cd supervisor
$ python setup.py bdist_wheel
```
