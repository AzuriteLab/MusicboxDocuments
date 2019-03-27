# VRChat向けジュエリーボックス付きオルゴール取扱説明書

[TOP](index.md)

## 構成

```
.-- Audio
 |  |- G_AIR.wav : サンプル曲 G線上のアリア
 |  `- JewelryBox.wav : サンプル曲 JewelryBox
 |- Texture
 |  |- MusicBox2k : 2Kテクスチャ類（非推奨）
 |  `- MusicBox4k : 4Kテクスチャ類（推奨）
 |- MusicBox.unitypackage : Unityパッケージ
 |- MusicBox_Production.fbx : FBXファイル
 |- README.txt : このファイル 
 `- LICENSE.txt : ライセンスファイル
```

一応fbxは添付していますが、`VRC_Trigger`などVRC SDKに依存した構造のもの & アニメーション設定済みのため、
改変すると一からの組み立て作業になってしまうので、テクスチャの編集やマテリアルの変更以外の改変は大変なのでお勧めしません…

## 使い方

`MusicBox.unitypackage` をUnityのProjectへImportします。
Import前にVRC SDKを取り込んでいないと組み込んである `VRC_Trigger` 類のコンポーネントがロードされませんので、ご注意ください。

![product](images/description/product.png "product")

その中の `MusicBox_Production.prefab` を `Hierarchy` にドロップすると、`MusicBox_Production`というゲームオブジェクトが生成されます。

![hierarchy](images/description/hierarchy.png "hierarchy")

これを好きなように配置するだけで使えるようになります。
曲を変更する場合は、[自分の好きな曲を設定する方法](customize.md) を参照してください。

`MusicBox_Production_Original.prefab` というprefabもありますが、これはわたしのオリジナル曲をあらかじめ設定したものです。

## ジュエリーボックスの扱いについて

赤い部分はジュエリーボックスになっていますので、Unity上でアクセサリのオブジェクトをいい感じに配置してそれっぽく見えるようにするといいかんじです。

---

Copylight(c) 2019 Azurite
