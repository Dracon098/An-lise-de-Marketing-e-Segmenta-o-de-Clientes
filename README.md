# 🎯 **Segmentação de Clientes & Análise de Marketing**

<div align="center">
  <img src="https://github.com/user-attachments/assets/90be0dfa-09ac-46c4-9994-dfd3843559b7" alt="Banner de Análise de Marketing" />
</div>

## 📊 **Visão Geral do Projeto**
Este projeto implementa um sistema avançado de segmentação de clientes e análise preditiva de marketing para uma empresa do setor alimentício. Utilizando técnicas de aprendizado de máquina, analisamos o comportamento dos clientes, dados demográficos e padrões de compra para otimizar o direcionamento de campanhas de marketing e aumentar o ROI.

---

## 🎯 **Objetivos Principais**
- Segmentar clientes com base em seu valor e potencial.  
- Desenvolver perfis detalhados dos clientes ideais.  
- Otimizar o direcionamento de campanhas de marketing.  
- Maximizar o retorno sobre o investimento em marketing.  

---

## 🔍 **Análise de Dados**

### **Análise do Perfil dos Clientes (1960-1990)**  
- **Educação**: 41% possuem ensino superior completo, apenas 2% têm educação básica.  
- **Estado Civil**: 65% em relacionamentos estáveis (39% casados, 26% união estável).  
- **Distribuição Etária**: Abrange diferentes faixas etárias, de 18 a 60+ anos.  

<div align="center">
  <img src="https://github.com/user-attachments/assets/4f09de2f-afa2-4c52-941b-7c36dbcfccac" alt="Distribuição Etária" />
  <p><em>Gráfico da distribuição etária dos clientes</em></p>
</div>

### **Comportamento de Compra**  
- Análise de várias categorias de produtos (vinhos, frutas, carnes, peixes, etc.).  
- Preferências de canal (web, catálogo, loja).  
- Taxas de resposta às campanhas.  

---

## 🛠️ **Implementação Técnica**

### **Pré-processamento de Dados**  
- Engenharia e seleção de características.  
- Tratamento de valores ausentes.  
- Normalização e escalonamento de dados.  
- Codificação de variáveis categóricas.  

### **Modelos de Machine Learning**

#### **1. Segmentação de Clientes**  
- **Análise de Clusters**: Identificados 3 segmentos distintos de clientes.  
- **Características Principais**: Renda, Idade, Padrões de Compra.  
- **Implementação**: Clustering K-means com PCA.  

<div align="center">
  <img src="https://github.com/user-attachments/assets/ddef5913-f0ff-4721-9a7d-dbc48096f6f1" alt="Clusters de Segmentação" />
  <p><em>Distribuição dos clusters dos clientes</em></p>
</div>

#### **2. Modelo Preditivo**  
- **Algoritmo**: Regressão Logística (otimizada).  
- **Métricas de Desempenho**:
  - ROC AUC: ~75-80%.  
  - Precisão: ~50-55%.  
  - Recall: ~60-65%.  
- **Validação Cruzada**: Estratégia com 5 dobras.  

<div align="center">
  <img src="https://github.com/user-attachments/assets/e20edffc-374a-4a62-acd7-83bf441f6a8b" alt="Desempenho do Modelo" />
  <p><em>Curva ROC do modelo preditivo</em></p>
</div>

---

## 👥 **Segmentos de Clientes Identificados**
- **🎯 Segmento 0: Clientes Premium**  
  - Alta renda.  
  - Alto gasto.  
  - Sem filhos.  
  - Alta taxa de aceitação de campanhas.  
  - Níveis mais altos de educação.  

- **👨‍👩‍👧‍👦 Segmento 1: Famílias Conscientes do Orçamento**  
  - Renda mais baixa.  
  - Menor gasto.  
  - Com filhos.  
  - Menor aceitação de campanhas.  
  - Mais educação básica.  
  - Demografia mais jovem.  

- **👴 Segmento 2: Seniores de Renda Média**  
  - Renda média.  
  - Gasto moderado.  
  - Com filhos.  
  - Aceitação média de campanhas.  
  - Demografia mais velha.  

---

## 📈 **Desempenho do Modelo**
- Melhores parâmetros encontrados através do **GridSearchCV**.  
- Seleção de características identificou 25 preditores mais importantes.  
- Melhoria significativa sobre as métricas base.  

<div align="center">
  <img src="https://github.com/user-attachments/assets/e3ff36ff-9fb2-411d-b7c9-2c0736deb998" alt="Importância das Características" />
  <p><em>Importância das características no modelo preditivo</em></p>
</div>

---

## 🚀 **Como Começar**

### **Pré-requisitos**  
- Python >= 3.8.  
- pandas, numpy, scikit-learn, imbalanced-learn, seaborn, matplotlib.  

### **Instalação**  
```bash
git clone https://github.com/Dracon098/analise_segmentacao_clientes
cd segmentacao-clientes
pip install -r requirements.txt

├── data/
│   ├── ml_project1_data.csv
│   └── processed/
├── notebooks/
│   ├── 1_analise_exploratoria.ipynb
│   ├── 2_analise_clusters.ipynb
│   ├── 3_modelagem_preditiva.ipynb
│   └── 4_otimizacao_modelo.ipynb
├── src/
│   ├── preprocessing/
│   ├── models/
│   └── visualization/
└── README.md
