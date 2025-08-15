<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=1f77b4&height=120&section=header"/>

[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=1f77b4&size=35&center=true&vCenter=true&width=1000&lines=ANÁLISE+DE+PRODUTOS+DE+SUPERMERCADO+NO+CHILE;ESTATÍSTICAS+DE+PREÇOS+POR+CATEGORIA+E+MARCA;Usando+Média,+Mediana+e+Desvio+Padrão;COM+GRÁFICOS+E+MAPAS;BEM-VINDO+AO+MEU+PORTFÓLIO!)](https://git.io/typing-svg)

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Análise%20de%20Dados-orange?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualização%20Gráfica-blue?logo=matplotlib)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

---

## 📑 Sumário

- [Objetivo](#objetivo)
- [Tecnologias](#tecnologias-utilizadas)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Análise Estatística](#análise-estatística)
- [Exemplos de Gráficos](#exemplos-de-gráficos)
- [Principais Insights](#principais-insights)
- [Como Executar](#como-executar)
- [Base de Dados](#base-de-dados)
- [Autor](#autor)

---

# Análise Comparativa — Preço Regular vs. Preço Unitário

Este repositório contém uma análise exploratória comparando o **Preço Regular (R$)** e o **Preço Unitário** de produtos de supermercado, com foco nas variações entre categorias.  
A análise foi realizada com **Python**, utilizando bibliotecas de manipulação e visualização de dados.

---

## Objetivo

Avaliar estratégias de precificação e dispersão, identificando categorias com maior impacto e variação significativa, destacando:

- Produtos com maior flutuação de preços  
- Impacto em categorias específicas como **laticínios** e **beleza & cuidados pessoais**  
- Distribuição estatística (média, mediana e desvio padrão) por categoria

---

## Tecnologias Utilizadas

- **Python 3.13**
- **Jupyter Notebook** (recomendado para análise interativa)
- **Ambientes de Desenvolvimento**: PyCharm / VSCode
- **Bibliotecas**:
  - `pandas` — manipulação de dados
  - `numpy` — operações numéricas
  - `matplotlib.pyplot` — visualizações estáticas
  - `seaborn` — gráficos estatísticos
  - `plotly.express` — gráficos e mapas interativos

---

## 📁 Estrutura do Projeto

```
price-analysis-chile/
├── .git/                          # Controle de versão Git
├── .ipynb_checkpoints/            # Auto-salvamento do Jupyter
├── data/
│   └── raw/                       # Base de dados original (CSV)
├── docs/                          # Documentação e arquivos interativos (ex: treemap.html)
├── img/                           # Imagens geradas dos gráficos
├── notebooks/
│   ├── analise_precos.ipynb       # Notebook principal da análise
│   └── Profissao Cientista de Dados_Extraindo_Médias.ipynb  # Notebook complementar
├── .gitignore                     # Regras de exclusão do Git
├── README.md                      # Visão geral do projeto (em inglês)
├── README_pt.md                   # Versão em português
└── requirements.txt               # Dependências do projeto
```

---

## 📈 Análise Estatística

### Estatísticas Gerais

| Métrica            | Preço Regular (R$) | Preço Unitário |
|--------------------|--------------------|----------------|
| Média              | 28,20              | 21,57          |
| Desvio Padrão      | 31,35              | 21,57          |
| Total de Registros | 813                | 813            |

---

### Por Categoria — Preço Unitário

| Categoria                   | Média  | Mediana | Desvio Padrão |
|----------------------------|--------|---------|----------------|
| beleza-e-cuidados-pessoais| 28,84  | 20,99   | 21,67          |
| comidas-preparadas         | 39,55  | 37,40   | 13,22          |
| congelados                 | 30,21  | 29,54   | 19,04          |
| frutas                     | 17,24  | 11,95   | 16,39          |
| instantaneos-e-sopas       | 11,79  | 6,89    | 12,76          |
| **laticínios**             | **15,13** | **9,89** | **17,82**     |
| verduras                   | 14,57  | 12,50   | 9,72           |

---

### Por Categoria — Preço Regular (R$)

| Categoria                   | Média  | Mediana | Desvio Padrão |
|----------------------------|--------|---------|----------------|
| beleza-e-cuidados-pessoais| 29,20  | 21,79   | 21,63          |
| comidas-preparadas         | 39,55  | 37,40   | 13,22          |
| congelados                 | 30,21  | 29,54   | 19,04          |
| frutas                     | 17,24  | 11,95   | 16,39          |
| instantaneos-e-sopas       | 11,79  | 6,89    | 12,76          |
| **laticínios**             | **30,29** | **17,20** | **41,99**     |
| verduras                   | 14,57  | 12,50   | 9,72           |

---

## 📊 Exemplos de Gráficos

> Abaixo estão algumas visualizações geradas na análise (todas armazenadas na pasta `img/`):

### ✅ Dispersão de Preços — Boxplot Comparativo  
<img src="img/blox02.png" width="600"/>

### ✅ Distribuição por Categoria — Treemap Interativo  
<img src="img/treemap_interativo.png" width="400"/>

### ✅ Distribuição de Descontos — Gráfico de Densidade  
Para entender melhor como os descontos estão distribuídos entre os produtos, foi gerado um gráfico de densidade com base na diferença entre Preço Regular e Preço Unitário.

**Objetivo**  
- Identificar faixas de desconto mais comuns  
- Detectar assimetrias ou concentrações  
- Destacar categorias com estratégias agressivas de preço

**Metodologia**  
O desconto foi calculado como:

```python
desconto = Preço_Regular - Preço_Unitário
```

Visualizado com `seaborn.kdeplot()` para mostrar a densidade de probabilidade.

**Visualização**  
<img src="img/dens11.png" width="600"/>

---

## Principais Insights

- **Produtos lácteos** apresentam a maior diferença entre Preço Regular e Preço Unitário  
- A categoria de **beleza e cuidados pessoais** tem mediana e desvio padrão estreitos, indicando baixa dispersão e poucos outliers  
- Categorias como **laticínios** têm alto desvio padrão, sugerindo forte variação de preços  
- O **Preço Unitário** tende a ser mais estável que o **Preço Regular**

---

## ▶ Como Executar

```bash
# Clonar o repositório
git clone https://github.com/seu-usuario/price-analysis-chile.git

# Acessar a pasta do projeto
cd price-analysis-chile

# (Opcional) Criar e ativar ambiente virtual
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows

# Instalar dependências
pip install -r requirements.txt
```

### Executando a Análise

- Abrir o notebook principal:

```
notebooks/analise_precos.ipynb
```

- Para estudo complementar:

```
notebooks/Profissao Cientista de Dados_Extraindo_Médias.ipynb
```

---

## 📂 Base de Dados

A base está disponível em:

```
data/raw/
```

Pronta para análise. Para gerar os gráficos novamente, certifique-se de que todas as bibliotecas estão instaladas e execute os notebooks via Jupyter.

---

## 👨‍💻 Author

**Johnny Sorato Martins Fernandes**  
Business Consultant | Data & Visualization Specialist | Executive Director at Tutoreanos — Primavera do Leste Unit

---

## 🔖 Tags

`data-science`, `price-analysis`, `product-categories`, `descriptive-statistics`, `boxplot`, `discount-visualization`, `interactive-map`, `python`, `pandas`, `seaborn`, `plotly`

---
