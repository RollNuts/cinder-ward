# Asset Intake Policy（Issue #7）

本リポジトリのアセット追加は、Steam 向け商用品質の 2D HD ダークファンタジーゲームを前提に実行する。  
最終判断は公開リスクを最小化し、ゲーム品質を担保できることを優先する。

## 1) 許可ソース

### 基本方針
- 優先順位: **CC0 > 商用可ライセンス（明確な条件付き） > 事前承認で追加生成**。
- CC BY 系は可だが、配布時のクレジット義務を厳守すること。
- NC / ND / Editorial / 不明ライセンスは原則禁止。

### 受け入れ可能なソース
- **Aseprite / PixelOver / Blender / Maya**  
  自前制作、または権利元が明確な素材を組み込んだ制作物として扱う。
- **Poly Haven**  
  **CC0 前提**で、背景・下地画像として受け入れ。取り込んだ資産と紐づく公開URLを必ず保存。
- **Mixamo（Adobe）**  
  Adobe FAQ 上のゲーム商用品利用可を根拠に、主にポーズ/アニメ下地として受け入れ。  
  キャラクター本体素材やモデル自体は二次利用条件を再確認して ledger へ記録する。
- **自前制作済み資産（外部フリー素材非依存）**  
  制作者・生成情報・利用範囲を明示すれば受け入れ対象。

## 2) 禁止 / 要承認ソース

- **Maya 付属素材**  
  商用利用条件が明確でないものは本番使用禁止。  
  条件が確認できれば、`license_ok = true` と承認担当確認のうえでのみ使用。
- **Sketchfab / Fab**  
  個別ライセンスが明記され、該当ライセンス本文の URL 付き確認が取れた場合のみ許可。  
  `CC0` / `CC BY` / `Fab Standard License` など、商用利用と改変が明示されたものだけを許容し、必要なクレジット台帳要件を満たすこと。
- **Meshy / 有料生成 API / paid endpoint**  
  事前承認フォーム未提出・未承認は使用禁止。
- **NC / ND / Editorial / no-commercial / 不明ライセンス**  
  いずれも禁止。
- **再配布不可素材の外部生データ**  
  取り込み済みでも ledger に根拠を置けない場合は即時ブロック。

## 3) ライセンス台帳（ledger）必須項目

アセット intake 時に次の項目を台帳（`docs/asset_license_ledger.md` など）に記録する。

1. `asset_id`（ユニークID）
2. `asset_name`
3. `asset_type`（3D / Sprite / Texture / Audio / etc.）
4. `source`（取得元）
5. `source_url`
6. `source_version_or_tag`
7. `author_or_vendor`
8. `license_name`
9. `license_url`
10. `license_summary`（商用可・改変可など）
11. `credit_required`（true/false）
12. `credit_text`（必要時のみ）
13. `commercial_allowed`（true/false）
14. `nc_nd_editorial_forbidden`（true/false、再確認ポイント）
15. `approved_by`
16. `approval_date`
17. `intake_status`（approved / blocked / rejected / archive）
18. `review_notes`（要注意事項）
19. `conversion_path`（3D->PixelOver->Aseprite など）
20. `storage_path`（本番/再利用/Archive の実体パス）

## 4) 3D → PixelOver → Aseprite の受け入れフロー

### 4-1. 3D元データ準備（Blender / Maya）
- ポリゴン・UV・材質の品質を確認。
- 著作権上不明なテクスチャやリグは混在させない。
- ライセンス条件が曖昧な素材を含む場合はブロック（Maya付属含む）。

### 4-2. PixelOver 変換
- 参照元3Dを PixelOver 用に最小限整形して書き出し。
- 生成ログと実行パラメータを保存（時間、解像度、モード、フレーム設定）。
- 2Dベース画像を素材群として保存。

### 4-3. Aseprite 統合作業
- PixelOver 出力をAsepriteで
  - 境界処理
  - ディティール調整
  - Steam配布前提の 2D-HD 可読性最適化
  - 必要ならパレット再設計
  - 規定タグ・命名規則を付与  
  したのち、最終候補として `approved` 判定対象へ送る。

### 4-4. 最終登録
- ledger を更新し、PR に添付する。
- `commercial_allowed` と `credit_required` が一致しない場合は PR 不可。

## 5) 失敗・差し戻し資産の保存ルール

- 生成失敗、審査差し戻し、方針不適合など理由の有無に関わらず、削除禁止。
- 必ず `archive/rejected` 配下へ移動保存する。
- 保存先例:
  - `Assets/Art/archive/<date>-<asset_id>/` … 未採用（保留）  
  - `Assets/Art/rejected/<date>-<asset_id>/` … 承認不可
- `notes.md` または `meta.txt` に
  - 取得元URL
  - 判定日
  - 差し戻し理由
  - レビュー担当
  を残す。

## 6) 有料/API生成利用申請フォーム（事前承認）

有料/API生成を使う前に、以下テンプレートで承認申請し、`license_review` として添付する。

- 申請ID:
- 申請日:
- 申請者:
- 利用サービス（モデル名）:
- 目的（背景/モーション/スプライト等）:
- 入力プロンプト・制約:
- 予算上限 / 試行上限:
- 出力保存場所（生成成功時）:
- 失敗時保存場所（失敗時）:
- 想定コマーシャル適用可否（Yes/No）:
- 商用再利用条件の確認方法:
- 承認者:
- 承認日:

## 7) アセット追加 PR チェックリスト

- [ ] Asset Intake Policy の対象カテゴリ確認（許可/要承認/禁止）
- [ ] ライセンス台帳に必須項目がすべて入力済み
- [ ] CC BY は credit_text を含むこと
- [ ] NC / ND / Editorial / 不明は混在していないこと
- [ ] 3D→PixelOver→Aseprite 経路の場合、各中間処理ログあり
- [ ] 失敗・差し戻しアセットは `archive/rejected` へ保存
- [ ] 有料/API生成は事前承認フォーム完備（該当なしの場合は明示）
- [ ] スクリーンショット・レビュー履歴を PR 描画内に添付
