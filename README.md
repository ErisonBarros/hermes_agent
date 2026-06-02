# 🤖 hermes_agent

> **AI-powered workflows for geospatial data, automation, and research reproducibility**

Repositório pessoal do **Prof. Erison Barros** para gestão de conhecimento, automação de fluxos de trabalho geoespaciais e logs de sessões do Hermes Agent.

[![License](https://img.shields.io/badge/license-Private-red.svg)]()
[![Maintained](https://img.shields.io/badge/maintained-yes-brightgreen.svg)]()
[![GitHub](https://img.shields.io/badge/github-ErisonBarros-blue.svg)](https://github.com/ErisonBarros)

---

## 📋 Sobre o Repositório

Este repositório funciona como uma **base de conhecimento pessoal** mantida pelo Hermes Agent, um assistente de IA que auxilia em workflows geoespaciais, pesquisa acadêmica, automação de tarefas e reprodutibilidade científica.

### 🎯 Objetivos

- **Centralizar** documentação, scripts e logs de atividades do Hermes Agent
- **Versionar** o conhecimento pessoal e profissional do Prof. Erison Barros
- **Automatizar** fluxos de trabalho relacionados a topografia, cartografia e geotecnologias
- **Documentar** sessões de trabalho, projetos em andamento e referências úteis

---

## 📂 Estrutura do Repositório

```
hermes_agent/
├── README.md                  # Este arquivo (visão geral do repo)
├── WIKI_SCHEMA.md             # Schema operacional do knowledge base
├── .gitignore                 # Arquivos ignorados pelo Git
│
├── raw/                       # 📥 Documentos-fonte (imutáveis)
│   └── cv-prof-erison.txt     # Currículo acadêmico completo
│
├── session-logs/              # 📅 Logs diários de sessões
│   ├── 2026-05-31.md          # Log da sessão de 31/05/2026
│   ├── 2026-06-01.md          # Log da sessão de 01/06/2026
│   └── token-consumption-2026-06-01.md  # Relatório de consumo de tokens
│
└── wiki/                      # 📚 Knowledge Base (gerenciado pelo LLM)
    ├── index.md               # Índice organizado por categoria
    ├── log.md                 # Registro cronológico de operações
    ├── perfil-profissional.md # Perfil acadêmico e profissional
    ├── bot-telegram-modal.md  # Projeto: Bot Telegram com Modal
    ├── github-workspace.md    # Configuração do workspace GitHub
    └── session-logging.md     # Sistema de logs automatizados
```

---

## 🔍 Detalhamento das Pastas

### 📥 `raw/` — Documentos-Fonte
Armazena **documentos originais** que servem como entrada para o knowledge base. Estes arquivos são **imutáveis** (read-only) e representam a "fonte da verdade" das informações.

| Arquivo | Descrição |
|---------|-----------|
| `cv-prof-erison.txt` | Currículo Lattes expandido do Prof. Erison Barros |

### 📅 `session-logs/` — Logs de Sessões
Registros **diários** de atividades realizadas com o Hermes Agent. Cada arquivo documenta:
- Ações executadas
- Arquivos criados/modificados
- Status de tarefas
- Commits e pushes realizados

| Arquivo | Conteúdo |
|---------|----------|
| `YYYY-MM-DD.md` | Log narrativo da sessão |
| `token-consumption-YYYY-MM-DD.md` | Relatório quantitativo de uso de tokens |

### 📚 `wiki/` — Knowledge Base
**Núcleo do repositório.** Páginas Markdown geridas pelo LLM seguindo o schema definido em [`WIKI_SCHEMA.md`](./WIKI_SCHEMA.md). Organizado em:

- **Perfis** — Informações pessoais e profissionais
- **Projetos** — Documentação de projetos em andamento
- **Conceitos** — Definições, glossários, referências técnicas
- **Ferramentas** — Configurações de software, APIs, serviços
- **Fontes** — Referências cruzadas aos documentos em `raw/`

O arquivo [`wiki/index.md`](./wiki/index.md) funciona como **catálogo navegável** de todas as páginas.

---

## ⚙️ Como o Repositório é Mantido

### 🔄 Workflow de Ingestão
Quando um novo documento é adicionado em `raw/`:
1. O Hermes Agent lê e extrai conceitos-chave
2. Cria/atualiza páginas em `wiki/` com resumos estruturados
3. Atualiza `wiki/index.md` com as novas entradas
4. Registra a operação em `wiki/log.md`

### 🔄 Workflow de Query
Quando o usuário faz uma pergunta:
1. O Agent busca em `wiki/index.md` por páginas relevantes
2. Lê e sintetiza respostas com citações
3. Pode gerar novas páginas se a síntese agregar valor

### 🔄 Push Automatizado
Os logs de sessão são sincronizados automaticamente com este repositório via **cron job** agendado para **23:30 (UTC-3)** diariamente.

---

## 🛠️ Tecnologias e Ferramentas

| Categoria | Ferramenta | Uso |
|-----------|-----------|-----|
| **IA/ML** | Hermes Agent, Phi-3-mini-4k-instruct, Gemini | Assistente conversacional, geração de conteúdo |
| **Deploy** | Modal (serverless GPU) | Hospedagem de bots e calculadoras |
| **Versionamento** | Git + GitHub | Controle de versão, backup, colaboração |
| **Documentação** | Markdown + Obsidian | Knowledge base, notas pessoais |
| **Geotecnologias** | QGIS, AutoCAD, CloudCompare | Topografia, cartografia, fotogrametria |
| **Comunicação** | Telegram Bot API | Interação com alunos e grupos |

---

## 📊 Estatísticas

- **📅 Início do tracking:** Maio/2026
- **📚 Páginas no wiki:** 6+
- **📥 Documentos-fonte:** 1 (CV completo)
- **🤖 Projetos ativos:** Bot Telegram com Modal
- **⏰ Push automático:** Diário às 23:30 UTC-3

---

## 🔗 Links Úteis

### Perfis Acadêmicos
- 🎓 [ORCID](https://orcid.org/0000-0003-4879-6880)
- 📄 [Lattes](http://lattes.cnpq.br/8237482217038157)
- 🏛️ [Labat](https://sites.google.com/view/labat/01)
- 🐍 [Python Book](https://erisonbarros.github.io/bookpython_ufpe/docs/index.html)

### Web Presence
- 💼 [GitHub](https://github.com/ErisonBarros)
- ✍️ [Blog](https://proferisonbarros.blogspot.com/)
- 📝 [Hashnode](https://erisonbarros.hashnode.dev/)
- 🌐 [Website UFPE](https://erobeng.wixsite.com/ufpe)

### Instituições
- 🏛️ [UFPE - DECART](https://www.ufpe.br/decart)
- 📋 [Coordenação de Estágio DECART](https://sites.google.com/view/coordenacaoestagiodecart/)

---

## 📝 Convenções

- **Commits:** Mensagens descritivas em português, prefixo por tipo (Add, Update, Fix, Remove)
- **Markdown:** Padrão GitHub Flavored Markdown
- **Wiki pages:** Links relativos para navegação interna
- **Session logs:** Formato narrativo + tabelas de status
- **Tokens:** Estimativa baseada em 1 token ≈ 4 caracteres

---

## 🤝 Contribuições

Este é um repositório **privado e pessoal**. Sugestões de melhorias no schema ou na organização são bem-vindas via issues.

---

## 📜 Licença

Conteúdo de uso pessoal e acadêmico. Documentos em `raw/` pertencem aos seus respectivos autores.

---

<p align="center">
  <em>Mantido por <a href="https://github.com/ErisonBarros">@ErisonBarros</a> com auxílio do <strong>Hermes Agent</strong></em><br>
  <em>Última atualização: 2026-06-01</em>
</p>
