# Sobre a religião, o gene, os instintos e a covardia humana

> Repositório de construção de argumentos ateus para desmontar argumentos religiosos.

## Resumo

Repositório estruturado para análise crítica da religião sob as perspectivas da genética evolutiva, dos instintos humanos e das dinâmicas psicológicas e comportamentais da covardia e busca por conforto existencial, servindo de base para a construção de argumentos ateus e desmontagem de teses religiosas/apologéticas.

## Público e objetivo

- **Público:** Pessoas interessadas em ceticismo, ateísmo, biologia evolutiva, psicologia comportamental e debate racional contra apologética religiosa.
- **Objetivo:** Organizar referências, dados e construções argumentativas sólidas para desmontar argumentos religiosos.

## Estrutura de alto nível

| Caminho | Função |
|---|---|
| `AGENTS.md` | Índice único do agente (não repete as regras) |
| `CLAUDE.md` | Claude Code: importa `AGENTS.md` |
| `.gemini/settings.json` | Gemini CLI: contexto = `AGENTS.md` |
| `spec-root.md` | Autoridade arquitetural do projeto |
| `rules.md` | Governança permanente, inclusive fronteira script de repo vs script de produto |
| `software-development-rules.md` | SOLID, DI e padrões (só se o repo for software/sistemas) |
| `flow.md` | Ordem de leitura e execução |
| `status.md` / `timeline.md` | Estado e histórico do projeto |
| `setup.md` / `tools-*.md` | Ambiente e ferramentas |
| `specs/` | Especificações formais (`to-do/`, `done/`, `optional/`) |
| `scripts/validation/min-tree.txt` | Única lista da árvore mínima |
| `core/` | Essencial do produto, inclusive scripts de produto em `core/scripts/` |
| `scripts/` | Scripts do **repositório** (não entram em `/core`) |
| `docs/`, `ideas/`, `references/`, `reports/`, `prompts/`, `resources/` | Apoio documental e operacional |

## Agentes

`AGENTS.md` é o único texto de instrução. Cursor, OpenCode e Codex leem esse arquivo. Claude Code lê `CLAUDE.md`, que só importa `AGENTS.md`. Gemini CLI usa `.gemini/settings.json` para procurar `AGENTS.md` em vez de `GEMINI.md`.

## Como iniciar

1. Abra o repositório no Cursor IDE.
2. Leia: `spec-root.md` → `rules.md` → `flow.md` → `setup.md` → `core/readme.md`.
3. O conteúdo central de argumentos e teses do projeto vive em `/core`. Referências e pesquisas de apoio vivem em `references/` e `docs/`.
4. Novas frentes de argumentação ou tarefas devem ser especificadas em `specs/to-do/` usando `spec-template.md`.
5. Atualize `status.md` e `timeline.md` a cada entrega relevante.

Detalhes de ambiente: ver `setup.md`, `tools-linux.md` e `tools-windows.md`.

## Documentação relacionada

- Fluxo do agente: `flow.md`
- Regras permanentes: `rules.md`
- Regras de scripts: `rules-scripts.md`
- Molde de specs: `spec-template.md`

## Estado atual

`status.md` e `timeline.md` registram o estado operacional e as alterações do repositório.
