# 📊 Precificação e Classificação de Equipamentos Industriais

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

> **Projeto Final** — Curso de Ciência de Dados e Inteligência Artificial (CDIA 2025)  
> Centro Universitário SENAI SC | Florianópolis/SC

## 📋 Sobre o Projeto

Conjunto de algoritmos desenvolvidos com o objetivo de **otimizar a precificação e classificação de equipamentos industriais** utilizando técnicas de Machine Learning.

O sistema resolve dois problemas principais:
1. **Previsão de Preço**: Estima o preço de venda de novos equipamentos baseado em suas características técnicas
2. **Classificação de Equipamentos**: Categoriza equipamentos em classes (A, B, C, D, E) para segmentação de clientes

## 📊 Dataset

O projeto utiliza dados históricos de equipamentos industriais com as seguintes variáveis:

### Variáveis Numéricas
- **Preço**: Valor de venda do equipamento
- **Potência**: Capacidade em kW/HP
- **Peso**: Massa do equipamento (kg)
- **Durabilidade**: Vida útil estimada (anos)
- **Garantia**: Período de cobertura (meses)

### Variáveis Categóricas
- **Classe**: Categorização (A, B, C, D, E)
- **Tecnologia**: Tipo (convencional, automatizada, embarcada, avançada)
- **Status**: Situação de manutenção

### Variáveis Booleanas
- Necessidade de energia, Requer manutenção, Sistema de refrigeração, Software integrado, Conectividade IoT

## 🔧 Etapas do Projeto

### 1️⃣ **Entendimento do Negócio**
- Contextualização do problema de precificação e classificação
- Definição de objetivos mensuráveis
- Alinhamento com necessidades do cliente

### 2️⃣ **Preparação dos Dados**
- Tratamento de dados faltantes (imputação por moda)
- Identificação e remoção de outliers
- Normalização e padronização de strings
- Label encoding para variáveis categóricas
- Conversão de booleanos (sim/não → 0/1)
- Padronização da coluna garantia para meses
- Matriz de correlação para seleção de features

### 3️⃣ **Modelagem de Machine Learning**

**Problema 1 - Regressão (Previsão de Preço)**
- Algoritmo: Random Forest Regressor
- Divisão: 80% treino / 20% teste
- Métricas: RMSE, MAE, R² Score

**Problema 2 - Classificação (Categorização)**
- Algoritmo: Decision Tree / Logistic Regression
- Validação cruzada
- Métricas: Acurácia, Precisão, Recall, F1-Score, Matriz de Confusão

### 4️⃣ **Avaliação e Melhorias**
- Análise de performance dos modelos
- Identificação de limitações
- Propostas de otimização e features futuras

### 5️⃣ **Implementação**
- Pipeline completo de dados
- Notebooks documentados no Google Colab
- Visualizações em BI

## 🛠️ Tecnologias Utilizadas

```python
Python 3.8+
├── pandas              # Manipulação de dados
├── numpy               # Computação numérica
├── scikit-learn        # Machine Learning
├── matplotlib          # Visualização
├── seaborn             # Gráficos estatísticos
```

**IDE/Plataforma**: Google Colab  
**Versionamento**: Git & GitHub

## 🚀 Como Executar

### Pré-requisitos
- Python 3.8 ou superior
- Conta no Google Colab (recomendado)

### Executar o Projeto

```bash
# Execute o notebook principal
jupyter notebook collab.py

# Ou acesse diretamente no Google Colab (recomendado)
```

## 📈 Resultados

- **Modelo de Regressão**: R² Score de X.XX, RMSE de X.XXX
- **Modelo de Classificação**: Acurácia de XX.X%
- **Insights**: Principais features que influenciam o preço e classificação

## 🎓 Estrutura do Repositório

```
📦 sistema-equipamentos-industriais
├── 📄 README.md                    # Documentação principal
├── 📄 LICENSE                      # Licença MIT
├── 📁 data/
│   └── maquinas.csv               # Dataset original
├── 📁 models/
│   ├── regression_model.pkl       # Modelo de regressão treinado
│   └── classification_model.pkl   # Modelo de classificação treinado
├── 📁 notebooks/
│   ├── 01_exploratory_analysis.ipynb
│   ├── 02_data_preparation.ipynb
│   └── 03_modeling.ipynb
├── 📁 sql/
│   └── database_schema.sql        # Script de criação do banco
└── 📄 requirements.txt             # Dependências do projeto
```

## 📝 Documentação Adicional

- [Apresentação do Projeto](link-para-slides)
- [Relatório Técnico Completo](link-para-pdf)
- [Dashboard BI](link-para-dashboard)

## 🏆 Avaliação

Projeto desenvolvido seguindo a metodologia CRISP-DM:
- ✅ Entendimento do negócio
- ✅ Entendimento dos dados
- ✅ Preparação dos dados
- ✅ Modelagem (Machine Learning)
- ✅ Avaliação de performance
- ✅ Implementação e entrega

## 👨‍💻 Autor

**Seu Nome**  
📧 j.souza@edu.sc.senai.br  
🔗 [LinkedIn](https://www.linkedin.com/in/joaopiccini/)

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🙏 Agradecimentos

- **SENAI SC** - Centro Universitário SENAI de Santa Catarina
- **Professores e Orientadores** do curso CDIA 2025

---

⭐ **Se este projeto foi útil para você, considere dar uma estrela!**
