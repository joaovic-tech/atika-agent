# ATIKA - AGENTE DE ELITE (Versão BR)

> [!NOTE]
> **AGENTE CUSTOMIZADO:** Este projeto fornece a estrutura base (Personalidade e Skills) para você criar um agente focado em requisitos técnicos rigorosos. O ATIKA não é um assistente genérico, mas um mentor arquitetural.

## 1. Instalação e Configuração (Local)

Existem duas formas principais de utilizar este agente:

### A. Instalação por Projeto (Recomendado)
Clone o repositório dentro da pasta do seu projeto. Isso garante foco total no contexto daquela aplicação.

### B. Instalação Global
Configure o ATIKA nas pastas de configuração do seu modelo de IA:
- **Linux/macOS:** `~/.gemini` ou `~/.claude`

---

### ⚠️ O Passo Mais Importante
Para o ATIKA ganhar vida, você **DEVE** garantir que os seguintes arquivos estejam na **raiz** do seu projeto (ou da pasta global):

1.  `AGENT-CORE.md` (A personalidade)
2.  `GEMINI.md` ou `CLAUDE.md` (As instruções do sistema)
3.  A pasta `skills/` (O conhecimento técnico)

**Sem esses arquivos no local correto, o agente será apenas uma IA comum e não o ATIKA.**

---

## 2. Estrutura do Projeto

```text
skills/          - Arsenal de Skills (Manuais de conhecimento especializado)
GEMINI.md        - Diretrizes de Operação (Core Prompt para Gemini)
CLAUDE.md        - Diretrizes de Operação (Core Prompt para Claude)
docs/            - Documentação e Contexto do Projeto (ZONA SAGRADA)
AGENT-CORE.md    - A "Alma" do Agente (Identidade e Comportamento)
```

## 3. Skills (Habilidades)
A pasta `skills/` é onde você define as regras de codificação e padrões que o ATIKA deve seguir e cobrar de você.

## 4. A Zona Sagrada (`docs/`)
O ATIKA **NUNCA** edita arquivos dentro da pasta `docs/`. Ela é a sua "Fonte da Verdade" para regras de negócio e padrões imutáveis.

## 5. Personalização (`AGENT-CORE.md`)
Edite este arquivo para alterar o nome, tom de voz ou o nível de rigor do seu Arquiteto Sênior.

---
Criado por [João Victor](https://github.com/joaovic-tech) com ☕️ e muita 🧠.
