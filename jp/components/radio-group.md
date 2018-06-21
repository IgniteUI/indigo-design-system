﻿---
title: Radio Group -  デザイン システム コンポーネント
_description: Radio Group コンポーネント シンボルは、一連のオプションで排他的な選択のメカニズムを提供します。
_keywords: デザイン システム, Sketch, Ignite UI for Angular, コンポーネント, UI ライブラリ, ウィジェット
_language: ja
---

## Radio Group

Radio Group コンポーネント シンボルは、グループ項目で排他的な選択をサポートします。グループの項目は、左揃えで単一列に次々にレイアウトされます。Radio Group は、[Ignite UI for Angular Radio Button コンポーネント](https://jp.infragistics.com/products/ignite-ui-angular/angular/components/radio_button.html)と視覚的に同じものです。

### Radio Group デモ

![](../images/radiogroup_demo.png)

### テーマ

Radio Group は、明暗バリアントでわかりやすく、背景に明暗のコントラストを付けてスタイル設定できます。すべての Radios を同じテーマに設定してださい。

![](../images/radiogroup_dark.png)
![](../images/radiogroup_light.png)

### 状態

グループの各 Radio は、**オン**とオフ、そして追加のバリアントとしてインタラクション無効の状態があります。

![](../images/radiogroup_states.png)

### スタイル設定

Radio Group は、さまざまなオーバーライドで各項目のラベル スタイルや色を制御することにより柔軟にスタイル設定できます。

![](../images/radiogroup_styling.png)

## 使用方法

Radio Group を追加項目で拡張する場合は、単一列で左寄せに統一してください。複数列のレイアウトや Radio を一度に 1 つ以上オンにしないようにします。

| いい例                                | 悪い例                               |
| --------------------------------- | ----------------------------------- |
| ![](../images/radiogroup_do1.png) | ![](../images/radiogroup_dont1.png) |
| ![](../images/radiogroup_do2.png) | ![](../images/radiogroup_dont2.png) |

## コードの生成

Radio Group の色やフォントを指定した場合、Radio Group HTML 要素は div でラップされます。ブラウザーによってネスト コンポーネント (他のコンポーネント内のコンポーネント) のスタイル設定が要求されます。

> [!WARNING]
> Radio Group のインスタンスで`シンボルからデタッチ`をトリガーした場合、Radio Group のコード生成の精度を低下します。提供された項目以上に項目を作成する場合のみ行います。`🚫radio-group`、`🕹️DataProperty`、`🕹️DataSource` レイヤー インタクトを保持してください。
 
### データ バインディング

データ バインディングは波括弧構文によって指定されます。例: {isAdmin}。テキスト フィールド (`🕹️DataProperty` および `🕹️DataSource` 以外) も文字列補間構文をサポートします。例: 管理者: {isAdmin}。データ バインディングはネストまたはネストなしが可能です。ターゲット プロパティがネストされたプロパティの場合、ネストされたプロパティ チェーンを含みますがモデル オブジェクト名は含みません。実例:

#### ネストなし

```PseudoCode
Customer {
    imageName: String;
}

DataProperty: {imageName}
```

#### ネストあり

```PseudoCode
Profile {
    imageName: String;
}

Customer {
    profile: Profile;
}

DataProperty: {profile.imageName}
```

### リアクティブ フォーム

モデル オブジェクト名および `🕹️DataProperty` が提供される場合、Reactive Forms フォームを作成するためにフォーム ビルダー コードで TypeScript ngOnInit メソッドが生成されます。`🕹️DataProperty` はラジオ ボタン コントロールの formControlName プロパティを設定します。

### DataProperty

`🕹️DataProperty` 値は Angular Reactive Forms を使用してラジオ ボタンの checked プロパティへの 2-way データ バインディングを設定するために使用されます。`🕹️DataProperty` はオプションです。`🕹️DataProperty` は、生成要求で提供されるモデル オブジェクト名で指定されたデータ オブジェクトのプロパティ名です。

### DataSource

提供される場合、`🕹️DataSource` 値が Radio Group のデータ ソース オブジェクトへのバインディングを設定するために使用されます。デフォルトで Radio Group ボタンの値およびラベルに割り当てる value および name プロパティがあるデータ ソースにバインドするために構成されます。`🕹️DataSource` プロパティはオプションです。

`🕹️DataSource` が設定される場合、スタイルはグループの最初のラジオから取得されます。その他の Radio Button スタイル設定が無視されます。`🕹️DataSource` が使用される場合、Text プロパティも無視されます。

### ラジオ ボタン

グループの Radio Button の設定を決定します。`🕹️DataSource` を設定し、最初の Radio Button が None の場合、ラジオ グループは描画しません。Radio Button が None の場合、Radio Button を描画しません。Radio Button の Color が None の場合、Radio Button を描画しません。3 つの Radio Button がすべて None の場合、Radio Group を描画しません。

### テキスト

`🕹️DataSource` を設定した場合、Text プロパティは無視されます。Text が提供される場合、Radio Button の値およびラベルで使用されます。

## その他のリソース

関連トピック:

コミュニティに参加して新しいアイデアをご提案ください。

- [Indigo Design **GitHub** (英語)](https://github.com/IgniteUI/design-system-docfx)