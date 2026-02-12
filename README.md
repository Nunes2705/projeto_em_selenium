# 📚 Automação de Busca de Preços e Disponibilidade de Livros

Este projeto é uma ferramenta de automação desenvolvida em Python que realiza a busca sistemática de livros em múltiplas plataformas web para verificar disponibilidade, links oficiais e preços.

## 🚀 Objetivo
Otimizar o processo de coleta de dados de produtos, integrando informações de diferentes fontes (Projeto Gutenberg e Books to Scrape) em uma planilha mestre de forma automática e precisa.

## 🛠️ Tecnologias Utilizadas
* **Python**: Linguagem base.
* **Selenium**: Para automação de navegação e Web Scraping.
* **Pandas**: Para manipulação, análise e gestão de dados (DataFrames).
* **Excel**: Utilizado como entrada (input) e saída (output) dos dados processados.

## 📋 Como Funciona
O script executa os seguintes passos analíticos:
1. **Leitura de Dados**: Carrega uma lista de livros de um arquivo `Produtos.xlsx`.
2. **Busca Prioritária (Gutenberg)**: Tenta localizar o livro como domínio público no Projeto Gutenberg.
3. **Busca de Backup (Books to Scrape)**: Caso não encontre no primeiro site, o robô navega por categorias e páginas no Books to Scrape para localizar o título e capturar o preço.
4. **Consolidação**: Exporta todos os dados (links e valores encontrados) para um novo arquivo chamado `ProdutosAtualizado.xlsx`.

## 🔧 Como Executar
1. Certifique-se de ter o Python e o Chrome instalados.
2. Instale as dependências necessárias:
   ```bash
   pip install selenium pandas openpyxl
3. Mantenha o arquivo Produtos.xlsx na mesma pasta do script.
4. Execute o arquivo automacao 2.ipynb.   
