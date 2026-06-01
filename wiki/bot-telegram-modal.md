# Telegram Bot com Modal

Bot inteligente (`hermes_erobeng_bot`) rodando em GPU serverless via Modal.

## Arquitetura
- **Plataforma:** Modal (serverless GPU)
- **Framework:** FastAPI com webhook
- **Modelo:** Phi-3-mini-4k-instruct (quantização 4-bit)
- **GPU:** T4
- **App name:** `telegram-intelligent-bot`
- **Secret:** `telegram-bot-token`

## URLs
- **Webhook:** `https://erisonbarros--telegram-intelligent-bot-fastapi-app.modal.run/webhook`
- **Chat ID:** 1452127804

## Configuração
- Token do bot via Modal Secrets (`telegram-bot-token`)
- Bot local usa `uv` para gestão de pacotes (pip/pip3 indisponíveis)
- Projeto em `/home/user/telegram_modal_bot/`

## Cron Jobs
- **Mensagem de boas-vindas diária:** 7:00 UTC (usa o cronjob do Hermes)

## Status
- ✅ Bot rodando com modelo rule-based local
- ✅ Deploy Modal em produção

---

*Relacionado: [[telegram-bot-config]], [[perfil-profissional]]*
