# homenikki_archive
褒めてくれる日記

## ローカルで動かすのにインストールが必要なもの
* Mecab
* Cabocha
* Python インタプリタ
* いくつかのPythonモジュール
  * pip -r homenikki/lib/requirements.txt でまとめてインストールできます

# 環境構築手順
* Mecabのインストール
  * Homebrewなら 'brew install mecab' で簡単インストール。Ubuntu等でも 'apt install mecab' でインストール。もしくは公式サイト( https://taku910.github.io/cabocha/ )　からダウンロード＆インストール
* Cabochaのインストール
  * Homebrewなら 'brew install cabocha' で簡単インストール。もしくは公式サイト( https://taku910.github.io/cabocha/ )　からダウンロード＆インストール
  * Pythonから呼び出すためPythonバインディングが必要。[この](https://qiita.com/musaprg/items/9a572ad5c4e28f79d2ae)サイトなど参考に。
* Google text-to-speech 設定
  * [text-to-speech API](https://cloud.google.com/text-to-speech?hl=ja) を有効化する。 お手持ちのGoogle アカウントで登録後、[このへん](https://cloud.google.com/text-to-speech/docs/before-you-begin?hl=ja)を参考にサービスアカウントを作成、キーをJSONファイルでローカルに保存し、そのパスを環境変数'GOOGLE_APPLICATION_CREDENTIALS'に書き込む。
  * うっかりGitHubリポジトリの中に入れてpushしないように注意。
  * text-to-speechは無料枠が月100万文字なので注意。その後100万文字ごとに16ドルかかる。（まず超すことはないと思われるが）
