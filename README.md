<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=1f77b4&height=120&section=header"/>

[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=1f77b4&size=35&center=true&vCenter=true&width=1000&lines=OLÁ,+EU+SOU+O+JOHNNY+FERNANDES;ANALISTA+DE+DADOS;CIENTISTA+DE+DADOS+EM+FORMAÇÃO;CONSULTOR+DE+NEGÓCIOS;SEJA+BEM-VINDO!+%3A%29)](https://git.io/typing-svg)


![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-An%C3%A1lise%20de%20Dados-orange?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualiza%C3%A7%C3%A3o%20Gr%C3%A1fica-blue?logo=matplotlib)
![License](https://img.shields.io/badge/Licen%C3%A7a-MIT-green)
![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)


## 📑 Sumário

- [Objetivo](#-objetivo)
- [Tecnologias](#-tecnologias-utilizadas)
- [Estrutura](#-estrutura-do-projeto)
- [Análises Estatísticas](#-análises-estatísticas)
- [Exemplos de Gráficos](#-exemplos-de-gráficos)
- [Insights Possíveis](#-insights-possíveis)
- [Como Executar](#-como-executar)
- [Dataset](#-dataset-recomenda-se-usar-um-ambiente-virtual)
- [Autor](#-autor)

---

# 📊 Análise Comparativa — Preço Normal x Preço Unitário

Este repositório contém uma análise exploratória comparando **Preço Normal (R$)** e **Preço Unitário** de produtos, com destaque para variações por categoria.  
A análise foi realizada utilizando **Python**, com bibliotecas de manipulação e visualização de dados.

## 🎯 Objetivo

Avaliar diferenças e dispersões entre os preços praticados, identificando categorias com maiores impactos e variações significativas, destacando:

- Produtos com maior variação de preço.
- Impacto em categorias específicas como **lácteos** e **beleza e cuidado pessoal**.
- Distribuição e comportamento estatístico (média, mediana e desvio padrão) por categoria.

---

## 🛠 Tecnologias Utilizadas

- Python 3.13
- Pandas
- Matplotlib
- Seaborn
- PyCharm / VSCode

---

## 📂 Estrutura do Projeto
analise_precos/
│
├── img/ # Imagens geradas dos gráficos
├── analise_precos.py # Script principal de análise
├── dataset_limpo.csv # Dataset tratado
└── README.md # Este arquivo


---

## 📈 Análises Estatísticas

### **Estatísticas Gerais**
| Métrica          | Preço Normal (R$) | Preço Unitário |
|------------------|-------------------|----------------|
| Média            | 28.20             | 21.57          |
| Desvio Padrão    | 31.35              | 21.57          |
| Contagem (n)     | 813.000            | 813.000        |

---

### **Por Categoria — Preço Unitário**
| Categoria                    | Média  | Mediana | Desvio Padrão |
|------------------------------|--------|---------|---------------|
| belleza-y-cuidado-personal   | 28.84  | 20.99   | 21.67         |
| comidas-preparadas           | 39.55  | 37.40   | 13.22         |
| congelados                   | 30.21  | 29.54   | 19.04         |
| frutas                       | 17.24  | 11.95   | 16.39         |
| instantaneos-y-sopas         | 11.79  | 6.89    | 12.76         |
| **lacteos**                   | **15.13**  | **9.89**    | **17.82**     |
| verduras                     | 14.57  | 12.50   | 9.72          |

---

### **Por Categoria — Preço Normal (R$)**
| Categoria                    | Média  | Mediana | Desvio Padrão |
|------------------------------|--------|---------|---------------|
| belleza-y-cuidado-personal   | 29.20  | 21.79   | 21.63         |
| comidas-preparadas           | 39.55  | 37.40   | 13.22         |
| congelados                   | 30.21  | 29.54   | 19.04         |
| frutas                       | 17.24  | 11.95   | 16.39         |
| instantaneos-y-sopas         | 11.79  | 6.89    | 12.76         |
| **lacteos**                   | **30.29**  | **17.20**   | **41.99**     |
| verduras                     | 14.57  | 12.50   | 9.72          |

---

## 📊 Exemplos de Gráficos

> A seguir, alguns gráficos gerados a partir da análise (todas as imagens estão na pasta `img/`):

### ✅ Comparativo — Preço Normal x Preço Unitário
<img src="img/grafico_comparativo.png" width="600"/>

### ✅ Distribuição de Preços por Categoria
<img src="img/distribuicao_categorias.png" width="600"/>

### ✅ Dispersão de Preços
<img src="img/boxplot_precos.png" width="600"/>

---

## 💡 Insights Possíveis

- **Produtos lácteos** apresentam a maior diferença entre Preço Normal e Preço Unitário.
- Categoria **beleza-y-cuidado-personal** tem **mediana e desvio padrão muito próximos**, indicando pouca dispersão e ausência de outliers relevantes.
- Categorias como **lácteos** têm desvio padrão elevado, mostrando forte variação de preços.
- Preço Unitário tende a ser mais estável que o Preço Normal.

---

## ▶ Como Executar

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/analise_precos.git

# Acesse a pasta do projeto
cd analise_precos

# Instale as dependências
pip install pandas matplotlib seaborn

# Execute o script principal
python analise_precos.py

📂 Dataset (recomenda-se usar um ambiente virtual)

O dataset já está limpo e tratado para análise.
Caso queira gerar novamente os gráficos, certifique-se de ter as bibliotecas instaladas e execute os scripts Python.

👨‍💻 Autor

Johnny Sorato Martins Fernandes
Consultor de Negócios | Especialista em Dados e Visualização | Diretor Executivo da Tutoreanos - Unidade Primavera do Leste


---
## 🔖 Tags
data-science, price-analysis, product-categories, descriptive-statistics, boxplot, discount-visualization, interactive-map, python, pandas, seaborn, plotly
