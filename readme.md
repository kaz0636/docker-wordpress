# WordPress開発用

## ディレクトリ・ファイル構成

/

docker-compose.yml

.env.sample 環境変数ファイルサンプル

themes/

- テーマファイル用ディレクトリ
- 解凍したテーマファイルを置く

db-data/

- テスト用dbデータ
- 変更禁止

---

## 準備

### 環境変数ファイルの作成

```bash
cp .env.sample .env
```

内容を編集

---

## 起動

```bash
docker-composer up -d
```

### アクセスurl

[http://192.168.99.100](http://192.168.99.100)
または
[http://docker.local](http://docker.local)
(※hostsに追加済の場合)

### 登録されているユーザー

#### 管理者

- admin:admin

#### 一般ユーザー

- user1:user1
- user2:user2

### 一時停止

```bash
docker-composer stop
```

### 再開

```bash
docker-compose start
```


### 破棄

```bash
docker-composer down
```

