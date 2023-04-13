# Mastodon Now

<p align="center">
<img src="https://github.com/sasakulab/mastodon-now/raw/main/assets/96x96.png"
	alt="Mastodon Now" width="96" height="96" />
</p>

## これはなに

**\#now*do*ing** なノートを Mastodon に投稿する Chrome 拡張機能です。

![#nowdoing](/img/nowdoing.png)

## インストール

以下の拡張機能プロバイダーから、お使いのブラウザにインストールしてください。

【準備中】

- ~~[Chrome ウェブストア](https://chrome.google.com/webstore/detail/mastodon-now/gaanhijofgiahpbmjelcfhccepcgbekh)~~
- ~~[Firefox Browser ADD-ONS](https://addons.mozilla.org/ja/firefox/addon/mastodon-now/)~~

Microsoft Edge は、"Chrome ウェブストア" からサイドロードできます。

## 初期設定

まずは **アクセストークン** を用意する必要があります。

1. Mastodon の **ユーザ設定** を開きます。
2. **開発** のタブを開き、**新規アプリ** を作成します。
3. **アプリの名前** には “Mastodon Now” などわかりやすい名前を指定します。
4. **アクセス権** から少なくとも **write:statuses** (**投稿の送信**) を選択します。
5. 画面最下部の **送信** を押下してアプリを作成します。
6. 作成されたアプリの名前をクリックしてアプリを開きます。
7. **アクセストークン** の欄に表示されている文字列がアクセストークンです。

次に Mastodon Now にアクセストークンを設定します。

1. Mastodon Now を起動し、**Settings** を開きます。
2. **Profile Name** にはインスタンス名などわかりやすい名前を指定します。
3. **Host** にはインスタンスホスト名を指定します (`https://` は必要ありません)。
4. **API Key** には上で用意したアクセストークンを指定します。
5. 最後に **Save Settings** を押下して設定を保存します。

## 審査用ファイルの生成

```sh
cd path/to/mastodon-now/
zip -r -FS ../mastodon-now.zip * --exclude '*.git*' 'README.md' '*img*'
```

## Contributor

この場を借りて厚く御礼申し上げます。

- [@KusaReMKN](https://kusaremkn.com/)
