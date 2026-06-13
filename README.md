# M.E.R.A.K.I
### Modular Emergent Reasoning Architecture with Kinetic Intelligence

Sistema de Inteligência Artificial independente, construído do zero.
Sem APIs de raciocínio externas. Sem modelos pré-treinados no núcleo.

---

## Estrutura da pasta

```
meraki/
│
├── iniciar.py            ← COMECE AQUI
│
├── Core — Base de conhecimento
│   ├── conceitos.py      fundação: Dimensao, Conceito, Relacao, BaseConhecimento
│   ├── compositor.py     motor de composição semântica + física do mundo
│   ├── semente.py        conhecimento inicial manual (65 conceitos, 60 relações)
│   └── config.py         loader central de configuração
│
├── Cognição — Raciocínio
│   ├── nucleo.py         4 módulos cognitivos + síntese + avaliador integrado
│   ├── memoria.py        5 sistemas de memória (M1–M5)
│   ├── avaliador.py      métricas automáticas de qualidade
│   └── analisador_m4.py  metacognição emergente por correlação estatística
│
├── Aprendizado — Crescimento autônomo
│   ├── pesquisador.py    crawler Wikipedia PT+EN com retry e rate limit
│   ├── professor.py      treino via LLMs gratuitos (Groq + Gemini)
│   └── agenda_pesquisa.py pesquisa sob demanda síncrona e assíncrona
│
├── Interface
│   └── nova.py           terminal interativo com comandos /historico /buscar /m4
│
└── Configuração
    ├── config.json       todos os parâmetros do sistema
    ├── requirements.txt  dependências Python
    └── .env.exemplo      template das chaves de API (copiar para .env)
```

---

## Início rápido

**1. Instalar dependências:**
```bash
pip install -r requirements.txt
```

**2. Iniciar (verificação automática de ambiente):**
```bash
python iniciar.py
```

**3. Ou iniciar direto:**
```bash
python nova.py
```

---

## Comandos no terminal

| Comando | Descrição |
|---|---|
| `/status` | Estado completo de todos os sistemas |
| `/buscar <termo>` | Consulta um conceito na base (M2) |
| `/historico` | Últimas 10 mensagens da sessão |
| `/feedback` | Avalia a última resposta (👍/👎) |
| `/m4` | Relatório de autoconhecimento emergente |
| `/pesquisar` | Liga/desliga o crawler em background |
| `/aprender` | Ensina um fato manualmente |
| `/verbose` | Mostra perspectivas dos 4 módulos |
| `/novo` | Inicia novo chat |
| `/sair` | Encerra |

---

## Treino com o Professor

O Professor usa LLMs gratuitos para ensinar conceitos com muito mais
qualidade que o crawler (~95% de precisão vs ~40% do crawler).

**Configurar (uma vez):**
1. Copie `.env.exemplo` para `.env`
2. Obtenha chave grátis em `console.groq.com`
3. Preencha `GROQ_API_KEY=sua_chave`

**Usar:**
```bash
# Conceitos diretos
python professor.py "fotossíntese" "democracia" "algoritmo"

# De um arquivo (um conceito por linha)
python professor.py --arquivo conceitos.txt

# Modo interativo
python professor.py --interativo
```

---

## Pesquisador autônomo

O Pesquisador coleta dados da Wikipedia PT+EN continuamente.

```bash
python pesquisador.py start    # inicia em background
python pesquisador.py stop     # para e salva
python pesquisador.py status   # estatísticas
```

---

## Arquitetura em camadas

```
┌─────────────────────────────────────────────────────────────┐
│  INTERFACE (nova.py) — terminal com notificações em tempo real │
├─────────────────────────────────────────────────────────────┤
│  NÚCLEO COGNITIVO (nucleo.py)                                │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐       │
│  │ Analista │ │ Criativo │ │ Crítico  │ │ Empático │       │
│  └──────────┘ └──────────┘ └──────────┘ └──────────┘       │
│                    ↓ Síntese ponderada                       │
├─────────────────────────────────────────────────────────────┤
│  MEMÓRIA (memoria.py)                                        │
│  M1 Conversa │ M2 Geral │ M3 Kevin │ M4 Própria │ M5 Relações│
├─────────────────────────────────────────────────────────────┤
│  BASE DE CONHECIMENTO (conceitos.py + compositor.py)         │
│  Dimensões numéricas │ Grafos │ Física semântica             │
├─────────────────────────────────────────────────────────────┤
│  APRENDIZADO (pesquisador.py + professor.py + agenda)        │
│  Crawler Wikipedia │ Professor LLM │ Pesquisa sob demanda    │
└─────────────────────────────────────────────────────────────┘
```

---

*Projeto desenvolvido do zero — sem modelos pré-treinados no núcleo de raciocínio.*
