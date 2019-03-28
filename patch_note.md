# VRChat向けジュエリーボックス付きオルゴール取扱説明書

[TOP](index.md)

## 変更履歴

### ver 2019.03.27.0

* オルゴールの設計変更
 * 外箱とオルゴール機構本体を分離（元々2メッシュ構成のため負荷は変わらないはずです）
 * 外箱がオルゴール機構を内包する構造になりました
 * 曲を鳴らす部分を `VRC_Audio Bank` に変更しました
  * この変更により曲の入れ替えが1パスで済み、曲の途中停止ができるようになりました
  * ゼンマイ音を鳴らす部分は `AudioTrigger` のままです
* 新しい設計のオルゴールを再配置
 * MusicBox.fbx: 宝石箱単体のFBXファイルになりました
 * MusicBox.prefab: 宝石箱と機構を統合し、各種Trigger設定済みのprefab（G線上のアリア）
 * MusicBox_Original.prefab: 宝石箱と機構を統合し、各種Trigger設定済みのprefab（オリジナル曲）
 * 旧版のオルゴールは一応残しており、Importしたディレクトリ下に`./OLD/`、`./FBX/OLD/` ディレクトリがあり、その中に格納されています
* 分離したオルゴール機構本体の追加
 * MusicBoxDrivingMechanism.fbx: 本体のFBXファイル
 * MusicBoxDrivingMechanism.prefab: 本体単体で駆動する各種Triggerを組み込み済みのprefab（G線上のアリア）
 * MusicBoxDrivingMechanism_Original.prefab: 本体単体で駆動する各種Triggerを組み込み済みのprefab（オリジナル曲）
* 新しいタイプのオルゴールを追加
 * ModernMusicBox.fbx: 外箱のFBXファイル
 * ModernMusicBox.prefab: 外箱と機構を統合し、各種Trigger設定済みのprefab（G線上のアリア）
 * ModernMusicBox_Original.prefab: 外箱と機構を統合し、各種Trigger設定済みのprefab（オリジナル曲）

---

Copylight(c) 2019 Azurite
