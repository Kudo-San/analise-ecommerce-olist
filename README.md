
<img width="1024" height="750" alt="Gemini_Generated_Image_4vx6hq4vx6hq4vx6" src="https://github.com/user-attachments/assets/301fc04c-6d6f-4e2e-8307-5f17b59a90aa" />


# 📊 Análise Exploratória de Dados do E-commerce Olist

Este repositório contém uma análise exploratória de dados (EDA) detalhada sobre o dataset público de e-commerce brasileiro da Olist. O objetivo deste projeto é extrair insights valiosos sobre o comportamento de vendas, a satisfação do cliente, o desempenho de categorias e vendedores, padrões de pagamento e a segmentação de clientes.

A análise foi conduzida utilizando Python em um ambiente Jupyter Notebook, com foco na manipulação de dados e na criação de visualizações claras para comunicar as descobertas.

## 🛠️ Tecnologias e Bibliotecas Utilizadas

* **Python 3**
* **Pandas:** Para manipulação e análise dos dataframes.
* **Matplotlib & Seaborn:** Para a criação de gráficos e visualizações de dados.
* **NumPy:** Para operações numéricas.
* **Jupyter Notebook:** Como ambiente de desenvolvimento interativo.

## 📦 Dataset

O conjunto de dados utilizado é o [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce), disponível no Kaggle. Ele contém informações sobre cerca de 100.000 pedidos realizados entre 2016 e 2018, distribuídos em múltiplos arquivos que abrangem:

* Pedidos (orders)
* Clientes (customers)
* Itens do pedido (order_items)
* Pagamentos (payments)
* Avaliações (reviews)
* Produtos (products)
* Vendedores (sellers)
* Geolocalização (geolocation)

## 📈 Análises Realizadas e Principais Insights

O notebook aborda diversas questões de negócio, gerando insights importantes:

1.  **Análise de Faturamento por Estado:**
    * **Pergunta:** Onde estão concentradas as vendas da Olist?
    * **Insight:** O faturamento é fortemente concentrado na Região Sudeste, com São Paulo representando a maior parte das receitas.

2.  **Relação entre Tempo de Entrega e Satisfação do Cliente:**
    * **Pergunta:** Clientes que recebem seus produtos mais rápido dão notas melhores?
    * **Insight:** Sim, existe uma forte correlação. O tempo mediano de entrega para avaliações nota 1 é quase o dobro do tempo para avaliações nota 5, indicando que a logística é um fator crítico para a satisfação.

3.  **Análise de Categorias de Produtos:**
    * **Pergunta:** As categorias que mais vendem em volume são as que mais faturam?
    * **Insight:** Não necessariamente. Categorias como "Cama, Mesa e Banho" lideram em ambos, mas categorias com "ticket médio" (preço médio) mais alto, como "Relógios e Presentes", aparecem no topo de faturamento sem estar no topo de volume de vendas.

4.  **Análise de Vendedores (Sellers):**
    * **Pergunta:** O sucesso é concentrado em poucos vendedores? Onde eles estão?
    * **Insight:** O mercado de vendedores é dinâmico, com a elite de top sellers se renovando a cada ano. A maior parte do faturamento gerado por vendedores também está concentrada no estado de São Paulo.

5.  **Análise de Pagamentos:**
    * **Pergunta:** Como os clientes pagam e parcelam suas compras?
    * **Insight:** O cartão de crédito é o método dominante. A análise de parcelamento mostra uma preferência por pagamentos à vista (1x), mas com um volume considerável de compras parceladas em 2, 3 e 10 vezes.

6.  **Segmentação de Clientes (RFM):**
    * **Técnica:** Utilização do modelo RFM (Recência, Frequência, Valor Monetário) para criar segmentos de clientes.
    * **Insight:** A análise identificou perfis distintos como "Campeões" (compram muito e com frequência), "Clientes em Risco" (compraram bem, mas há muito tempo) e "Clientes Hibernando" (a maior base, com compras antigas e de baixo valor), permitindo a criação de estratégias de marketing direcionadas.

## 🚀 Como Executar o Projeto

Para replicar esta análise, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/Kudo-San/analise-ecommerce-olist.git
    ```

2.  **Navegue até a pasta do projeto:**
    ```bash
    cd seu-repositorio
    ```

3.  **Crie e ative um ambiente virtual (recomendado):**
    ```bash
    # Para Windows
    python -m venv .venv
    .venv\Scripts\activate

    # Para macOS/Linux
    python3 -m venv .venv
    source .venv/bin/activate
    ```

4.  **Crie o arquivo de dependências `requirements.txt`:**
    * No seu terminal com o ambiente ativado, execute o comando abaixo para gerar o arquivo com as bibliotecas que você usou:
    ```bash
    pip freeze > requirements.txt
    ```
    * **Importante:** Se você ainda não instalou as bibliotecas, instale-as primeiro (`pip install pandas matplotlib seaborn jupyter`) e depois gere o arquivo.

5.  **Instale as dependências (para outra pessoa que clonar seu repositório):**
    ```bash
    pip install -r requirements.txt
    ```

6.  **Inicie o Jupyter Notebook:**
    ```bash
    jupyter notebook analise_e-commerce_olist.ipynb
    ```

## 📂 Estrutura do Repositório

* ├── 📁 `Analise_E-commerce/` : Pasta dos arquivos.
* │   ├── 📁 `Varios dataset olist.csv` : Pasta com os dados da Olist.
* 📄 `analise_e-commerce_olist.ipynb` : O Jupyter Notebook com todo o código da análise.
* 📄 `.gitignore`
* 📄 `README.md` :Este arquivo de documentação.
* 📄 `requirements.txt` : Arquivo com as bibliotecas Python necessárias.

## 👨‍💻 Autor
**Marcelo Kudo**

## 💬 Sobre mim

**Engenheiro de Machine Learning & Especialista em Automação Industrial**  
💡 **Foco:** IIoT | Análise de Dados | IA Industrial  

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
