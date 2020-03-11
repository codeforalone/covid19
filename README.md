# 愛知県(非公式) 新型コロナウイルス感染症対策まとめサイト

愛知県もやりましょう
取り急ぎ作りました。

## 東京都 新型コロナウイルス感染症対策サイト

[![東京都 新型コロナウイルス感染症対策サイト](https://user-images.githubusercontent.com/1301149/75629392-1d19d900-5c25-11ea-843d-2d4376e3a560.png)](https://stopcovid19.metro.tokyo.lg.jp/)

### 【北海道版】新型コロナウイルス感染症対策サイト
[サイトへのリンク](https://stopcovid19.hokkaido.dev/)

[GitHubへのリンク](https://github.com/codeforsapporo/covid19)

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
```
$ yarn install
```

**docker compose を使う場合**
```bash
$ docker-compose run --rm app yarn install
```

### ステージング・本番環境への反映

`master` ブランチがアップデートされると、自動的に `production` ブランチにHTML類がbuildされます。そして、本番サイト https://covid19-aichi-unoffical.netlify.com/ が更新されます。

`staging` ブランチがアップデートされると、自動的に `gh-pages` ブランチにHTML類がbuildされます。そして、ステージングサイト https://stg-covid19-aichi-unoffical.netlify.com/ が更新されます。

`development` ブランチがアップデートされると、自動的に `dev-pages` ブランチにHTML類がbuildされます。そして、開発用サイト https://dev-covid19-aichi-unoffical.netlify.com/が更新されます。