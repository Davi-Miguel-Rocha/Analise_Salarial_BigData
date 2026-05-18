# Analise_Salarial_BigData

# 📊 Inteligência de Mercado: Predição e Projeção Salarial em Data Science com Deep Learning

Este projeto aplica conceitos avançados de **Big Data** e **Deep Learning** para analisar, prever e projetar tendências salariais no mercado global de Ciência de Dados. Utilizando uma rede neural artificial desenvolvida em **TensorFlow/Keras**, o modelo é capaz de mapear o impacto de variáveis categóricas complexas (como cargos específicos e localizações geográficas) e prever a valorização de carreiras até o ano de 2027.

---

## 🚀 Funcionalidades do Projeto

* **Pipeline de Big Data Automatizado:** Processamento robusto de dados categóricos de alta cardinalidade utilizando `OneHotEncoder`.
* **Modelo Preditivo Estabilizado:** Rede neural multicamadas otimizada com o algoritmo `RMSprop` e técnicas de regularização (`Dropout`) para evitar que o modelo *decore os dados*.
* **Simulador de Cenários Futuros:** Função integrada para predição de salários de novos perfis profissionais baseando-se em tendências temporais.
* **Análise Comparativa de Mercado (Duelo de Valorização):** Projeção visual comparando o crescimento das duas maiores carreiras do setor (Data Scientist vs. Data Engineer) para os próximos anos.

---

## 🛠️ Arquitetura e Tecnologias

### Ferramentas e Bibliotecas
* **Linguagem:** Python
* **Ambiente:** Google Colab (Suporte a aceleração por GPU T4)
* **Manipulação de Dados:** `pandas`, `numpy`
* **Machine Learning & Pré-processamento:** `scikit-learn`
* **Deep Learning:** `TensorFlow 2.x` / `Keras`
* **Visualização de Dados:** `matplotlib`, `seaborn`

### Estrutura da Rede Neural (Sequential)
1.  **Camada de Entrada (Dense):** 128 neurônios, ativação `ReLU` (ajustada dinamicamente à dimensionalidade do One-Hot Encoding).
2.  **Camada de Regularização (Dropout):** Taxa de 20% para garantir o poder de generalização do modelo.
3.  **Camadas Ocultas (Dense):** Duas camadas intermediárias de 32 neurônios e uma de 16 neurônios com ativação `ReLU`.
4.  **Camada de Saída (Dense):** 1 neurônio com ativação linear (regressão do valor salarial em USD).

---

## 📈 Resultados obtidos

### 1. Evolução do Aprendizado
O modelo exibiu uma curva de aprendizado extremamente saudável e otimizada pelo ajuste de processamento em lotes (`batch_size=256`).

* **Métrica de Erro:** Erro Médio Absoluto (MAE).
* **Erro Médio Final:** **~$42,389.36** por salário.
* **Análise Técnica:** O erro residual representa a variância natural e não observada do mercado de tecnologia (fatores como stacks tecnológicas específicas, bônus corporativos e flutuações de ações). As curvas de Treino e Validação convergiram perfeitamente de forma síncrona, eliminando qualquer indício de que o modelo *decorou os dados* ou *não aprendeu com eles*.

### 2. Projeção de Mercado: Data Scientist vs. Data Engineer (2024 - 2027)
Ao interrogar o modelo para simular profissionais de nível Sênior atuando nos Estados Unidos em modelo Remoto, a inteligência artificial revelou os seguintes insights:

* **Tendência Macroeconômica:** O modelo identificou um vetor de crescimento linear positivo para o mercado de dados como um todo até 2027.
* **Diferencial de Carreira (2027):**
    * **Senior Data Scientist:** Projeção de **$102.910,00**
    * **Senior Data Engineer:** Projeção de **$92.917,00**
* **Insight de Negócio:** Embora o mercado esteja em expansão uniforme para ambas as frentes, o modelo detectou uma valoração historicamente superior (~10%) para a vertente estatística/analítica (Data Scientist) em relação à infraestrutura de dados (Data Engineer).

---

## 💻 Como Executar o Projeto no Google Colab

1.  Abra o ambiente do [Google Colab](https://colab.research.google.com/).
2.  Faça o upload do arquivo de dados `data_science_salaries.csv` na pasta lateral do ambiente.
3.  Copie e execute as células de código organizadas no notebook.
4.  *(Opcional)* Para ganho máximo de performance devido ao grande volume de colunas gerado pelo One-Hot Encoding, ative o acelerador de hardware em: `Ambiente de Execução > Alterar tipo de ambiente de execução > GPU T4`.

---

## 👥 Autores e Desenvolvimento

* **Desenvolvedor:** Davi Miguel da Rocha Lima
* **Contexto:** Projeto Prático de Big Data e Sistemas Preditivos da aula de tópicos de bigData em python.
