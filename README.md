<img width="1024" height="750" alt="Gemini_Generated_Image_4vx6hq4vx6hq4vx6" src="https://github.com/user-attachments/assets/301fc04c-6d6f-4e2e-8307-5f17b59a90aa" />

# 📊 Análise de Dados e Modelo de Machine Learning para o E-commerce Olist

![Python](https://img.shields.io/badge/Python-3.11%2B-%233776AB?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Análise-%23150458?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualização-%233776AB?logo=seaborn)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-%23F7931E?logo=scikit-learn)

Este repositório contém um projeto completo de Ciência de Dados, desde uma análise exploratória de dados (EDA) detalhada até a construção de um modelo de Machine Learning para prever a satisfação do cliente, utilizando o dataset público de e-commerce brasileiro da Olist.

---

## 🎯 Objetivo do Projeto

O objetivo principal deste projeto é duplo:

1.  **Análise Exploratória (EDA):** Realizar uma investigação profunda nos dados para extrair insights acionáveis sobre a performance do negócio, incluindo padrões de vendas, geografia de clientes e vendedores, logística, satisfação do cliente e desempenho das categorias de produtos.
2.  **Machine Learning:** Construir e avaliar um modelo de classificação capaz de prever a probabilidade de um cliente ficar insatisfeito (dar uma nota de avaliação baixa), permitindo que a empresa atue proativamente para mitigar experiências negativas.

---

## 🚀 Principais Insights e Descobertas

A análise revelou diversos padrões e oportunidades de melhoria para o negócio:

* **Insight 1: Tempo de Entrega é o Fator Crítico para a Satisfação.** A EDA e o modelo de Machine Learning confirmaram que o tempo de entrega é o principal fator que influencia a nota de avaliação do cliente. Pedidos com notas baixas (1-3) tiveram uma mediana de entrega significativamente maior do que os com notas altas (4-5).

* **Insight 2: Concentração Geográfica de Clientes e Vendedores.** O faturamento é massivamente concentrado em clientes e vendedores do estado de São Paulo (SP), que atua tanto como o principal mercado consumidor quanto como o principal polo de vendas.

* **Insight 3: Alta Competitividade e Renovação na Elite de Vendedores.** A análise anual dos top vendedores mostrou que a liderança do mercado é altamente dinâmica, com poucos vendedores conseguindo se manter no topo por anos consecutivos, indicando um ecossistema saudável e competitivo.

* **Insight 4: Segmentação RFM Revela Oportunidades de Marketing.** A análise RFM (Recência, Frequência, Valor Monetário) mostrou que uma grande parte da base de clientes se enquadra nos segmentos "Hibernando" ou "Em Risco", indicando uma grande oportunidade para campanhas de reativação. O segmento "Campeões", embora pequeno, é responsável por uma parcela desproporcional do faturamento.

---

## 🤖 Modelo de Machine Learning: Previsão de Satisfação

Para transformar os insights em uma ferramenta preditiva, foi desenvolvido um modelo de Machine Learning.

* **Problema de Negócio:** Prever se um cliente ficará insatisfeito (nota de avaliação de 1 a 3) com base nos dados do pedido.
* **Metodologia:** Foi treinado um modelo `RandomForestClassifier`. A técnica **SMOTE** foi utilizada para tratar o desbalanceamento de classes (muito mais clientes satisfeitos do que insatisfeitos), garantindo que o modelo aprendesse a identificar corretamente a classe minoritária.
* **Performance:** O modelo final alcançou uma boa performance, com foco principal em **identificar corretamente os clientes insatisfeitos (Recall)**, conseguindo capturar **45%** dos clientes verdadeiramente insatisfeitos no conjunto de teste.
* **Principal Conclusão do Modelo:** A análise de *feature importance* confirmou que o **`tempo_de_entrega`** é, de longe, o fator mais preditivo para a insatisfação, validando a principal descoberta da EDA e fornecendo uma direção clara para a otimização do negócio.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

* **Linguagem:** Python
* **Análise de Dados:** Pandas, NumPy
* **Visualização de Dados:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn, Imbalanced-learn (para SMOTE)
* **Ambiente:** Jupyter Notebook, VS Code

---

## 📂 Estrutura do Projeto

O projeto está organizado de forma modular para garantir clareza e reprodutibilidade, seguindo as melhores práticas da indústria:

```
/
|--📁.venv/                 # Ambiente virtual com as dependências
|--📁 dados/                # Contém todos os arquivos .csv do dataset Olist
|--📁 notebooks/            # Contém os notebooks da análise e do modelo
|   |--📄01_analise_exploratoria.ipynb
|   |--📄02_modelo_ml_satisfacao.ipynb
|--📄 README.md             # Este arquivo de documentação
|--📄requirements.txt       # Arquivo com as bibliotecas Python necessárias
```

---

## ⚙️ Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/Kudo-San/analise-ecommerce-olist.git
    ```
2.  **Navegue até a pasta do projeto:**
    ```bash
    cd [Analise_E-commerce]
    ```
3.  **Crie e ative o ambiente virtual:**
    ```bash
    python -m venv .venv
    .\.venv\Scripts\activate
    ```
4.  **Instale as dependências:**
    *(Nota: Antes de enviar para o GitHub, rode o comando `pip freeze > requirements.txt` no seu terminal ativado para criar este arquivo.)*
    ```bash
    pip install -r requirements.txt
    ```
5.  **Abra a pasta `notebooks` e execute os arquivos `.ipynb` em ordem.**

---

<h1 align="center">🧑🏻‍💻 Marcelo Kudo</h1>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&duration=4000&pause=1500&color=00D9FF&center=true&vCenter=true&width=700&lines=🚀+Especialista+em+IA+e+Automação+Industrial;🤖+Machine+Learning+%7C+Visão+Computacional+%7C+IIoT;🏭+CLP+%7C+Robô+Industrial+%7C+UR+%7C+NVIDIA;⚙️+Indústria+4.0+;✨+Desenvolvendo+soluções+que+geram+impacto+" alt="Header animado">
</p>

---

<div align="center">
  
## 🛠️ **Stack Tecnológico**

### 🤖 **Inteligência Artificial & Machine Learning**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

### ⚙️ **Automação Industrial**
![CLP](https://img.shields.io/badge/CLP-0065B3?style=for-the-badge&logo=rockwellautomation&logoColor=white)
![Robô Industrial](https://img.shields.io/badge/Robô_Industrial-FF0000?style=for-the-badge&logo=robot&logoColor=white)
![UR](https://img.shields.io/badge/Universal_Robots-000000?style=for-the-badge&logo=universalrobots&logoColor=white)
![IIoT](https://img.shields.io/badge/IIoT-0088CC?style=for-the-badge&logo=iot&logoColor=white)

### 🖥️ **Hardware & Sistemas**
![NVIDIA Jetson](https://img.shields.io/badge/NVIDIA_Jetson-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=white)

### 📊 **Análise de Dados & Visualização**
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

</div>

---
<div align="center">

## 🧠 **Sobre Mim**

Profissional com expertise entre **automação industrial** e **inteligência artificial**, focando em desenvolver soluções para a **Indústria 4.0**.

### 🎯 **Expertise Técnica**

| **Área** | **Competências** |
|----------|------------------|
| **🤖 Automação Industrial** | Programação de CLP's, IHM, Inversor de Frequência |
| **👁️ Visão Computacional** | OpenCV, PyTorch, detecção de defeitos, classificação, aplicações industriais |
| **🧠 Machine Learning** | Modelos preditivos, redes neurais, scikit-learn, TensorFlow |
| **⚡ Edge Computing** | NVIDIA Jetson, otimização para hardware embarcado |
| **🤝 Robótica** | Robôs colaborativos UR, robótica industrial |
| **🌐 IIoT** | Integração de sistemas, protocolos industriais |
| **📊 Análise de Dados** | Pandas, NumPy, análise exploratória, visualização com Seaborn/Matplotlib |
| **📈 Dashboards** | Streamlit, Power BI, SQL, relatórios interativos para tomada de decisão |

"Tecnologia é poderosa quando resolve problemas reais."

</div>
