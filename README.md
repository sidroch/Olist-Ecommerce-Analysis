# 📦 Olist Ecommerce Analysis  
Análise completa do comportamento de vendas, logística e receita utilizando o dataset público da Olist.  
Projeto desenvolvido como parte do **Tech Challenge — Pós-Tech FIAP (2026)**.

---

## 📊 Objetivo do Projeto

Transformar dados operacionais da Olist em **insights estratégicos**, explorando:

- comportamento de compra por estado  
- eficiência logística  
- desempenho por categoria  
- receita por cliente  
- riscos e oportunidades regionais  
- storytelling analítico orientado por dados  

O projeto combina:

- **Python + Pandas** para EDA  
- **Power BI** para visualização executiva  
- **GitHub** para versionamento  
- **PDF** para apresentação final  

---

## 🧱 Estrutura do Repositório

Olist-Ecommerce-Analysis/

data/                 		# CSVs e datasets (originais + extraídos do PPT)
notebooks/            	# Jupyter Notebooks (.ipynb)
reports/              	# PDFs
scripts/              	# Scripts auxiliares em Python
README.md             	# Documentação do projeto
---
Bases de Dados Originais (Olist)
As bases originais foram obtidas do repositório público da Olist e incluem:
1.	customers.csv
2.	geolocation.csv
3.	order_items.csv
4.	order_payments.csv
5.	order_reviews.csv
6.	orders.csv
7.	products.csv
8.	sellers.csv
9.	product_category_name_translation.csv

---
Esses arquivos são utilizados para análises de:
1)	comportamento do consumidor
2)	logística
3)	receita
4)	categoria de produto
5)	relacionamento entre tabelas

---
Dados Extraídos do Relatório Executivo 
Além das bases originais, foram extraídos os principais indicadores apresentados nos gráficos e convertidos em CSV para uso no notebook.
Arquivos Gerados
receita_estado.csvInsights de receita por estado (SC, RJ, MG, RS, PR)
categorias.csvDestaques de categorias: maior volume, maior receita e alto valor agregado
logistica.csvPercentual de atrasos logísticos por estado
riscos_oportunidades.csvPrincipais riscos e oportunidades identificados por UF

---

## 📓 Notebooks
df_receita = pd.read_csv("../data/receita_estado.csv")
df_categorias = pd.read_csv("../data/categorias.csv")
df_logistica = pd.read_csv("../data/logistica.csv")
df_riscos = pd.read_csv("../data/riscos_oportunidades.csv")

Links de acesso aos gráficos
- 📊 [Gráficos do Relatório Executivo](notebooks/graficos_relatorio_olist.ipynb)
- 🔍 [Análise Exploratória de Dados (EDA)](notebooks/01_eda_olist.ipynb)

---

🔍 Principais Insights
🏆 Receita por Estado
1)	SC lidera em receita por cliente (+1,76% vs SP)
2)	RJ tem maior volume absoluto, mas gargalos logísticos
3)	MG, RS, PR apresentam estabilidade e previsibilidade
---
🛒 Categorias de Produto
1)	Cama & Mesa → maior volume
2)	Beleza & Saúde → maior receita
3)	Relógios → alto valor agregado

---
🚚 Eficiência Logística
Percentual de atrasos:
1)	RJ	12%
2)	SC	8%
3)	RS	6%
4)	MG	4%
5)	SP	4%
6)	PR	4%

---
⚠️ Riscos & Oportunidades
Risco: RJ com 12% de atrasos
Oportunidades: SC (premium), PR (relógios), MG/RS (expansão de base)

---
👥 Equipe
Projeto desenvolvido por:
Adriane de Souza Lino
Barbara Rodrigues Gusmão Rebelo
Bruna Alessandra Belotto
Sidnei Rocha 
Pós-Tech FIAP · Tech Challenge 2026

📄 Licença
Este projeto é de uso acadêmico e não possui vínculo oficial com a Olist.

