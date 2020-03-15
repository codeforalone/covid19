# 愛知県(非公式) 新型コロナウイルス感染症対策まとめサイト

### 非公式愛知県版について

- 愛知県の公式版がリリースされた場合は終了予定
- サイト構成などは東京版の構成から大きく変えないようにする
- データは愛知県の公式サイトからスクレイピングによって収集したものを整形して利用する
- Webホスティング環境は東京都同様netlifyを使用

## 開発者向け情報

### 環境構築の手順

- 必要となるNode.jsのバージョン: 10.19.0以上

**yarn を使う場合**

``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**docker compose を使う場合**

```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### `Cannot find module ****` と怒られた時

**yarn を使う場合**

```bash
$ yarn install
```

**docker compose を使う場合**

```bash
$ docker-compose run --rm app yarn install
```

### ステージング・本番環境への反映

`master` ブランチがアップデートされると、自動的に `production` ブランチにHTML類がbuildされます。そして、本番サイト http://stopcovid19.aichi-info.net/ が更新されます。

`staging` ブランチがアップデートされると、自動的に `gh-pages` ブランチにHTML類がbuildされます。そして、ステージングサイト https://stg-covid19-aichi-unoffical.netlify.com/ が更新されます。

`development` ブランチがアップデートされると、自動的に `dev-pages` ブランチにHTML類がbuildされます。そして、開発用サイト https://dev-covid19-aichi-unoffical.netlify.com/が更新されます。

