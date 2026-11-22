# BMI計算機（標準ライブラリだけ）

Python の標準ライブラリ（`wsgiref`）だけで動く、いちばん小さな Web アプリです。
練習用の形です。本格的な公開は、セクション7の Flask で行います。

## 手元で動かす

```
python app.py
```

ブラウザで `http://localhost:8000` を開きます（Mac は `python3 app.py`）。
ターミナルに `0.0.0.0` と出ても、ブラウザで開くのは `localhost` です。

## Render で公開する

- Runtime：Python
- Build Command：`pip install -r requirements.txt`（中身は空でかまいません）
- Start Command：`python app.py`

## うまく動かない時

- 公開した URL が開かない：`host` が `0.0.0.0` になっているか、`PORT` の環境変数を読んでいるかを確かめます。
- 身長は 50〜300（cm）、体重は 1〜500（kg）の範囲だけを受け付けます。範囲の外や数字でない値は、画面に理由が出ます。
