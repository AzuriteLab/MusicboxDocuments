# VRChat向けジュエリーボックス付きオルゴール取扱説明書

[TOP](index.md)

!!! EXPERIMENTAL !!!

## 構成

* `Audio`: サンプルの楽曲データが入っているディレクトリです
* `Texture`: テクスチャが入っているディレクトリです
* `MusicBox.fbx`: オルゴールのfbxファイルです
* `MusicBox.unitypackage`: オルゴールのunityパッケージです
* `README.txt`: 説明書です。ここへのリンクが載っています
* `LICENSE.txt`: ライセンスファイルです

一応fbxは添付していますが、`VRC_Trigger`などVRC SDKに依存した構造のもの & アニメーション設定済みのため、
改変すると一からの組み立て作業になってしまうので、テクスチャの編集やマテリアルの変更以外の改変は大変なのでお勧めしません…

## 使い方

`MusicBox.unitypackage` をUnityのProjectへImportします。
Import前にVRC SDKを取り込んでいないと組み込んである `VRC_Trigger` 類のコンポーネントがロードされませんので、ご注意ください。

その中の `MusicBox.prefab` を `Hierarchy` にドロップすると、`MusicBox_Production`というゲームオブジェクトが生成されます。

これを好きなように配置するだけで使えるようになります。
曲を変更する場合は、[自分の好きな曲を設定する方法](customize.md) を参照してください。

---

Copylight(c) 2019 Azurite
