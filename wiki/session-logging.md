# Session Logging

Sistema de logs de conversas com push automático para o repositório GitHub.

## Como Funciona
- Cada sessão gera ou atualiza um arquivo `session-logs/YYYY-MM-DD.md`
- Um cron job executa diariamente às 23:30 (UTC-3) e faz commit + push
- O script também verifica mudanças em `wiki/` e `raw/`

## Cron Job
- **ID:** `c2ee0ce14534`
- **Schedule:** `30 2 * * *` (23:30 UTC-3)
- **Entrega:** Local (salva em `~/.hermes/cron/output/`)

## Script
```bash
bash /home/user/scripts/session-log-push.sh
```
- `git pull --rebase` antes de adicionar
- `git add` em session-logs/, wiki/, raw/
- Só faz commit se houver mudanças
- `git push origin main`

## Formato do Log
- Headers com data, usuário, hora de início
- Resumo executivo
- Histórico detalhado por tópicos
- Tabela de status ao final
- Markdown puro, legível no GitHub

---

*Relacionado: [[github-workspace]], [[WIKI_SCHEMA]]*
