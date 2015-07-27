# 01 Python環境をインストールする
## Pythonの機械学習用スタック
Pythonを機械学習用に使うには、下記のライブラリをインストールするのが望ましい。
- IPython(インタラクティブシェル)
- NumPy(行列演算)
- SciPy(行列演算)
- Pandas(データフレーム)
- matplotlib(可視化)
- Seaborn(データビジュアライゼーション)
- Scikit Learn(機械学習)
- StatsModels(統計)
- OpenCV(コンピュータービジョン)
- gensim(自然言語処理用)
- Numba
- Cython

自分の場合、IPython, NumPy, SciPy, Pandas, matplotlib(Pylab), Scikit learnはよく使う。

LAPACKなどのライブラリへのリンクなども考えると、初期設定は結構大変なので、後述のAnacondaを使うのが一番簡単。

## Anacondaのインストール

Anacondaは、Continuum Analyticsの出している、科学技術演算用のPythonディストリビューションである。基本的には無料で使える。
上記に挙げたライブラリの多くがすでに組み込まれた状態でインストールできる。

https://store.continuum.io/cshop/anaconda/

anacondaは、`~/anaconda` 下にインストールを行う。

ターミナルで下記のように叩いて、エラーがなければインストールが成功している。

```
$ conda list
```

もしコマンドが見つからないなどのエラーが出た場合、`~/anaconda/bin`などにPATHを張ってあげると良い

## インストールの確認

下記のPythonコードを実行して、特に問題なければインストールが完了している。

Pythonのインタラクティブシェルとしては、IPythonを使うと便利。

```py
import numpy as np
import scipy as sp
import pandas as pd
import pylab as pl
import sklearn

np.array([0, 1, 2])
```
