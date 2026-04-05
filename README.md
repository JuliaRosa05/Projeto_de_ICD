# Porcentagem de Sucesso em Processos Seletivos: Estudantes do CI-UFPB

Este projeto faz parte da disciplina de **Introdução à Ciência de Dados (ICD)** e tem como objetivo analisar o desempenho e a taxa de aprovação de estudantes do Centro de Informática da Universidade Federal da Paraíba (CI-UFPB) em processos seletivos do setor de tecnologia.

## 👥 Equipe
* **Ítalo Mendonça**
* **Julia Rosa**
* **Maria Nathalia**

---

## 🎯 Objetivo do Projeto
Investigar e quantificar o sucesso de estudantes das graduações do Centro de Informática (Ciência da Computação, Engenharia de Computação e Ciência de Dados e IA) em seleções do mercado de trabalho.

Além da métrica geral, o projeto busca identificar:
* **Recorte de Gênero:** Existe diferença na taxa de aprovação ou no tempo de inserção no mercado entre estudantes de diferentes gêneros?
* **Diferença entre Cursos:** Há variação de sucesso entre as três graduações do Centro?

---

## 📊 Abordagem de Coleta de Dados
A metodologia de coleta foi estruturada para garantir a integridade dos dados oficiais:

* **Dados Acadêmicos (CI):** Extração de listas de bolsistas e voluntários de projetos de extensão e PROBEX através dos portais institucionais e documentos do Centro de Informática.
* **Dados de Mercado (Externo):** Mineração de nomes e cargos em editais de convocação para residências tecnológicas, concursos e estágios publicados no Diário Oficial.
* **Enriquecimento via API:** Para a análise de gênero, utilizamos a API de nomes do IBGE, que realiza a predição probabilística do gênero com base no primeiro nome dos candidatos.

---

## 📖 Dicionário de Dados
Abaixo estão as descrições das colunas que compõem o dataset final:

| Nome da Coluna | Descrição da Coluna | Exemplo |
| :--- | :--- | :--- |
| `origem_dado` | Indica se o registro é proveniente do ambiente universitário (CI) ou do mercado (Diário Oficial). | "Universidade" |
| `curso` | Graduação vinculada ao estudante (Ciência da Computação, Engenharia de Computação ou Ciência de Dados e IA). | "Ciência de Dados e IA" |
| `genero_predito` | Gênero identificado através da API do IBGE com base no primeiro nome. | "Feminino" |
| `tipo_vaga` | Categoria da oportunidade (Extensão, Monitoria, Estágio ou Efetivo). | "Extensão" |
| `ano_referencia` | Ano de publicação do edital ou da convocação oficial. | 2024 |
| `status_selecao` | Indica se o estudante foi aprovado, classificado ou convocado para a vaga. | "Aprovado" |

---

## 🔗 Disponibilização dos Dados
Os dados brutos e processados utilizados nesta análise estão disponíveis no serviço de armazenamento abaixo:

* [Link para a pasta de dados (Google Drive/GitHub Data)]

---
*Projeto desenvolvido para a disciplina de ICD - UFPB (2025.2).*
