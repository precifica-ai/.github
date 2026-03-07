---
description: Gera o README de exibição da organização no GitHub seguindo layout e regras do projeto
---

Use o subagente **github-org-readme** e a skill **org-readme-layout** para gerar o README da organização.

**Antes de gerar:**
1. Pergunte ao usuário qual logo usar: **notext** (logo sem texto) ou **text** (logo com texto). As opções ficam em `assets/logo/` (ex.: `logo-notext.png`, `logo-text.png`).
2. Se o usuário já tiver informado a escolha, use direto.

**Ao gerar:**
- Siga o passo a passo da skill org-readme-layout (logo centralizada 200px, nome da organização, divisória, resumo, footer).
- Respeite a regra org-readme-github: nenhum dado sensível, só conteúdo público.
- Escreva o conteúdo em `README.md` (ou no arquivo que for o README de exibição da organização).

**Depois de gerar:**
- Confirme que o checklist da regra e da skill foi atendido (logo, estrutura, sem dados sensíveis).
