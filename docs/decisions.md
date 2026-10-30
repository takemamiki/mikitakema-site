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

### 公開（完了）
- リポジトリ mikitakema-site を Public にし、GitHub Pages で公開
- http://mikitakema.com で表示されることを確認
- HTTPS 化は証明書発行待ち（10/29 時点）

### サイトの中身
- 自己紹介文は「音楽も、エッセイも、業務ツールも。作り続ける人です。」で始まる B案でいったん決定（10/28）
- 問い合わせは X の DM へ誘導する
- X などでリンクを告知するのは、プロフィール文が決まってから（10/30）