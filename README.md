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
* **Performance:** O modelo final alcançou uma performance robusta, com foco principal em **identificar corretamente os clientes insatisfeitos (Recall)**, conseguindo capturar **[INSERA AQUI O VALOR DO RECALL DA CLASSE '1' DO SEU MODELO FINAL, ex: 65%]** dos clientes verdadeiramente insatisfeitos no conjunto de teste.
* **Principal Conclusão do Modelo:** A análise de *feature importance* confirmou que o **`tempo_de_entrega`** é, de longe, o fator mais preditivo para a insatisfação, validando a principal descoberta da nossa EDA e fornecendo uma direção clara para a otimização do negócio.

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
|--📁.venv/                # Ambiente virtual com as dependências
|--📁 dados/                # Contém todos os arquivos .csv do dataset Olist
|--📁 notebooks/            # Contém os notebooks da análise e do modelo
|   |--📄01_analise_exploratoria.ipynb
|   |--📄02_modelo_ml_satisfacao.ipynb
|--📄 README.md             # Este arquivo de documentação
|--📄requirements.txt      # Arquivo com as bibliotecas Python necessárias
```

---

## ⚙️ Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/Kudo-San/analise-ecommerce-olist.git
    ```
2.  **Navegue até a pasta do projeto:**
    ```bash
    cd [NOME_DO_SEU_REPOSITORIO]
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

## 👨‍💻 Autor
**Marcelo Kudo**

## 💬 Sobre mim

**Engenheiro de Machine Learning & Especialista em Automação Industrial** 💡 **Foco:** IIoT | Análise de Dados | IA Industrial  

Profissional com **+18 anos de experiência em tecnologia** unindo **Automação Industrial**, **Análise de Dados** e **Inteligência Artificial**, aplicando tecnologia para otimizar processos industriais.  
Desenvolvo **modelos de Machine Learning** voltados à **manutenção preditiva** e **otimização de desempenho**, com foco em **integração direta com sistemas de controle**.

---

### ⚙️ Competências Técnicas
- 🧠 **Machine Learning:** TensorFlow, PyTorch, Keras  
- 🐍 **Programação:** Python (Pandas, NumPy), SQL  
- 📊 **Análise e Visualização:** Power BI, Dashboards de KPI’s  
- 🏭 **Automação & IIoT:** CLPs, IHMs, Edge AI, Rockwell, Mitsubishi, Schneider, além de Edge AI e sistemas de visão embarcada.

---

🎯 **Missão:** Conectar **Inteligência Artificial à operação fabril**, transformando dados em decisões automatizadas e resultados reais.  
🚀 **Interesses:** Indústria 4.0, MLOps, Edge Computing e Realidades Aumentada e Mista.

[comment]: <> (Link para o LinkedIn)
[<img align="left" alt="Marcelo Kudo | LinkedIn" width="24px" src="https://www.vectorlogo.zone/logos/linkedin/linkedin-icon.svg" />][linkedin]

[comment]: <> (Link para o GitHub)
[<img align="left" alt="Marcelo Kudo | GitHub" width="24px" src="https://www.vectorlogo.zone/logos/github/github-tile.svg" />][github]

[linkedin]: https://www.linkedin.com/in/[SEU_LINKEDIN_AQUI]
[github]: https://github.com/[SEU_USUARIO_DO_GITHUB]
