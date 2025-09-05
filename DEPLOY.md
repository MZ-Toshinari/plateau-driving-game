# デプロイ手順

## GitHub Pagesでのデプロイ

1. GitHubアカウントにログイン
2. 新しいリポジトリを作成:
   - Repository name: `plateau-driving-game`
   - Public に設定
   - README.md は追加しない

3. ローカルリポジトリをプッシュ:
```bash
cd /home/toshinari-sone/plateau-driving-game
git remote add origin https://github.com/YOUR_USERNAME/plateau-driving-game.git
git branch -M main
git push -u origin main
```

4. GitHub Pages設定:
   - リポジトリの Settings タブ
   - Pages セクション
   - Source: Deploy from a branch
   - Branch: main / (root)
   - Save

5. アクセスURL:
   `https://YOUR_USERNAME.github.io/plateau-driving-game/`

## 代替デプロイ方法

### Netlify Drop
1. https://app.netlify.com/drop にアクセス
2. `/home/toshinari-sone/plateau-driving-game` フォルダをドラッグ&ドロップ
3. 自動生成されるURLでアクセス可能

### Vercel
1. https://vercel.com にアクセス
2. GitHubリポジトリを連携
3. 自動デプロイ完了

## ファイル構成
```
plateau-driving-game/
├── index.html (メインゲームファイル)
├── README.md
└── DEPLOY.md
```
