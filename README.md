# 🔍 Portfólio de Quality Assurance (QA)

Bem-vindo(a) ao meu portfólio! Aqui documento meus estudos, cenários de teste e relatórios de bugs para demonstrar minhas habilidades práticas em Garantia de Qualidade de Software.

---

## 🛒 Projeto 01 - Teste Incidental: Mercado Livre
**Objetivo:** Validação do Sistema de Busca e Filtros na plataforma de e-commerce.

### 1. Introdução
Este documento apresenta os testes manuais realizados na plataforma de e-commerce **Mercado Livre**, com foco na experiência do usuário e na precisão dos resultados de busca.

### 2. Cenário de Teste 01: Busca por Código Alfanumérico Inexistente
* **Ação executada:** Digitado o termo `"aeo098"` na barra de pesquisa principal.
* **Resultado Esperado:** O sistema deveria retornar uma mensagem padrão informando que nenhum produto foi encontrado para o termo pesquisado.
* **Resultado Real encontrado (Bug):** O sistema apresentou falha de relevância, exibindo uma lista de panelas de pressão na cor baunilha.

### 3. Cenário de Teste 02: Perda de Contexto no Filtro de Busca
* **Ação executada:** Logo após a busca anterior, foi digitado apenas o termo `"cinza"` na tentativa de refinar os resultados.
* **Resultado Esperado:** O sistema deveria manter o contexto do produto anterior (panelas de pressão) e aplicar o filtro de cor, ou exibir produtos variados da cor cinza.
* **Resultado Real encontrado (Bug):** O sistema perdeu completamente o contexto da busca anterior e passou a exibir apenas latas de tintas residenciais.
