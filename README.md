# Nall4 — Discord Bot

Bot de análise financeira para Discord com arquitetura hexagonal, LangGraph e Gemini.

## O que faz

- `/analisar [ticker]` — análise completa de qualquer ativo BR ou US
- `/carteira [tickers]` — resumo da carteira com múltiplos ativos
- `/relatorio` — relatório semanal sob demanda
- Mensagem livre → conversa com o agent sobre mercado

## Stack

- Python 3.11+
- LangGraph + Gemini API (agent e síntese)
- BRAPI (ações BR, FIIs, dividendos)
- yfinance (ações US e globais)
- discord.py (interface)
- SQLite + aiosqlite (memória de conversa)
- APScheduler (relatório semanal automático)
- Railway (deploy)

## Arquitetura

Hexagonal (Ports & Adapters) com SOLID aplicado em cada camada.