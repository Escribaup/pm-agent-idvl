# PM Agent — iDVL Tecnologia Contábil

Ferramenta de gestão de projetos e OKRs com IA embutida. Arquivo HTML único, zero dependências, roda direto no navegador.

## ✨ Funcionalidades

- **Dashboard** — visão geral do projeto com progresso RAG dos OKRs
- **OKRs** — objetivos e key results com sliders de progresso
- **Log de acontecimentos** — registro estruturado com análise de IA (decisão, ação, risco, marco, reunião, blocker, lição, checkpoint)
- **Riscos (CRGP)** — registro com probabilidade, impacto e status
- **Marcos (CRO)** — linha do tempo do projeto
- **Artefatos** — geração de documentos com IA (Easy Life Canvas, TAP, EAP, Backlog, Stakeholders, Nota Técnica, etc.)
- **Tarefas** — gestão de tarefas com checklist, prioridade, vínculo a projeto e responsável
- **Calendário** — visão mensal consolidada de tarefas, marcos e prazos de todos os projetos

## 🤖 Provedores de IA suportados

- **Claude** (Anthropic) — `claude-haiku-4-5` ou qualquer modelo configurável
- **Gemini** (Google) — `gemini-2.5-flash` ou qualquer modelo configurável
- **ChatGPT** (OpenAI) — `gpt-4o-mini` ou qualquer modelo configurável

As API keys ficam salvas apenas no `localStorage` do navegador. Nunca são enviadas para servidor.

## 💾 Persistência de dados

- **localStorage** — dados salvos automaticamente no navegador
- **Pasta mapeada** (File System Access API) — sincronização com pasta local/Google Drive
- **Exportação/Importação JSON** — backup manual e transferência entre dispositivos

## 🗂️ Estrutura de skills (metodologia)

```
pm-agent-metodologia/
├── SKILL.md                    # Metodologia Easy Life Canvas + EasyPMDOC
└── references/
    ├── artefatos/
    │   └── easy-life-canvas.md
    └── templates/
        ├── LEIA-ME.md
        └── nota_tecnica.md     # Template customizável
```

Salve a pasta `pm-agent-metodologia/` na pasta mapeada para personalizar os artefatos gerados.

## 🚀 Deploy

### Vercel (recomendado)
1. Acesse [vercel.com/new](https://vercel.com/new)
2. Importe este repositório
3. Vercel detecta automaticamente como site estático
4. Cada push na `main` faz deploy automático

### Local
Abra `index.html` diretamente no Chrome ou Edge. Não requer servidor.

## 📋 Schema JSON dos projetos

O app usa arquivos `.json` por projeto. Para gerar um projeto com IA, clique em `{ } Schema` dentro do app para copiar o prompt completo.

## 🔧 Requisitos

- Chrome ou Edge (versão 86+) para a funcionalidade de pasta mapeada
- API key de pelo menos um provedor de IA para usar as funcionalidades de geração
- Sem dependências externas, sem Node.js, sem instalação

## 📝 Metodologia

Baseado em **EasyBok (Easy Life Canvas)** + **EasyPMDOC** (Hybrid Easy Project Management).

---

Desenvolvido por **iDVL Tecnologia Contábil** · Curitiba/PR
