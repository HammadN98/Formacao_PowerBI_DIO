# Modelagem de Dados com Power BI

## Cursos

- Fndamentos de Modelagem dimensional
- Modelagem de dados no Power BI
- Primeiros passos com DAX e calculos com Power BI
- Otimizacao de modelos de dados com foco em desempenho no Power BI

  ## Projeto Pratico

  ### - Criando um Star Schema para um cenario de univesidade com Power BI
 
      Descrição do desafio de modelagem dimensional
      
      Objetivo:
      
      Criar o diagrama dimensional – star schema – com base no diagrama relacional disponibilizado.
      
      Foco:
      
      Professor – objeto de análise
      
      Vocês irão montar o esquema em estrela com o foco na análise dos dados dos professores.
      Sendo assim, a tabela fato deve refletir diversos dados sobre professor, cursos ministrados,
      departamento ao qual faz parte....
      Por aí vocês já têm uma ideia do que deve compor a tabela fato do modelo em questão.
      
      Obs.: Não é necessário refletir dados sobre os alunos!
      
      O que deve ser feito?
      
      Deverá ser criada a tabela Fato que contêm o contexto analisado. Da mesma forma,
      é necessária a criação das tabelas dimensão que serão compostas pelos detalhes relacionados ao contexto.
      
      Por fim, mas não menos importante, adicione uma tabela dimensão de datas.
      Para compensar a falta de dados de datas do modelo relacional, suponha que você tem acesso aos dados e crie         os campos necessários para modelagem.
      
      Ex: data de oferta das disciplinas, data de oferta dos cursos, entre outros.
      O formato, ou melhor, a granularidade, não está fixada. Podem ser utilizados diferentes formatos que                correspondem a diferentes níveis de granularidade.
  ### Modelagem e transformacaode dados com DAX ecom Power BI

      Descrição do Desafio de Projeto

      Utilizaremos a tabela única de Financial Sample para criar as tabelas dimensão e fato do nosso modelo baseado em star schema.
      
      O processo consiste na criação das tabelas com base na tabela original. A partir da cópia serão selecionadas as colunas que irão compor a visão da nova tabela. Sendo assim, a partir da tabela principal serão criadas as tabelas:
      
      Financials_origem (modo oculto – backup)
      
      D_Produtos (ID_produto, Produto, Média de Unidades Vendidas, Médias do valor de vendas, Mediana do valor de vendas, Valor máximo de Venda, Valor mínimo de Venda)
      
      D_Produtos_Detalhes(ID_produtos, Discount Band, Sale Price, Units Sold, Manufactoring Price)
      
      D_Descontos (ID_produto, Discount, Discount Band)
      
      D_Detalhes (*)
      
      D_Calendário – Criada por DAX com calendar()
      
      F_Vendas (SK_ID , ID_Produto, Produto, Units Sold, Sales Price, Discount Band, Segment, Country, Salers, Profit, Date (campos))
      
      *Verifique as informações que não foram contempladas nas demais tabelas dimensão que fornecem maiores detalhes sobre vendas.

  
      
