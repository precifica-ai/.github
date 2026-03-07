---
description: Executa fluxo git add, commit convencional e push usando o subagente github-org-readme e a skill conventional-commit-pt
---

- **Subagente:** github-org-readme  
- **Skill:** conventional-commit-pt  

Execute o fluxo abaixo, na ordem:

1. **Adicionar alterações:** `git add .`

2. **Commit convencional:** Gere a mensagem de commit usando a skill **conventional-commit-pt** (prefixos em inglês, descrição em português). Use o subagente **github-org-readme** quando fizer sentido ao contexto das mudanças. Em seguida execute: `git commit -m "<mensagem>"`

3. **Enviar:** `git push`

Resumo dos comandos: `git add .` → `git commit -m "..."` (mensagem pela skill conventional-commit-pt) → `git push`.
