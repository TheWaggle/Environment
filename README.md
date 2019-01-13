# Environment
Elixir環境構築

## 簡単な説明
[事前準備](https://gist.github.com/Yoosuke/65873bff61ae66bd4ad1d23180a927f3)
開発に必要なツールは予めインストールしておきます。

## 環境構築手順
1.Elixirのインストールをします。
[Elixir](https://elixir-lang.org/install.html)
[node.js](https://nodejs.org/ja/)
[PostgreSQL](https://postgresapp.com/)

コンソール画面に入り、以下のコマンドを打つ
* hexファイルをUPdataします。
```
mix local.hex
```
* Phoenix v1.4をインストールします。
```
mix archive.install hex phx_new 1.4.0
```

* gismapというプロジェクト名でphx.newコマンドを打ちます。
```
mix phx.new gismap
```

依存関係を取得してインストールしますか？ [Yn]と聞かれるので、Yを入力します。
```
Fetch and install dependencies? [Yn] y
```

インストールすると、以下のコマンドが案内されるので、
順にコマンドをうっていきます。

```
We are almost there! The following steps are missing:

    $ cd gismap

Then configure your database in config/dev.exs and run:

    $ mix ecto.create

Start your Phoenix app with:

    $ mix phx.server

You can also run your app inside IEx (Interactive Elixir) as:

    $ iex -S mix phx.server

```

```
cd gismap

mix ecto.create

mix phx.server
```
http://localhost:4000　にアクセスして、以下が表示されていたら成功です。
![phx.server](template/img/phx.server.png)

