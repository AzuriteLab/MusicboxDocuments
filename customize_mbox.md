# VRChat向けジュエリーボックス付きオルゴール取扱説明書

[TOP](index.md)

## オルゴールそのものの改変方法

プリセットでは木製の宝石箱タイプとお休みさんのガラスシェーダが適用された2つのバリエーションがあります。
しかし、オルゴール自体の改変を簡易にするために、機構を分離したprefabを用意しています。

この頁ではそのprefabを用いた新たなバリエーションを追加する方法を解説します。

### 外箱のゲームオブジェクトをHierarchyに作成する

ご自身で制作された（またはどこかにあった）外箱のFBXやprefabをHierarchyにドロップしてゲームオブジェクトを作成します。
ここではプリセットにある `ModernMusicBox.fbx` を取り込んでいます。

### オルゴール機構のゲームオブジェクトをHierarchyに作成する

`MusicBoxDrivingMechanism.prefab` をHierarchyにドロップし、オルゴール機構のゲームオブジェクトを生成します。

### オルゴール機構をケースのゲームオブジェクト内に内包させる

前項で生成された `MusicBoxDrivingMechanism` ゲームオブジェクトを外箱のゲームオブジェクト直下に配置します。

そして、`MusicBoxDrivingMechanism` ゲームオブジェクトの位置を外箱基準で合わせます

これで改変は完了です。

宝石箱のような蓋の開閉と再生機構を連携させる方法は中級者向きのため、`MusicBox.prefab` の中身を参考にしてください。
`MusicBox`の`VRC_Trigger`と、`MusicBoxDrivingMechanism`の`VRC_Trigger`同士で`SetGameObjectActive`アクションにてオブジェクトの
on/offを行うことによって実現しています。

---

Copylight(c) 2019 Azurite
