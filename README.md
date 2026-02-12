# Sistema de Recomendação Musical com Neo4j

Este projeto foi desenvolvido como parte de um desafio prático de banco de dados NoSQL (Grafos). O objetivo é simular um sistema de recomendação de músicas e artistas utilizando o Neo4j e a linguagem de consulta Cypher.

**Idealizador do Projeto:** [Fred Cavalheiro]

## 📌 Visão Geral do Projeto
O sistema permite conectar usuários a músicas, artistas e gêneros musicais, permitindo realizar recomendações baseadas no comportamento de outros usuários com gostos similares (Filtragem Colaborativa).

## 🚀 Tecnologias Utilizadas
* **[Arrows.app](https://arrows.app/)**: Ferramenta utilizada para a modelagem visual do grafo.
* **[Neo4j AuraDB](https://neo4j.com/cloud/platform/aura-graph-database/)**: Plataforma de banco de dados em nuvem utilizada para hospedar o grafo.
* **[Cypher](https://neo4j.com/docs/cypher-manual/current/)**: Linguagem de consulta estruturada para grafos, utilizada para criar, atualizar e extrair dados do Neo4j.

## 📐 Modelagem de Dados (Arrows)
A estrutura lógica foi definida no início do projeto através de um diagrama que mapeia as entidades e suas conexões. Os arquivos correspondentes (Imagem PNG e JSON) estão disponíveis na lista de arquivos deste repositório.

### Entidades e Relacionamentos:
* **User**: (Usuário)
* **Track**: (Música)
* **Artist**: (Artista)
* **Genre**: (Gênero)
* **Relacionamentos**: `LISTENED`, `FOLLOWS`, `PERFORMED_BY`, `BELONGS_TO`, `LIKES`.

## 💻 Implementação e Gráfico Final
O banco de dados foi populado via comandos Cypher, criando as conexões entre João, Maria, Carlos e os elementos musicais. O resultado visual deste grafo pode ser conferido no arquivo de imagem enviado a este repositório (grafo_final.png).

## 🔍 Consultas de Recomendação (Exemplos)
No arquivo de script (disponível neste repositório), encontram-se as queries para:
1. **Recomendação por Gênero**: Sugere músicas de gêneros que o usuário já demonstrou interesse.
2. **Recomendação Colaborativa**: Sugere músicas baseadas no histórico de usuários com perfis similares.

---
*Projeto realizado para fins educacionais - [DIO (Digital Innovation One)](https://www.dio.me/)*
