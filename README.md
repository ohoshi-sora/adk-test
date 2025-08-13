# マルチエージェントシステム構築技術検証

## 概要

Google ADK（Agent Development Kit）を使用したマルチエージェントシステムの構築について技術検証を行っています。複数のエージェントが協調してタスクを実行するシステムを作ることを目的としています。

## 背景

マルチエージェントシステムは、複数の自律的なエージェントが協調して複雑なタスクを解決するシステムです。近年のAI技術の発展により、大規模言語モデル（LLM）を活用したエージェントの実装が注目されています。

## 技術スタック

- **Google ADK**: Googleが提供するエージェント開発キット
- **Python 3.10**: メインの開発言語
- **FastAPI**: Web APIフレームワーク
- **Uvicorn**: ASGIサーバー
- **Google Cloud AI Platform**: AIサービス基盤
- **Gemini 2.5 Flash**: 大規模言語モデル

## プロジェクト構成

```
adk-test/
├── .gitignore         
├── .venv/             
├── multi_tool_agent/   # マルチツールエージェント実装
│   ├── __init__.py
│   └── agent.py        # エージェント定義
└── README.md           
```

## セットアップ手順

### 1. 環境構築

```bash
# Python仮想環境の作成
python3 -m venv .venv

# 仮想環境のアクティベート
source .venv/bin/activate

# 依存関係のインストール
pip install google-adk
```

### 2. Google ADKの起動

```bash
# ADK Webサーバーの起動
adk web
```

サーバーが起動すると、ブラウザで `http://localhost:8000` にアクセスできます。


## 現在の進捗

- [x] プロジェクト環境の構築
- [x] Google ADKのインストール
- [x] 基本的なエージェントの実装
- [x] Web UIでの動作確認
- [ ] マルチエージェント連携の実装
- [ ] パフォーマンステスト



## 参考文献

- [Google ADK Documentation](https://developers.google.com/adk)

*最終更新: 2025年8月14日*
