# Portfolio Hub

Python バックエンドエンジニアを目指して制作している、フルスタックアプリのポートフォリオ一覧です。
各プロジェクトは**異なる学習テーマ**を持ち、設計・テスト・CI/CD・デプロイ・ドキュメントまで一貫して仕上げています。

すべてのプロジェクトで共通して意識していること:

- レイヤードアーキテクチャ（api → service → repository/external）
- 型安全（Python 型ヒント / TypeScript strict）
- テスト（pytest）と CI（GitHub Actions: Lint + Test + Build）
- Docker 対応・環境変数管理
- 統一した README とデモURL

---

## ✅ 公開済みプロジェクト

### 01. Task Management
タスク管理のCRUDアプリ。フルスタック開発の基礎（FastAPI + Next.js + Docker + CI/CD）を一通り実装。

- **テーマ**: CRUD / レイヤード設計 / CI/CD / Docker
- **技術**: FastAPI, SQLAlchemy, Next.js, TypeScript, Docker, GitHub Actions
- 🔗 [Demo](https://portfolio-01-task-management.vercel.app/) ・ [API Docs](https://portfolio-01-task-management.onrender.com/docs) ・ [Repository](https://github.com/momoka0925/portfolio-01-task-management)

### 02. Weather Dashboard
Open-Meteo API を利用した天気ダッシュボード。外部API連携と非同期・キャッシュ設計がテーマ。

- **テーマ**: 外部API連携 / 非同期通信 / キャッシュ抽象化 / DTO / エラー設計
- **技術**: FastAPI, httpx(async), Pydantic, Next.js, TypeScript, Docker
- 🔗 [Demo](https://portfolio-02-weather-dashboard.vercel.app/) ・ [API Docs](https://portfolio-02-weather-dashboard-api.onrender.com/docs) ・ [Repository](https://github.com/momoka0925/portfolio-02-weather-dashboard)

### 03. Expense Tracker
JWT認証とリレーショナルDB設計がテーマの支出管理アプリ。ユーザーごとのデータ分離を実装。

- **テーマ**: 認証(JWT Access+Refresh) / 認可・データ分離 / PostgreSQL / Alembic / Repository / Soft Delete / Pagination
- **技術**: FastAPI, SQLAlchemy 2.0, Alembic, PyJWT, bcrypt, PostgreSQL, Next.js, TypeScript, Docker
- 🔗 [Demo](https://portfolio-03-expense-tracker.vercel.app/) ・ [API Docs](https://portfolio-03-expense-tracker-api.onrender.com/docs) ・ [Repository](https://github.com/momoka0925/portfolio-03-expense-tracker)

---

## 🚧 今後の予定

| # | プロジェクト | 主な学習テーマ |
|---|---|---|
| 04 | URL Shortener | リダイレクト / UUID / Analytics |
| 05 | Inventory Management | リレーション / 在庫管理 / SQL |
| 06 | AI Chat Client | LLM API / Streaming / Prompt |
| 07 | PDF Summarizer | PDF解析 / AI要約 |
| 08 | Web Scraper Dashboard | スクレイピング / データ可視化 |
| 09 | RAG Knowledge Base | Embedding / Vector DB / Retrieval |
| 10 | Business Automation Platform | 認証 / AI / Background Task / 統合 |

---

## 🧰 共通基盤

- **デプロイ**: フロントは Vercel、APIは Render（Docker）。デプロイは共通スクリプトで自動化。
- **CI**: 各リポジトリで GitHub Actions（Lint / Test / Build）を実行。

> このリポジトリは各プロジェクトへの入口（ハブ）です。詳細は各リポジトリの README を参照してください。
