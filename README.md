# AI-oss-Japanese

日本語圏のAI/OSSコミュニティ向けプロジェクト。実運用を想定したモデル・評価・配布の標準パターンを提供します。

<!-- badges -->
[![CI](https://img.shields.io/badge/CI-GitHub_Actions-informational)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## Features
- 実装と評価の**分離**（`src/` と `eval/`）
- **再現可能**な環境（Docker / devcontainer / lockfile）
- Lint / Type check / Test を**PR必須**（Actions）
- Discord / GitHub のイベント連携（Webhook）

## Requirements
- Python 3.10+（uv / poetry いずれか）
- (任意) Docker 24+ / docker compose

## Quickstart
### Local (uv)
```bash
uv venv && source .venv/bin/activate
uv pip install -r requirements.txt
pytest -q
<!-- feature/ad-agent-init: 広告運用エージェント開発の初期構築ブランチ -->
