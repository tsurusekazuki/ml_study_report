# 機械学習モデル作成、評価、保存について

pythonの機械学習ライブラリである**scikit-learn**を用いてモデルのp作成・評価し、**pickie**tおいうライブラリで保存を行う。

## pickieでモデルを保存する

pickieは、pythonでオブジェクトをシリアライズ化(直列化)する一般的な方法。

>シリアライズ: プログラミング言語においてオブジェクトをバイト列などの表現に変換すること

## モデル作成から評価・保存までの流れ

モデル作成

```
// モデルのトレーニング
model = model = LogisticRegression()
model.fit(X_train, Y_train)

```

モデル評価

```
pred = model.predict(X_test)

```

モデル保存

```
pickle.dump(model, open(filename, 'wb'))

```
