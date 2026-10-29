# decisions.md（mikitakema-site の決定事項）

## 2026-10-29 独自ドメイン接続

### ドメインの所有確認（完了）
- GitHubアカウント（takemamiki）で mikitakema.com を検証済み（Verified）
- Cloudflare DNS に TXTレコード `_github-pages-challenge-takemamiki` あり
  - **削除禁止**（消すと検証が外れ、乗っ取り対策が無効になる）
  - Cloudflare側のレコードにも同じ内容のコメントを記入済み

### カスタムドメイン設定（完了）
- リポジトリの Settings → Pages → Custom domain に mikitakema.com を設定
- リポジトリ直下の CNAME ファイル（中身: mikitakema.com）は**削除・編集禁止**
  - GitHubが自動で作ったファイル。消すとドメイン設定が外れる