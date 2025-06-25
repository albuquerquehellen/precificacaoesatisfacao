<h1 align="center">🛒 Análise de Produtos e Avaliações - Amazon</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white" />
</p>

---

## 🎯 Objetivo

Realizar uma análise sobre produtos vendidos na **Amazon**, investigando a relação entre **descontos**, **preços**, **avaliações** e **engajamento dos clientes**.

O projeto busca validar hipóteses e gerar recomendações estratégicas para orientar ações comerciais, de pricing e campanhas promocionais mais assertivas.

---

## 🛠️ Ferramentas e Tecnologias

- 📌 **Google Colab**  
- 📦 **Python 3.10**  
- 📚 Bibliotecas:
  - `pandas`
  - `matplotlib`
  - `seaborn`

---

## ⚙️ Processamento de Dados

- **Limpeza e normalização:** tratamento de nulos, conversão de tipos e padronização de categorias.
- **Integração de dados:** união das bases de produtos e avaliações via `product_id`.
- **Criação de variáveis derivadas:**
  - `desconto_alto` (≥ 50%)
  - `nota_alta` (≥ 4,5)
  - Faixas de preço, desconto e quantidade de avaliações usando `pd.cut()`.
- **Cálculo de estatísticas descritivas:** média, mediana, moda, desvio padrão, variância e IQR.
- **Correlação de Pearson** e **Risco Relativo** para avaliar associações e probabilidades.

---

## 📊 Principais Descobertas

- **Descontos maiores não aumentam as notas** dos produtos — correlação negativa fraca (–0,17).
- Produtos com desconto **≥ 50% têm 12% menos chance de receber nota ≥ 4,5** (Risco Relativo = 0,88).
- **Faixas de preço intermediárias concentram o maior volume de avaliações.**
- **Preço não influencia significativamente a nota média** (correlação +0,12).
- **Categorias de destaque:**
  - 📈 **Melhor avaliação:** *Accessories*, *Craft Materials*, *Batteries*
  - 💸 **Maior desconto:** *Wearable Technology*, *Accessories*

---

## 📌 Conclusões

- Descontos agressivos não elevam a satisfação do cliente.
- Preço isolado não determina o engajamento nem a avaliação média.
- Algumas categorias combinam bons descontos e notas altas — ideais para campanhas promocionais.
- A reputação do produto depende mais da experiência do cliente e da qualidade percebida do que de preço ou desconto.

---

## 📝 Recomendações

- Evitar apostar em grandes descontos como estratégia para aumentar avaliações.
- Priorizar categorias com bom desempenho combinado (desconto e avaliação) para campanhas e promoções.
- Investir na experiência do cliente e na qualidade do produto.
- Explorar faixas de preço intermediárias, que concentram maior volume de avaliações e potencial de engajamento.
