<p align="center">
  <img src="assets/logo-vassouras.png" alt="Universidade de Vassouras" width="400"/>
</p>

<h3 align="center">
  Universidade de Vassouras  
</h3>

---

### 📚 Curso: **Engenharia de Software**  
### 🖥️ Disciplina: **Inteligência Artificial e Machine Learning**  
### 👨‍🎓 Autor: **Matheus Beiruth**

---

# Graduate Admission Predictor (Keras/TensorFlow) 🎓

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red)
![Status](https://img.shields.io/badge/Status-Production-success)

## 📋 Project Overview
Esta aplicação é uma ferramenta de **Inteligência Artificial** desenvolvida para prever a probabilidade de admissão em programas de mestrado/doutoramento. Utilizando um modelo de **Rede Neural Profunda (DNN)** construído com **Keras** e **TensorFlow**, o sistema analisa métricas académicas padronizadas (como GRE, TOEFL e CGPA) para estimar a "Chance of Admit".

O projeto destaca-se pela flexibilidade, oferecendo tanto uma interface interativa via terminal quanto capacidade de processamento em lote (batch processing) para análise de grandes volumes de dados.

## 🚀 Features
* **Motor de Inferência Keras:** Carregamento eficiente de modelos pré-treinados (`.keras`) para previsões instantâneas.
* **Interactive CLI:** Interface de linha de comando robusta com validação de dados em tempo real para consultas individuais.
* **Batch Processing:** Pipeline de processamento de arquivos CSV para gerar previsões em massa, ideal para análise de múltiplos candidatos simultaneamente.
* **Data Validation:** Verificação automática de limites e tipos de dados (ex: GRE entre 260-340, TOEFL 0-120).

## 🛠️ Tech Stack
* **Core:** Python 3
* **ML Framework:** TensorFlow / Keras
* **Data Manipulation:** Pandas, NumPy
* **Model Persistence:** Keras SavedModel format

## 📊 Model Parameters
O modelo foi treinado para analisar os seguintes atributos:

| Parâmetro | Descrição | Intervalo Típico |
| :--- | :--- | :--- |
| **GRE Score** | Graduate Record Examination | 260 - 340 |
| **TOEFL Score** | Test of English as a Foreign Language | 0 - 120 |
| **University Rating** | Classificação da Universidade de origem | 1 - 5 |
| **SOP** | Força da Declaração de Propósito (Statement of Purpose) | 1 - 5 |
| **LOR** | Força das Cartas de Recomendação | 1 - 5 |
| **CGPA** | Cumulative Grade Point Average | 0 - 10 |
| **Research** | Experiência em Investigação (0 = Não, 1 = Sim) | Binário |

## ⚙️ Installation & Usage

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/BeiruthDEV/keras-admission-predictor.git](https://github.com/BeiruthDEV/keras-admission-predictor.git)
    cd keras-admission-predictor
    ```

2.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Certifique-se do Modelo:**
    Garanta que o ficheiro `modelo_treinado.keras` está na raiz do diretório.

4.  **Execute a aplicação:**
    ```bash
    python prever_admissao.py
    ```

### Modos de Operação

Ao iniciar, selecione o modo desejado:

* **Modo 1 (Single Candidate):** Responda às perguntas no terminal para uma avaliação pontual.
* **Modo 2 (Batch CSV):** Forneça o caminho de um arquivo CSV (ex: `entrada_teste.csv`) para gerar um relatório de saída (`predicoes_saida.csv`) com as probabilidades calculadas.

---
*Desenvolvido por Matheus Beiruth como parte do portfólio de Machine Learning.*
