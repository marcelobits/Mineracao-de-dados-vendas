# Mineração de dados em um Fluxo de vendas


| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | **Mineração de dados em um Fluxo de vendas**
| :label: Tecnologias | PowerBi, Excel
| :rocket: URL         | https://bit.ly/3PxGvx7
| :fire: Desafio     |

<!-- Inserir imagem com a #vitrinedev ao final do link -->
![image](https://user-images.githubusercontent.com/44843566/207916261-e32c8278-1ffb-47c4-bb9e-f386de07de51.png)
#vitrinedev

## Detalhes do projeto

O projeto surgiu da necessidade de reestruturação do departamento de vendas e seus conceitos e regras de comissionamentos. Para isso foi necessário uma investigação da base de dados dos últimos 6 anos com a finalidade de identificar padrões do fluxo de vendas, identificar inconsistências que podem prejudicar o fluxo e procedimentos vigentes juntamente com limitações e barreiras que impedem a dinâmica necessária para aproveitar as janelas de oportunidades.

**Ferramenta de Desenvolvimento**

 Excel e Power BI

**Sobre a base de dados**

O arquivo base foi um excel parcialmente estruturado que passou pelo processo de ETL na ferramenta do Power BI


## Fluxo de desenvolvimento
![image](https://user-images.githubusercontent.com/44843566/207919907-19af2b85-cfa3-4edb-86b3-68a8fb8b4992.png)


## Modelo De visualização desenvolvido


**Home**

*Apresentação Macro da Classificação da base de Clientes.* 

Apresentando:
Base total de clientes cadastrados desde o início
Base de Foco, clientes dos últimos 6 anos
Classificação da base de clientes dos últimos 6 anos em:

 * PF e PJ
  
 * Clientes Antigos (entraram na base Antes de 2021)
  
 * Clientes Novos (entraram na base em 2021 e 2022)
  
 * Clientes Recorrentes (fizeram ao menos 1 compra por ano durante os últimos 6 anos)
  

![image](https://user-images.githubusercontent.com/44843566/207936329-daaa0125-3be2-41e9-a62d-26e85fc470ef.png)




**Dispersão**


*Classificação dispersiva da base de clientes tendo como parâmetro Valor Faturado e Quantidade de Reservas*

O objetivo desta visualização é demonstrar a Dispersão dos clientes ao longo dos anos tendo como base o volume de reservas e faturamento, facilitando a visualização da evolução da base como um todo podendo futuramente inserir uma matriz de classificação com base em sua posição no gráfico como uma balanced scorecard, como a imagem abaixo.

![image](https://user-images.githubusercontent.com/44843566/207947628-95ab2987-84d5-4722-a997-0122b01a59a2.png)





*1) Matriz de Exemplo*

![image](https://user-images.githubusercontent.com/44843566/207946795-f6cd6f3b-56c5-4f90-9f05-249c7879ae3e.png)



**Pareto 80/20**

*Representatividade em percentual de clientes que compõem cerca de 80% do faturamento*

O Objetivo desta visualização é analisar qual o mix de clientes que de forma acumulada representam uma grande fatia do faturamento. Podendo a partir desta análise fomentar uma diversificação caso seja necessário.


*O nome dos clientes foram distorcidos.
![image](https://user-images.githubusercontent.com/44843566/207952491-a1321180-f43b-414b-bffd-d0481a465bd8.png)


**Faturamento x Quantidade**

*Demonstrativo mensal, semanal e por tipo de veículo*

O objetivo desta análise é uma visualização ao longo dos meses a fim de identificar tendências mais abrangentes, tendo como referência a quantidade média dos últimos 12 meses. A análise Semanal nos ajuda a avaliar os dias da semana com maior pico de viagens executadas, nota-se que durante a semana existe uma quantidade menor de locações em comparação com o final de semana que pode se tratar de uma limitação ou apenas uma característica do negócio. Para uma avaliação mais abrangente seria necessário a quantidade de propostas realizadas também por dia de semana para avaliar se existe demanda para os dias da semana.

![image](https://user-images.githubusercontent.com/44843566/207962944-143a1a51-117d-4a26-83a1-d8f2bec900ba.png)


A mesma Base de Análise das Reservas, também foi reaproveitada para Analisar o Faturamento. Nota-se que alguns pontos mesmo sobre a mesma base apresentam movimentos diferentes como por exemplo: Durante a semana vemos que na quarta feira a uma quantidade média de 15 viagens realizadas porém analisando o faturamento médio no mesmo dia da semana nota-se que o menor valor médio também ocorre na quarta feira. Para uma análise mais abrangente também seria necessário uma avaliação das propostas enviadas e mensurar a quantidade de valores promocionais e quesitos de aplicação.

![image](https://user-images.githubusercontent.com/44843566/207965625-6566cb94-5142-4a02-a087-035df9508857.png)



**Análise Semestral**

O objetivo desta análise é apresentar uma sazonalidade que aparenta ser uma característica do negócio, podendo futuramente ser incorporada a uma previsão

*Quantidade*
![image](https://user-images.githubusercontent.com/44843566/207968549-cc8a446d-101a-41a7-856b-468455feecaa.png)

*Faturamento*
![image](https://user-images.githubusercontent.com/44843566/207968777-bc062e54-e4ea-44e7-bf04-d5d0c72a7d8d.png)


**Rentabilidade**

*Demonstrativo de Valor Faturado tanto por quilômetro vendida (planejada) e por quilômetro Executado (realizado)*

O objetivo deste painel é demonstrar o faturamento por quilômetro. O serviço ofertado como produto é o transporte que tem como uma parte de composição de Preço a Quilometragem da viagem, logo se o contratante planeja e paga por 100 quilômetro mas utiliza apenas 50 quilômetro a rentabilidade da viagem aumenta.


![image](https://user-images.githubusercontent.com/44843566/207971284-65790e95-ef1e-48f4-a0be-3d258edd8bd9.png)



**Histograma**

*Distribuição quantitativa do preço médio faturado por viagem realizada*

O objetivo deste histograma é observar a classificação e a distribuição dos valores faturados e qual é a faixa de valor médio que mais se repete.
Exemplo: 

  * No eixo horizontal observamos as faixas de valores a primeira é 375 e termina em 875
  
  * No eixo Vertical observamos a Quantidade de vezes que este valor se repete que é cerca de 21 vezes
  
nota-se que o valor médio de faturamento por viagem que se repete mais de 140 vezes é entre 2375 e 2875 no ano de 2022


![image](https://user-images.githubusercontent.com/44843566/207976784-5c91df8f-7f39-4ec1-861a-5c758bfb448e.png)


**Inconsistências**

*Quantidade de falhas dentro do fluxo de vendas*

O objetivo deste visual é demonstrar falhas no processo administrativo do fluxo de vendas e qual sua representação monetária.

![image](https://user-images.githubusercontent.com/44843566/207978203-c52f9e53-0001-45c0-ab2c-74a3fd00dcd0.png)


**Simulador**

*Simular fluxo de comissões*

O objetivo deste visual é simular cenários que auxiliem na política de comissionamento dos vendedores, a fim de alavancar movimentações em direções estratégicas.

![image](https://user-images.githubusercontent.com/44843566/207979210-d311c00f-097b-4508-b926-c2feb8024c43.png)



Gostou do Projeto ou tem alguma dúvida ou sugestão? 

Me adiciona no Linkedin: https://www.linkedin.com/in/marcelo-ferreira-dados/

