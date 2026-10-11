# Kensho Datasets

日本の市場データを週次で公開する配布専用リポジトリです。

- **Anime Figure Prices** — アニメフィギュア価格のスナップショット（毎週月曜）
- **MLIT Property Prices** — 国土交通省 不動産取引価格（別リポジトリ `mlit-property-prices-mcp`）

## データセット一覧

| データセット | 説明 | 最新リリース |
|-------------|------|-------------|
| **Anime Figure Prices** | アニメフィギュア価格のスナップショット（毎週月曜更新） | [2026-W41](https://github.com/atushi1841/kensho-datasets/releases/tag/weekly/2026-W41) |
| **MLIT Property Prices** | 国土交通省 不動産取引価格 | [mlit-property-prices-mcp](https://github.com/atushi1841/mlit-property-prices-mcp) |

## 使用方法

### GitHub Releases からダウンロード

```bash
# 最新リリース取得
gh api repos/atushi1841/kensho-datasets/releases/latest

# 週次リリース一覧
gh api repos/atushi1841/kensho-datasets/releases | jq '.[] | {tag_name, name}'
```

### Apify Actor 経由で取得

- [Anime Figure Prices Scraper](https://apify.com/atushi1841/anime-figure-prices-scraper)
- [Yahoo Auctions Japan Scraper](https://apify.com/atushi1841/yahoo-auctions-japan-scraper)
- [Mercari Japan Scraper](https://apify.com/atushi1841/mercari-japan-scraper)

## ライセンス

MIT
