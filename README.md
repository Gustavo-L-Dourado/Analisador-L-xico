# 📦 Analisador Léxico: Rastreio de Encomendas

**Autor:** Gustavo Landim Dourado (RA: 2473254)  
*Projeto desenvolvido para o Desafio de Analisador Léxico (Tema: Correios e Mercado Livre).*

---

## 🚀 O Projeto

Este repositório contém um analisador léxico construído em **Python** usando a biblioteca **Lark**. Ele processa uma mini-linguagem criada para monitoramento de pacotes (a "RastreioLang") e conta com uma interface gráfica interativa feita com **ipywidgets**.

O notebook já vem com o código executado e sem erros, incluindo a instalação automática de dependências.

---

## 📁 O que tem no código?

O arquivo `.ipynb` possui 9 células que abrangem todo o funcionamento do analisador. De forma resumida, ele contém:

1. **Configuração:** Instalação de bibliotecas e utilitários visuais.
2. **Gramática:** Definição de 23 tokens, palavras reservadas e expressões regulares (Regex).
3. **Tokenizador:** Motor de análise e tratamento inteligente de erros.
4. **Testes:** Casos de uso automatizados (válidos e inválidos) e resolução de ambiguidades.
5. **Interface:** Tela interativa para digitar, testar os códigos e ver a tabela de tokens.

---

## ⚙️ Como Executar

⚠️ **Atenção:** Rode as células obrigatoriamente em ordem (da primeira à última).

**Opção A: No Google Colab (Mais fácil)**
1. Faça o upload do arquivo `.ipynb` no Colab.
2. No menu superior, clique em *Ambiente de execução → Executar tudo*.

**Opção B: Localmente (VS Code / Jupyter)**
1. Instale as dependências no terminal:
   ```bash
   pip install lark ipywidgets ipykernel
