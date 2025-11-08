
<img width="1024" height="1024" alt="Gemini_Generated_Image_vbcaetvbcaetvbca" src="https://github.com/user-attachments/assets/fd1ba14a-52cf-4b10-b400-c058fd93c403" />

# 1. Problema de negócio
    
SuperStore, uma grande rede de supermercados com múltiplas unidades físicas, enfrenta o desafio de integrar dados para melhorar a tomada de decisão. Atualmente, os gerentes dependem de planilhas pontuais, resultando em indicadores desalinhados. O principal objetivo é estabelecer um conjunto unificado de indicadores.
Você foi contratado como Analista de Dados para o novo time, sendo responsável por criar esses indicadores a partir de dados transacionais da empresa. Seu primeiro desafio é analisar os pedidos de compra.
A análise deve focar em descrever o comportamento dos clientes—incluindo quais produtos mais compram, a quantidade, o valor médio da cesta e a frequência de pedidos. todas as análises em conjunto com as segmentações, para ter um melhor entendimento do desempenho

O Problema de Negócio (O Desafio de Gestão)

1.Primeiro desafio:

Como estão indo os pedidos da SuperStore?

2.Segundo desafio:

Medir a retenção de clientes.
    
## Dado da empresa
    
Análise Descritiva

## Passo 1: Definição do Fato
- Coluna “Order ID”

## Passo 2: Definição das Dimensões
- Order Date Tempo
- Ship Data Tempo
- Ship Mode Entrega
- Sales Produto
- Discount Produto
- Product Produto

## Passo 3: Combinação Fato-Dimensão
- Quantidade de Pedidos por Data ( Dia, Mês, Ano, Semana, Feriado )
- Quantidade de Pedidos por Data de Envio ( Dia, Mês, Ano, Semana,
Feriado )
- Quantidade de Pedidos por Tier de Preço ( Baixo, Médio, Alto )
- Quantidade de Pedidos por Quantidade de Itens
- Quantidade de Pedidos por Tier de desconto ( Baixo, Médio, Alto )
- Quantidade de Pedidos por Produto
- Quantidade de Pedidos por Clientes
- Quantidade de Pedidos Por Data e Tier de Preço
- Quantidade de Pedidos Por Data e Quantidade de Itens
- Quantidade de Pedidos por Data e Produto
- Quantidade de Pedidos por Data e Clientes
- Quantidade de Pedidos por Data de Envio e Tier de Preço

# 2. Premissas do negócio
    
1. A análise foi realizada com datas entre 15/09/2016  e 03/09/2018 .    
2. Varejo foi o modelo de negócio assumido.    
3. Os 3 principais visões de negócio foram: visão vendas, visão pedidos, Retenção dos clientes.
    
# 3. Estratégia da solução
  O painel estratégico foi desenvolvido ultilizando as métricas que refletem as 3 principais visões do modelo de negócio da empresa:
    
  1. Visão vendas
  2. Visão pedidos
  3. Retenção dos clientes
    
Cada visão é representada pelo seguinte conjunto de métricas.
    
1. Visão vendas
    1. Faturamento
    2. Total de produtos vendidos
    3. Lucro percentual
    4. Volume de venda pelo modo de envio
    5. Quantidade de produto, quantidade de clientes único, média de produto por cliente x Mês
    6. Evolução mensal faturamento e lucro percentual
    7. Lucro por categoria
        
2. Visão pedidos
    1. Total de pedidos
    2.  percentual de crescimento (2016-2017)
    3.  Média de pedido por cliente
    4.  Quantidade de pedido por região
    5.  Top 10 Estados com maior volume de pedidos
    6.  Evolução de crescimento e volume de pedido por Ano
    7.  Composição de pedido por categoria do produto
        
3. Retenção dos clientes:

    i. Coluna order_date

    ii. Coluna custumer_id
     
    --> Com a coluna order_date, derivamos a coluna :        
       
   1. Mês de aquisição
        
    2. Mês decorrido
          
   Análise foi feita no ano  2014, período de  12 meses
        
# Top 4 insights de dados
  1. Lucro por categoria,
     A categoria que traz o maior lucro pra empresa é : Technology
        
  2. Média de produto por cliente:
     Em média, são de 2 a 3 produtos por clientes
        
  3. Distribuição e Lucratividade (Geografia e Categoria):
    
     A distribuição dos pedidos por Região e Categoria de Produto, comparada ao volume de pedidos
     "A Região 'Sul', tem menor volume de pedidos, o que está acontecendo? Tempo de entrega demorando muito? Um ponto a ser analisado."
        
  4. Cohot--> queda drástica inicial:
 
  **Insight Chave:** O negócio tem uma perda de clientes muito acentuada após o primeiro mês.
  **Detalhe:** Observe que a maioria das coortes (as linhas) cai para menos de 50% de retenção no Mês 1 e continua caindo rapidamente nos meses subsequentes. 
  Isso é esperado, mas mostra que a experiência inicial do cliente (onboarding, primeiro pedido, pós-venda) precisa ser drasticamente melhorada.
        
# O produto final
  
  Dashboard Online, na ferramenta power Bi online e disponível para acesso em qualquer dispositivo conectado à internet.
  O painel pode ser acessado através desse link:https://app.powerbi.com/view?r=eyJrIjoiOGYzOTRkZmItMzFmZC00ZmJkLTkxZGYtZThmNjNmYjUzZDljIiwidCI6ImZiY2ExYWE5LTAxMDEtNDRlNC1iZmU1LWEyODRjNzA0YjIyMCJ9&pageName=3074463d7b3344ab037a
    
# Conclusão
   
   O objetive desse projeto foi cria um conjunto de gráficos ou tabelas que exibam essas métricas da melhor forma possível para o CEO.
  
Da visão da Empresa, podemos concluir que entre os anos de 2014-2017, mesmo com uma grande queda no número percentual da retenção dos clientes logo no segundo mês,
 a Empresa segue com um crescimento de 28% no número de pedidos



    
