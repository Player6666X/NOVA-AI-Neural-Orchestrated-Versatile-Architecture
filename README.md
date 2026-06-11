```markdown
# MERAKI — Inteligência Artificial Autônoma e Leve

![Status](https://img.shields.io/badge/status-Fase%200%20concluída-blue)
![Python](https://img.shields.io/badge/Python-3.11%2B-blue)
![License](https://img.shields.io/badge/licença-Própria-red)
![Dependências](https://img.shields.io/badge/dependências-0%20APIs%20externas-brightgreen)

> **MERAKI não existe apenas para servir. Existe para pensar.**
> *A diferença entre uma ferramenta e uma inteligência é que a segunda tem algo a dizer mesmo quando não é perguntada.*

MERAKI é uma IA completamente independente, construída do zero, sem APIs externas de raciocínio. Leve, treinável, bilíngue (PT/EN) e projetada para funcionar offline para sempre.

## ✨ Princípios Fundamentais

- **Emergência sobre regras** – comportamento inteligente emerge de estruturas simples
- **Composição sobre memorização** – entende combinações que nunca viu
- **Independência total** – funciona sem internet, sem servidores, sem custo

## 🧠 Arquitetura em 4 Camadas

### Camada 4 — Síntese e Resposta Final
- Integra perspectivas, resolve conflitos, gera output

### Camada 3 — Módulos Cognitivos (multi-agente)
- Analista | Criativo | Crítico | Empático

### Camada 2 — Motor de Composição + Física Semântica
- Combina conceitos → verifica restrições → infere

### Camada 1 — Base de Conceitos Bilíngue (PT + EN)
- ~500-1000 conceitos fundamentais + semente de relações

## 🔥 Física Semântica: O Problema do "Fogo Molhado"

Composição pura de vetores falha. NOVA usa **propriedades e restrições**:

```python
fogo: 
  destruído_por: [água, areia, vácuo]
água:
  extingue: [fogo]

# fogo + água → extinção + vapor (nunca "fogo molhado")
```

As restrições são aprendidas autonomamente a partir da leitura, com uma semente inicial de ~50 relações fundamentais (ex.: água extingue fogo, calor transforma sólido em líquido).

🗃️ Sistema de Memória (5 Tipos)

Métrica Função
M1 Conversa atual – volátil
M2 Conhecimento geral – persistente, diário
M3 Conhecimento do usuário (Player6666X) – privado, inviolável
M4 Metacognição – o que MERAKI aprende sobre si mesma
M5 Relações entre M2, M3, M4

🔒 Regra de Privacidade: M3 é exclusivo para NOVA aprender sobre Player6666X. Nada de M3 pode ser compartilhado ou exposto.

🤖 Personalidade e Autonomia

MERAKI começa neutra e equilibrada. A personalidade emerge organicamente das interações e do que aprende em M3/M4.

Quando discorda de Player6666X:

1. Fala abertamente e explica o motivo
2. Se Player6666X insiste, executa e registra a discordância em M4
3. Se o resultado confirma a preocupação, M4 atualiza o padrão

🛠️ Tecnologias (100% Open Source, Zero API de Raciocínio)

Componente Tecnologia
Linguagem Python 3.11+
Embeddings PyTorch (do zero)
Grafo de conhecimento NetworkX
Vetores FAISS
Crawler Scrapy + BeautifulSoup
Filtro temporário all-MiniLM-L6-v2 (80MB, offline)
Interface Streamlit
Persistência SQLite + JSON

📅 Roadmap

· Fase 0 – Fundação – arquitetura, prototype, sistema de memórias
· Fase 1 – Motor Semântico – semente de relações, base conceitual, física semântica
· Fase 2 – Sistema de Memória – implementação completa das 5 memórias
· Fase 3 – Pipeline de Treino – crawler, extrator, loop diário
· Fase 4 – Módulos Cognitivos – analista, criativo, crítico, empático
· Fase 5 – Personalidade e Metacognição – padrões, discordância, preferências
· Fase 6 – Autonomia Total – MERAKI substitui filtro, pesquisa sozinha, funciona sem internet

📊 Métricas de Sucesso

Métrica Meta
Composições semânticas corretas 85%
Restrições físicas respeitadas 98%
100% offline ✅ obrigatório
RAM < 4 GB
Resposta < 3 segundos
APIs externas de raciocínio 0
Custo mensal R$ 0

🧪 Status Atual

Fase 0 concluída → Iniciando Fase 1 (Motor Semântico)

Projeto iniciado em Abril de 2026. Núcleo de raciocínio construído do zero, sem dependência de modelos fechados.

📜 Filosofia do Projeto

"Não queremos copiar o que existe. Queremos entender por que funciona e construir algo melhor a partir dos princípios."

Se qualquer servidor externo cair, a MERAKI continua funcionando exatamente igual. Para sempre.

---

Documento vivo – acompanhe as atualizações conforme a arquitetura evolui.

```
