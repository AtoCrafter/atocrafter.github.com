---
layout: page
title: "Access Chest"
description: "持ち運べる大容量チェストを追加します"
---
{% include JB/setup %}

![Access Chest の GUI 画面サンプル](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/ss.png)


特徴
----

- どこからでも手に持ったままアクセスできるチェスト
- 最大13824スタックの超巨大容量
- 16色の色分け管理
- その他便利な追加機能


導入方法
--------
### 前提 MOD
- Minecraft Forge

### **ダウンロード**
[こちらからダウンロード][download]
*対応バージョン : Minecraft 1.4.7*

### インストール
ダウンロードした zip ファイルを .minecraft/mods フォルダに直接入れてください。（クライアント・サーバー共に共通）

使い方
------
アイテムを持って右クリックをすると各色に応じたチェストを開くことができます。

Access Chest Class-1 は Class-0 の 8 倍の容量を、Class-2 は Class-1 の 8 倍の容量を……という具合に Class によって最大容量が異なります。
Class-0 の容量が 27 スタックなので消費したチェストと同等の容量を持つことになります。

Class が違っても色が同じなら中身は同じになります。逆に染色で色を変えると中身は異なります。

アイテムを持ってスニークキー（デフォルトでは Shift）を押しながら右クリックすると通常のチェストと同じように設置できます。
設置された Access Chest を壊すとアイテムとして回収できます。そのとき中身はこぼれません。

Access Chest とほぼ同じ機能を持ち、持ち運べないなどのいくつかの機能が制限された Compressed Chest も追加されます。
こちらはレシピにエンダーパールを使いません。

### 各種機能
#### フィルタ
Access Chest を開いたとき右下のテキストボックスに文字列を入力するとアイテム名にその文字列を含むアイテムがリストアップされます。
文字列の入力を始めるにはチャットキー（デフォルトでは T）を押すかテキストボックス内をクリックします。
テキストボックス内の文字列は Clear ボタンで空にできます。

#### ネーミング \(Rename\)
現在の色の Access Chest に名前をつけることができます。Rename ボタンを押したときのテキストボックスに入力されている文字列によって Access Chest のアイテム名が変化します。

#### ソート \(Sort\)
Sort ボタンで ID 順に並べ替えます。

#### カスタムソート \(数字 + Sort\)
通常のソートはID順に並べられますが、自分で好きに優先順位をつけられます。

数字キーを押しながら Sort ボタンをクリックすると、フィルターによって現在表示中のアイテム全てに押した数字キーに対応する優先順位をつけます。
優先順位は 1～9 キーで 1～9 を、0 キーで 10 を割り当てます。
デフォルトの優先順位は 7 です。

フィルターに`"pri:"+数字`を入力するとその優先順位がついたアイテムが検索されます。

#### 一括収納 \(Store（Shift キーで表示）\)
StoreInv ボタンで手持ち欄以外のインベントリ内のアイテムを、StoreEqp ボタンで手持ち欄のアイテムを全てチェストに収納します。

#### 一括排出 \(Eject（Shift キーで表示）\)
Eject ボタンで表示されているチェスト内の全てのアイテムをドロップします。
フィルタも有効です。

大量のアイテムによってワールドがフリーズするなどの問題を防ぐため、一度に排出できる量を制限しています。
この量はコンフィグで設定可能です。デフォルトでは 96 スタック（1 画面分）となっています。

#### 自動収納
アイテムを拾おうとしたとき、インベントリ内に Access Chest
を持っていれば、インベントリ内が一杯でも Access Chest 内に直接収納できます。

コンフィグファイルから無効にすることができます。

### レシピ

#### Access Chest
##### Access Chest Class-0 : チェスト + エンダーパール
![Access Chest Class-0](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeAccessChest0.png)
##### Access Chest Class-1 : Access Chest Class-0(8) + ラピスラズリブロック
![Access Chest Class-1](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeAccessChest1.png)
##### Access Chest Class-2 : Access Chest Class-1(8) + 金ブロック
![Access Chest Class-2](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeAccessChest2.png)
##### Access Chest Class-3 : Access Chest Class-2(8) + ダイヤモンドブロック
![Access Chest Class-3](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeAccessChest3.png)

#### Compressed Chest
##### Compressed Chest Class-1 : チェスト(8) + ダイヤモンド
![Compressed Chest Class-1](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeCompressedChest1.png)
##### Compressed Chest Class-2 : Compressed Chest Class-1(8) + ダイヤモンドブロック
![Compressed Chest Class-2](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeCompressedChest2.png)

#### コピーレシピ
##### Access Chest Class-1(2) : Access Chest Class-1 + エンダーチェスト
![Access Chest Class-1](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeCopy1.png)
##### Access Chest Class-2(2) : Access Chest Class-2 + エンダーチェスト(3)
![Access Chest Class-2](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeCopy2.png)
##### Access Chest Class-3(2) : Access Chest Class-3 + エンダーチェスト(8)
![Access Chest Class-3](http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/img/RecipeCopy3.png)

### コンフィグ

- ejectStackLimit : 一括排出で排出されるスタックの限界数を決めます。大量のアイテムでプログラムが固まる、といった問題がある場合は少なくしてください。
- rowsScroll : 1 回のホイールスクロールでどれだけページを移動させるかです。デフォルトでは 8 行（= 1 ページ）になっています。
- enableAutoCollect : 自動収納機能を有効にするかです。デフォルトでは有効になっています。

### 紹介動画

<script type="text/javascript" src="http://ext.nicovideo.jp/thumb_watch/sm18955909?w=490&h=307"></script><noscript><a href="http://www.nicovideo.jp/watch/sm18955909">【ニコニコ動画】【Minecraft】 Access Chest 【自作MOD紹介】</a></noscript>


サポート
--------
バグ、要望がありましたら[マインクラフト　非公式日本ユーザーフォーラム][forum]までご連絡ください。

### 最新バージョン対応について

この MOD は大規模とは言わずも、中規模に近い大きさになってしまったため、素早く対応するのは困難です。
[GitHub][]にてソースコードを公開していますので、修正にご協力いただけると幸いです。

### 過去のバージョン


謝辞
----
テクスチャを提供して頂きました the M さん、誠にありがとうございます。


[download]: http://dl.dropbox.com/u/77191991/MinecraftModding/AccessChest/release/
[forum]: http://forum.minecraftuser.jp/viewtopic.php?f=13&t=4123
[GitHub]: https://github.com/AtoCrafter/AccessChest
