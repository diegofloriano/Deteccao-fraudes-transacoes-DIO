# Detecção de Fraudes em Transações Financeiras 💳🚨

Projeto prático desenvolvido para o desafio de Machine Learning da **Digital Innovation One (DIO)**, focado na criação, avaliação e otimização de modelos preditivos para identificação de transações fraudulentas em sistemas financeiros.

---

## 📌 Sobre o Projeto

A detecção de fraudes em transações de cartão de crédito e meios de pagamento digitais apresenta um desafio central em Ciência de Dados: o **extremo desbalanceamento das classes**, onde transações legítimas representam a quase totalidade do volume e as fraudes constituem uma fração ínfima do dataset.

O objetivo deste projeto é aplicar o pipeline completo de aprendizado de máquina em Python para tratar o desbalanceamento de dados, realizar a análise exploratória, treinar classificadores e avaliar o desempenho utilizando métricas adequadas a cenários com alta assimetria de classes.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Análise e Manipulação de Dados:** Pandas, NumPy
* **Visualização de Dados:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn
* **Balanceamento de Dados:** Imbalanced-Learn (`imblearn`)
* **Ambiente de Execução:** Jupyter Notebook

---

## 📂 Estrutura do Repositório

```plaintext
Deteccao-fraudes-transacoes-DIO/
│
├── data/                  # Datasets utilizados na análise
├── notebook/              # Análise exploratória e modelagem
└── README.md              # Documentação do projeto
```

---

## 🔄 Pipeline do Projeto

1. **Análise Exploratória de Dados (EDA):**
   * Avaliação da distribuição do volume financeiro (`Amount`) e do tempo (`Time`).
   * Análise da proporção entre transações legítimas (Classe 0) e fraudulentas (Classe 1).

2. **Pré-Processamento:**
   * Normalização e padronização de atributos usando `StandardScaler`.
   * Separação dos dados em conjuntos de treino e teste mantendo a proporção das classes (`stratify`).

3. **Tratamento de Desbalanceamento:**
   * Aplicação de técnicas de reamostragem (*Undersampling* e/ou *Oversampling/SMOTE*) no conjunto de treino para evitar que os modelos apresentem viés em favor da classe majoritária.

4. **Treinamento e Modelagem:**
   * Treinamento e validação de algoritmos de classificação (Regressão Logística, Árvores de Decisão e Random Forest).

5. **Avaliação de Métricas:**
   * Análise focada em **Recall** (sensibilidade para capturar o maior número possível de fraudes), **Precision**, **F1-Score**, **Matriz de Confusão** e **AUC-ROC**.

---

## 📊 Principais Resultados

* A aplicação das técnicas de reamostragem permitiu aumentar drasticamente o **Recall** do modelo, reduzindo a taxa de falsos negativos (fraudes não detectadas).
* A padronização das variáveis de entrada evitou distorções nos limites de decisão dos algoritmos baseados em distância e gradiente.

---

## 🚀 Como Executar o Projeto

1. **Clonar o repositório:**
   ```bash
   git clone [https://github.com/diegofloriano/Deteccao-fraudes-transacoes-DIO.git](https://github.com/diegofloriano/Deteccao-fraudes-transacoes-DIO.git)
   cd Deteccao-fraudes-transacoes-DIO
   ```
2. **Instalar as dependências:**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn jupyter
   ```
3. **Iniciar o Jupyter Notebook:**
   ```bash
   jupyter notebook Deteccao_fraudes_transacoes_DIO.ipynb
   ```

## ✒️ Autor

Desenvolvido por Diego FLoriano.

