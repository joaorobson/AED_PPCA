# PPCA-AED-GraphRAG

Este repositório contém os dados, scripts e resultados relacionados ao artigo que explora a aplicação de **GraphRAG** e **RAG Naive** em consultas a grafos de conhecimento construídos com o suporte do **LLM Graph Builder** e **Neo4j**.

## Integrantes

- João Robson Santos Martins
- Angelo Donizete Buso Júnior
- Clayton Alboy Monaro Inácio
- Zilber Rondineli Verona Sepúlveda

## Objetivo do Projeto

O objetivo deste projeto é comparar a eficiência de dois modos de interação baseados em RAG:
1. **Vector Mode**: Recuperação tradicional baseada em embeddings vetoriais.
2. **Graph+Vector+Fulltext Mode**: Combina navegação em grafos de conhecimento com recuperação vetorial e texto completo.

O domínio escolhido foi a **Constituição Federal Brasileira** e suas emendas, representadas em um grafo de conhecimento no banco de dados **Neo4j**.

## Estrutura do Repositório

- **/data**: Contém os documentos processados (Constituição e Emendas) em formato TXT e JSON.
- **/scripts**: Scripts Python usados para construir o grafo e gerar embeddings.
- **/results**: Arquivos JSON com as respostas geradas para cada modo de interação.
- **/notebooks**: Notebooks Jupyter para análise e visualização de resultados.

## Requisitos

- Python 3.9+
- Neo4j Desktop ou AuraDB
- Bibliotecas Python: `neo4j`, `openai`, `numpy`, `pandas`

## Como Reproduzir o Experimento

1. Clone o repositório:
   ```bash
   git clone https://github.com/angeloBuso/ppca-aed-graphrag.git
   cd ppca-aed-graphrag
