---
name: org-readme-layout
description: Organiza o README de exibição da organização no GitHub com logo, nome, resumo e footer. Usar ao criar ou editar README.md do perfil da organização, ao estruturar o layout do readme ou quando o usuário pedir passo a passo do readme.
---

# Organização do README da Organização

Passo a passo para montar o README de exibição da organização no GitHub.

## 1. Logo (topo, centralizada)

- **Local**: `assets/logo/` — usar um dos arquivos:
  - `*notext*` — logo sem texto
  - `*text*` — logo com texto
- **Estilo**: largura 200px, bordas arredondadas, centralizada.

Exemplo em Markdown:

```markdown
<p align="center">
  <img src="assets/logo/logo-notext.png" width="200" style="border-radius: 8px;" alt="ProfitAI" />
</p>
```

O usuário escolhe se o arquivo é `logo-notext.png` ou `logo-text.png` (ou extensão equivalente).

## 2. Nome da organização

Logo abaixo da logo, o nome **ProfitAI** (ou o nome da organização), em destaque.

```markdown
<p align="center"><strong>ProfitAI</strong></p>
```

## 3. Linha divisória

Uma linha horizontal separando o cabeçalho do conteúdo.

```markdown
---
```

## 4. Resumo da organização

Texto explicando o que é a organização. Para a ProfitAI:

- **Foco**: restaurantes.
- **Uso do sistema**: gerenciar gastos, ver o que pode melhorar, margem de lucros.
- **Alertas**: resumo de faturamento via WhatsApp.
- **Objetivo**: o dono do restaurante saber como está indo o negócio.

Incluir também que o **desenvolvimento** é focado em IA, em especial **agentes de IA**.

Manter linguagem clara e sem dados sensíveis.

## 5. Footer

- Linha divisória acima do footer.
- Texto centralizado: **@ProfitAI 2026** (ou ano atual).
- Tudo centralizado.

```markdown
---
<p align="center">@ProfitAI 2026</p>
```

---

## Template completo

Usar esta estrutura ao montar o README. Substituir `logo-notext.png` por `logo-text.png` se o usuário preferir logo com texto.

```markdown
<p align="center">
  <img src="assets/logo/logo-notext.png" width="200" style="border-radius: 8px;" alt="ProfitAI" />
</p>

<p align="center"><strong>ProfitAI</strong></p>

---

A **ProfitAI** é focada em restaurantes. Os estabelecimentos usam nosso sistema para gerenciar gastos, identificar o que pode melhorar e acompanhar a margem de lucro. Os donos recebem alertas via WhatsApp com o resumo do faturamento, para saber como o negócio está indo.

No desenvolvimento do sistema, priorizamos o uso de **IA**, com foco em **agentes de IA**.

---

<p align="center">@ProfitAI 2026</p>
```

## Checklist antes de finalizar

- [ ] Logo em `assets/logo/` (notext ou text conforme escolha).
- [ ] Logo com `width="200"` e bordas arredondadas.
- [ ] Nome da organização abaixo da logo.
- [ ] Divisória entre cabeçalho e resumo.
- [ ] Resumo com foco em restaurantes, gestão, alertas WhatsApp e desenvolvimento em IA/agentes.
- [ ] Footer com divisória e "@ProfitAI 2026" centralizado.
- [ ] Nenhum dado sensível (e-mails, tokens, URLs internas, etc.).
