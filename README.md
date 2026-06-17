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
- **PPT** para apresentação final  

---

## 🧱 Estrutura do Repositório

```text
Olist-Ecommerce-Analysis/
│
├── data/                 # CSVs e datasets (originais + extraídos do PPT)
├── notebooks/            # Jupyter Notebooks (.ipynb)
├── reports/              # PPTs, PDFs, apresentações
├── scripts/              # Scripts auxiliares em Python
└── README.md             # Documentação do projeto

Bases de Dados Originais (Olist)
As bases originais foram obtidas do repositório público da Olist e incluem:

customers.csv

geolocation.csv

order_items.csv

order_payments.csv

order_reviews.csv

orders.csv

products.csv

sellers.csv

product_category_name_translation.csv

Esses arquivos são utilizados para análises de:

Esses arquivos são utilizados para análises de:

comportamento do consumidor

logística

receita

categorias de produto

relacionamento entre tabelas

📥 Dados Extraídos do Relatório Executivo (PPT)
Além das bases originais, foram extraídos do PPT os principais indicadores apresentados nos gráficos e convertidos em CSV para uso no notebook.

📁 Arquivos Gerados
Arquivo	Descrição
receita_estado.csv	Insights de receita por estado (SC, RJ, MG, RS, PR)
categorias.csv	Destaques de categorias: maior volume, maior receita e alto valor agregado
logistica.csv	Percentual de atrasos logísticos por estado
riscos_oportunidades.csv	Principais riscos e oportunidades identificados por UF


Esses arquivos ficam em:

Código
/data
📥 Como carregar os dados no notebook
python
import pandas as pd

df_receita = pd.read_csv("../data/receita_estado.csv")
df_categorias = pd.read_csv("../data/categorias.csv")
df_logistica = pd.read_csv("../data/logistica.csv")
df_riscos = pd.read_csv("../data/riscos_oportunidades.csv")
🔍 Principais Insights
🏆 Receita por Estado
SC lidera em receita por cliente (+1,76% vs SP)

RJ tem maior volume absoluto, mas gargalos logísticos

MG, RS, PR apresentam estabilidade e previsibilidade

🛒 Categorias de Produto
Cama & Mesa → maior volume

Beleza & Saúde → maior receita

Relógios → alto valor agregado

🚚 Eficiência Logística
Percentual de atrasos:

Estado	% Atrasos
RJ	12%
SC	8%
RS	6%
MG	4%
SP	4%
PR	4%


⚠️ Riscos & Oportunidades
Risco: RJ com 12% de atrasos

Oportunidades: SC (premium), PR (relógios), MG/RS (expansão de base)

▶️ Como Executar o Projeto
1. Clonar o repositório
bash
git clone https://github.com/sidroch/Olist-Ecommerce-Analysis.git
cd Olist-Ecommerce-Analysis
2. Criar ambiente virtual (opcional)
bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
3. Instalar dependências
bash
pip install -r requirements.txt
4. Abrir o notebook
bash
jupyter notebook
🧠 Roadmap de Evolução
[ ] Criar dashboard final em Power BI

[ ] Implementar modelo preditivo de atraso logístico

[ ] Criar API simples para consulta de KPIs

[ ] Automatizar pipeline de ingestão de dados

[ ] Criar testes unitários para scripts Python

👥 Equipe
Projeto desenvolvido por:

Adriane de Souza Lino

Barbara Rodrigues Gusmão Rebelo

Bruna Alessandra Belotto

Sidnei Rocha — Pós-Tech FIAP · Tech Challenge 2026

📄 Licença
Este projeto é de uso acadêmico e não possui vínculo oficial com a Olist.
