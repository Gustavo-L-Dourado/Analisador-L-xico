# INTEGRANTES

Gustavo Landim Dourado Ra:2473254

# README — Desafio Analisador Léxico (Rastreio de Encomendas)

Este arquivo descreve o notebook **`Cópia_de_Desafio_Analisador_Lexico_Rastreio.ipynb`**,
entregue como resposta ao Desafio da Seção 7 da Aula CP 05 (Prática 1) —
"Meu Analisador Léxico de Mercado" (tema 2 — Rastreio de encomendas / Correios
e Mercado Livre).

## O que é

Um analisador léxico completo, escrito em Python com a biblioteca **Lark**
(`lexer="basic"`), para uma mini-linguagem de rastreio de encomendas
("RastreioLang"), com interface interativa em **ipywidgets**.

O notebook já vem **executado** (saídas salvas), tendo rodado sem erros —
inclusive a instalação das dependências via `%pip install` no Google Colab.

## Estrutura do notebook (9 células)

| # | Tipo | Conteúdo |
|---|------|----------|
| 0 | Markdown | Apresentação do desafio, do tema e da mini-linguagem |
| 1 | Código | Preparação do ambiente (instala `lark` e `ipywidgets`) |
| 2 | Código | Ferramentas de visualização (tabela de tokens, texto colorido, erro com "setinha") |
| 3 | Código | Gramática do lexer (23 tipos de token, com prioridades comentadas) |
| 4 | Código | Tokenizador + dicas de erro específicas do domínio |
| 5 | Código | Conversão de lexema em valor, mascaramento LGPD e pós-processamento (bônus) |
| 6 | Código | Casos de teste automatizados (válidos e inválidos) |
| 7 | Código | Laboratório de prioridade — reproduz ao vivo os conflitos léxicos |
| 8 | Código | Interface ipywidgets (entrada, botão, texto colorido, tabela de tokens, abas) |

> **Observação:** em relação à versão original entregue, esta cópia mantém
> apenas a célula de introdução em Markdown; as seções explicativas em texto
> (tabela de tokens documentada, diário de ambiguidade, tabela de requisitos
> e checklist de autoavaliação) foram removidas do notebook. Todo o código é
> idêntico ao da versão original e continua funcionando normalmente.

## Como executar

1. **Google Colab:** *Arquivo → Fazer upload de notebook* → selecione o
   `.ipynb` → *Ambiente de execução → Executar tudo*.
2. **VS Code / Jupyter local:**
   ```bash
   pip install lark ipywidgets ipykernel
   ```
   Abra o `.ipynb`, escolha o interpretador Python e execute as células em
   ordem (`Shift+Enter`).

As células devem ser executadas **em ordem** (0 → 8): cada uma depende de
funções/objetos definidos nas anteriores (gramática, tokenizador, funções de
visualização etc.).

## Requisitos do desafio atendidos pelo código

- ✅ 23 tipos de token (mínimo exigido: 12)
- ✅ 10 palavras reservadas + 2 grupos de reservadas, com `/i` e `\b`
- ✅ 10 literais definidos por expressão regular
- ✅ 3 conflitos de prioridade identificados e resolvidos (comentados na
  célula 3 e demonstrados ao vivo na célula 7)
- ✅ Comentários (`#`) e espaços ignorados via `%ignore`
- ✅ Erros léxicos com linha, coluna e mais de 15 dicas específicas do domínio
- ✅ Interface com entrada, botão, texto colorido e tabela de tokens
- ✅ 4 casos válidos + 7 inválidos + 2 "léxico OK, regra de negócio recusa"
- ✅ Bônus: pós-processamento (aba *Encomendas*), conversão de lexema em
  valor e mascaramento de dados pessoais (LGPD)
