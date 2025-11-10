🛍️ Análise de Dados de E-commerce — Olist

📊 Descrição do Projeto:

Este projeto tem como objetivo realizar uma análise exploratória e descritiva dos dados de e-commerce disponibilizados pela empresa Olist, com o intuito de extrair insights de negócio e identificar padrões sobre o comportamento de compras, desempenho logístico e receita gerada.

A base de dados contém informações detalhadas sobre pedidos, clientes, pagamentos, vendedores e entregas.

🎯 Objetivos Principais:

Analisar o volume total de pedidos e o número de clientes únicos;

Calcular a receita total;

Identificar pedidos com problemas logísticos (não entregues, não enviados ou não aprovados);

Investigar distribuições geográficas dos clientes;

Criar visualizações de dados (Seaborn/Matplotlib e Power BI) para apoiar decisões de negócio.

🧠 Principais Insights Obtidos:

Métrica	Valor / Observação

ticket médio R$205.83

Total de pedidos	98.665

Receita total	R$ 21.183.543,46

Total de clientes únicos	98665

Crescimento médio mensal	-52,10% (indicando queda de receita média nos meses analisados)

Pedidos não aprovados	15
Pedidos não enviados	1.245
Pedidos não entregues	2.567

Esses resultados indicam que há ineficiências logísticas e possíveis oportunidades de melhoria operacional no fluxo de entrega e aprovação de pedidos.

🧹 Tratamento de Dados:

Durante a limpeza e preparação da base, foram adotadas as seguintes práticas:

Análise de valores ausentes (NaN): identificados principalmente nas colunas de datas (order_approved_at, order_delivered_customer_date etc.), indicando diferentes etapas do processo logístico.

Decisão consciente de não imputar valores para manter a integridade das análises de status dos pedidos.

Conversão de variáveis de data (order_purchase_timestamp) para períodos mensais (.dt.to_period('M')) a fim de calcular crescimento e tendências temporais.

Junção de múltiplos datasets (orders, order_items, payments, customers) usando chaves relacionais (order_id, customer_id).

📈 Visualizações Criadas:

Foram utilizados Matplotlib e Seaborn para criar gráficos exploratórios, como:

Receita total por estado dos clientes (customer_state);

Distribuição de tipos de pagamento;

Evolução mensal da receita;

Proporção de pedidos entregues vs. não entregues.

Posteriormente, os dados foram conectados ao Power BI para construção de um dashboard interativo, permitindo:

Filtrar vendas por estado e categoria;

Acompanhar métricas de desempenho logístico;

Visualizar tendências de crescimento e receita total.

🛠️ Tecnologias Utilizadas:

Categoria	Ferramentas
Linguagem	Python
Bibliotecas	Pandas, NumPy, Matplotlib, Seaborn
BI / Dashboard	Power BI
Ambiente	Jupyter Notebook
Banco de dados (fonte)	Olist E-commerce Public Dataset

🧾 Conclusão:

O projeto demonstra domínio completo do ciclo analítico:

Coleta e integração de múltiplas fontes de dados;

Limpeza e preparação cuidadosa;

Cálculo de métricas de negócio relevantes;

Comunicação visual e interpretação de insights.

✍️ Autor:
Fellipe Abrantes
📧 fellipeabrantesoares@gmail.com 

🔗 LinkedIn https://www.linkedin.com/in/fellipe-abrantes-772a76354/
 
