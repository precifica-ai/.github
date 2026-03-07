---
name: conventional-commit-pt
description: Gera mensagens de commit no formato Conventional Commits com prefixos em inglês e descrição em português. Usar ao escrever ou sugerir mensagens de commit, ao revisar mudanças staged ou quando o usuário pedir commit convencional.
---

# Commit convencional (prefixo EN, descrição PT)

Gera mensagens de commit no padrão [Conventional Commits](https://www.conventionalcommits.org/): **prefixos (type/scope) em inglês**, **descrição e corpo em português**.

## Formato

```
<type>(<scope>): <descrição em português>

[corpo opcional em português]
```

- **type** e **scope**: sempre em inglês.
- **Descrição** (após os dois pontos): em português, imperativo, sem ponto final na primeira linha.
- **Corpo** (opcional): em português.

## Tipos (em inglês)

| Tipo     | Uso |
|----------|-----|
| `feat`   | Nova funcionalidade |
| `fix`    | Correção de bug |
| `docs`   | Apenas documentação |
| `style`  | Formatação, espaços, etc. (sem mudança de código) |
| `refactor` | Refatoração (sem feat nem fix) |
| `perf`   | Melhoria de performance |
| `test`   | Testes |
| `chore`  | Build, deps, tarefas gerais |
| `ci`     | Configuração de CI/CD |

Scope é opcional (ex.: `feat(auth):`, `fix(api):`).

## Exemplos

**feat**
```
feat(auth): adiciona login com JWT
feat: implementa exportação em PDF do relatório
```

**fix**
```
fix(api): corrige serialização de datas no endpoint de pedidos
fix: resolve loop infinito na validação do formulário
```

**docs**
```
docs: atualiza README com instruções de deploy
docs(api): descreve parâmetros do endpoint /users
```

**refactor / chore**
```
refactor(db): extrai queries para repositório
chore(deps): atualiza dependências de desenvolvimento
```

**Com corpo**
```
feat(relatorios): adiciona filtro por período

Inclui seletor de data inicial e final na tela de relatórios.
Ajusta chamada à API para enviar parâmetros no query string.
```

## Checklist antes de sugerir

- [ ] Tipo (e scope, se houver) em **inglês**.
- [ ] Descrição em **português**, modo imperativo.
- [ ] Primeira linha com até ~72 caracteres quando possível.
- [ ] Sem ponto final na primeira linha.
