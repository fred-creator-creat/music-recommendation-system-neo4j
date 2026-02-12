# Sistema de Recomendação Musical com Neo4j

Este projeto foi desenvolvido como parte de um desafio prático de banco de dados NoSQL (Grafos). O objetivo é simular um sistema de recomendação de músicas e artistas utilizando o Neo4j e a linguagem de consulta Cypher.

## 📌 Visão Geral do Projeto
O sistema permite conectar usuários a músicas, artistas e gêneros musicais, permitindo realizar recomendações baseadas no comportamento de outros usuários com gostos similares (Filtragem Colaborativa).

## 🚀 Tecnologias Utilizadas
* **Arrows.app**: Para a modelagem visual do grafo.
* **Neo4j AuraDB**: Instância na nuvem para execução do banco de dados.
* **Cypher**: Linguagem de consulta para grafos.

## 📐 Modelagem de Dados (Arrows)
Abaixo, a estrutura lógica definida no início do projeto:

![Modelo Lógico](Start%20imange%20music%20recomendation%20sistem.png)

### Entidades e Relacionamentos:
* **User**: (Usuário)
* **Track**: (Música)
* **Artist**: (Artista)
* **Genre**: (Gênero)
* **Relacionamentos**: `LISTENED`, `FOLLOWS`, `PERFORMED_BY`, `BELONGS_TO`, `LIKES`.

## 💻 Implementação e Gráfico Final
Após a execução dos scripts Cypher, o grafo resultante no Neo4j Aura apresenta as conexões entre João, Maria, Carlos e os elementos musicais:

![Grafo Final](grafico_final.png)

## 🔍 Consultas de Recomendação (Exemplos)
No arquivo `project_music_neo4j` (dentro deste repositório), você encontrará as queries utilizadas para:
1. **Recomendação por Gênero**: Sugere músicas de gêneros que o usuário já demonstrou interesse.
2. **Recomendação Colaborativa**: Sugere músicas que usuários com histórico similar ouviram, mas que o usuário atual ainda não conhece.

---
*Projeto realizado para fins educacionais - DIO.*
