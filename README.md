# pleasanter

### 目的
---

ホストマシン上でPleasanterを円滑に利用開始できることを目的としています。
そのため環境変数はソースコードの管理下においております。



### 前提
---

- 2025年2月5日時点の記事を[参考](https://pleasanter.org/ja/manual/getting-started-pleasanter-docker)にセットアップしました。
- Docker Desktopがホストマシン上にインストールされていること。


### システムの起動
---
```sh
## imageのpull
docker compose pull

## CodeDefinerの起動
docker compose run --rm codedefiner _rds /l "ja" /z "Asia/Tokyo"

## システムの起動
docker compose up -d pleasanter
```


### システムへのアクセス
---
http://localhost:50001 にアクセス

以下が初回ログイン時の情報
- user: `Administrator`
- pass: `pleasanter`
