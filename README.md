# コンテナのビルド

## 手動でビルドする場合

```bash
$ docker buildx bake -f docker-compose.yml
$ docker compose up -d
```

## vscodeのremote containerでビルドする場合

`Open Folder in Container`でルートディレクトリを開く

# mkdocsの使い方

## プロジェクトの作成

```bash
$ mkdocs new test
```

## ビルド

```bash
$ cd test/
$ mkdocs build
```

## ローカル実行

```bash
$ mkdocs serve
```

vscodeのターミナルで事項している場合は`ブラウザで開く`メニューが出てくるのでクリックする。それ以外の環境では`127.0.0.1:8000`にアクセスする。
