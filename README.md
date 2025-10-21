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
    git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
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
.
├── 📁 dados/
│   ├── olist_customers_dataset.csv
│   └── ... (outros arquivos)
├── 📄 analise_e-commerce_olist.ipynb
├── 📄 .gitignore
├── 📄 LICENSE
├── 📄 README.md
└── 📄 requirements.txt

## 👨‍💻 Autor

**Marcelo Kudo**
