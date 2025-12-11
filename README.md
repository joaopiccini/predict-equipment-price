# 📊 Precificação e Classificação de Equipamentos Industriais usando ML

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Projeto Final** — Curso de Ciência de Dados e Inteligência Artificial (CDIA 2025)  
> Centro Universitário SENAI SC | Florianópolis/SC

[![Static Badge](https://img.shields.io/badge/Apresenta%C3%A7%C3%A3o_oral_do_Projeto-Google_Drive-orange)
](https://drive.google.com/file/d/1e650zAB8fuatlp94hI3tDpmX0PZC3zbd/view?usp=drive_link)

## 📋 Sobre o Projeto

Este projeto consiste em um conjunto de algoritmos de Machine Learning desenvolvidos para treinar modelos visando resolver dois problemas principais:

1. **Previsão de Preço**: Estima o preço de venda de novos equipamentos baseado em suas características técnicas
2. **Classificação de Equipamentos**: Categoriza equipamentos em classes (A, B, C, D, E) para segmentação de clientes

## 🎓 Estrutura do Projeto

```
📦 predict-equipment-price
├── 📄 README.md                    # Documentação principal
├── 📄 LICENSE                      # Licença MIT
├── 📁 data/
│   └── maquinas.csv                 # Dataset original
│   └── maquinas_normalizado.csv     # Dataset após normalização dos dados
├── 📁 docs/
│   └── Apresentação.pdf             # Apresentação do Projeto
│   └── Apresentação.mp4             # Apresentação do Projeto em Vídeo
│   └── Relatório Técnico.pdf        # Relatório Técnico Completo
├── 📁 models/
│   ├── pricer.pkl                   # Modelo de precificação treinado
│   └── classifier.pkl               # Modelo de classificação treinado
├── 📁 notebooks/
│   ├── Classificação dos Equipamentos.ipynb
│   ├── Normalização e Análise dos Dados.ipynb
│   └── Persistência dos Dados.ipynb
│   └── Previsão de Preço.ipynb
```

Projeto desenvolvido seguindo a metodologia CRISP-DM:

- ✅ Entendimento do negócio
- ✅ Entendimento dos dados
- ✅ Preparação dos dados
- ✅ Modelagem (Machine Learning)
- ✅ Avaliação de performance
- ✅ Implementação e entrega

## 📊 Dataset

O projeto utiliza dados históricos de equipamentos industriais, fornecidos por uma empresa, com as seguintes variáveis:

### Variáveis Numéricas

- **Preço**: Valor de venda do equipamento
- **Potência**: Capacidade em kW/HP
- **Peso**: Massa do equipamento (tonelada)
- **Durabilidade**: Vida útil estimada (anos)
- **Garantia**: Período de cobertura (meses)

### Variáveis Categóricas

- **Classe**: Categorização (A, B, C, D, E)
- **Tecnologia**: Tipo (convencional, automatizada, embarcada, avançada)
- **Status**: Situação atual de manutenção

### Variáveis Booleanas

- Necessidade de energia, Requer manutenção, Sistema de refrigeração, Software integrado, Conectividade IoT

## 🔧 Etapas do Projeto

### 1️⃣ **Entendimento do Negócio**

- Contextualização do problema de precificação e classificação

### 2️⃣ **Preparação dos Dados**

- Tratamento de dados faltantes
- Identificação e remoção de outliers
- Normalização e padronização de strings
- Label encoding para variáveis categóricas
- Conversão de booleanos (sim/não → 0/1)
- Padronização da coluna garantia para meses
- Matriz de correlação para seleção de features

### 3️⃣ **Modelagem de Machine Learning**

**Problema 1 - Regressão (Previsão de Preço)**

- Algoritmo: Logistic Regression
- Divisão: 80% treino / 20% teste
- Métricas: MAE, R² Score

**Problema 2 - Classificação (Categorização)**

- Algoritmo: Random Forest Classifier
- Divisão: 80% treino / 20% teste
- Métricas: Acurácia, Precisão, Recall, F1-Score, Matriz de Confusão

### 4️⃣ **Avaliação e Melhorias**

- Análise de performance dos modelos
- Identificação de limitações
- Propostas de otimização e features futuras

### 📈 Resultados

- **Modelo de Precificação**: R² Score de 0.82, MAE de 4433.46
- **Modelo de Classificação**: Acurácia de 97.3%

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

## 🚀 Como Executar

### Pré-requisitos

- Python 3.8 ou superior
- Conta no Google Colab (recomendado)

### Executando o Projeto

Baixe os notebooks do repositório e acesse diretamente no Google Colab, também é possivel executar localmente com jupyter notebook ou outras ferramentas, mas este repositório não da suporte a execução local.

## 👨‍💻 Autor

**João Piccini**  
📧 j.souza@edu.sc.senai.br  
🔗 [LinkedIn](https://www.linkedin.com/in/joaopiccini/)

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🙏 Agradecimentos

- **SENAI SC** - Centro Universitário SENAI de Santa Catarina
- **Professores e Orientadores** do curso CDIA 2025

---

⭐ **Se este projeto foi útil para você, considere dar uma estrela!**
