# Projeto_DIO_Dashboard_XBOX
- [Link para o Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMDE1ZDRlMTItNThhOS00NDkyLTgzYjMtZjM4OTNiYjI1NjQwIiwidCI6ImEwMmZiN2Y3LTM2ZTItNDU2Yy04MWI5LTRkZWJjMTI1MzkyNiJ9)

## Introdução e Objetivo
- Este dashboard foi desenvolvido usando **dados fictícios** referentes ao período de um ano das assinaturas dos clientes de diferentes planos e passes da empresa XBOX. 
- O objetivo é fornecer informações sobre a performance dos serviços XBOX ao longo de um ano, permitindo o acompanhamento das receitas dos tipos de assinaturas, renovações e o impacto de cupons de desconto no faturamento final.
    - [Link para os dados do dashboard]()

## Visão geral dos dados
1. Subscriber ID
2. Name
    - Nomes dos clientes que assinaram algum plano, consequentemente assinaram algum passe ou não.
3. Plan
    - Existe 3 planos para o assinante escolher "Core, Standard e Ultimate". O Core è o mais basico custando 5 reais e não libera nenhum passe, Standard custa 10 reais e libera o passe do Minecraft, Ultimate custa 15 reais e libera os dois passes, do Minecraft e EA Play.
4. Start Date 
    - A data que os assinantes assinaram os serviços da XBOX
5. Auto Renewal 
    - Informa se o cliente renovou o plano ou não. Se o serviço expirou e o cliente não renovou o plano, o sistema registra novamente o cliente no banco de dados. Esse processo se repete até o cliente renovar o plano.
6. Subscription Price
    - Preço dos planos "Core, Standard e Ultimate"
7. Subscription Type
    - Periodo de validade que o cliente pode escolher para sua assinatura (Annual = Anual),(Monthly = Mensal) e (Quartely = Trimestral).
8. EA Play Season Pass
    - Indica se o cliente assinou o plano de EA Play, um serviço de assinatura que oferece acesso a uma biblioteca de jogos da Electronic Arts, benefícios exclusivos e descontos em compras de jogos.
9. EA Play Season Pass Price
    - Indica o valor da assinatura do passe da EA custando 30 reais e se o clinte assinou ele.
10. Minecraft Season Pass
    - Indica se o cliente assinou o plano de Minecraft, que oferece benefícios exclusivos, como skins, pacotes de conteúdo e outras vantagens dentro do jogo.
11. Minecraft Season Pass Price
    - Indica o valor da assinatura do passe do Minecraft custando 20 reais e se o clinte assinou ele.
12. Coupon Value
    - Valores dos descontos dos cupoms que o cliente pode usar, quanto mais o cliente gasta com o serviço, mais alto pode ser o valor do seu cupom. São 10 valores de cupons; 1,00/2,00/3,00/5,00/7,00/8,00/10,00/12,00/15,00/20,00
13. Total Value 
    - Total que cada cliente gastou com o serviço da XBOX, descontando o valor do cupom.

# Explicação dos Visuais do Dashboard
- **Filtros:**
    - Auto Renewal; 
        - Filtra as assinaturas que tem renovação ou não.
    - Coupon Value;
        - Valores dos cupoms que os clientes usaram.
    - Subscription Type
        - Filtra os tipos de inscrição.
    - Plan
        - Filtra os planos que o cliente escolheu.
    - Mês
        - Filtra cada mês do ano.

- **Cartões**
1. Cartão Total Value;
    - **Soma de Total Value (R$ 7,633 Mil):**
        - Valor total já descontado das assinaturas.
    - **Assinantes (295):**
        - Clientes que assinaram algum serviço do XBOX no ano de 2024.
    - **Average Total Value (R$ 25,87):**
        - Gasto médio de cada cliente ao final da compra. 
    - **Median Total Value (R$ 20,00):**
        - Valor central dos gastos dos clientes. Entende-se que metade dos clientes gasta até este valor.
    - **Max Total Value (R$ 62,00):**
        - Valor da compra mais alta feita por 21 clientes. Totalizando (**R$ 1.302,00**). Destacando que 13 clientes não renovaram o plano, ficando apenas 8 com a renovação ativa. 
    - **Min Total Value (R$ 3,00 ):**
        - Valor da compra mais baixa feita por 11 clientes. Totalizando (**R$33,00**). Apenas 2 tem renovação e todos usaram o cupom de 2 reais
2. Cartão Total Coupon;
    - **Total Coupon (R$ 2.122,00):**
        - Valor Total dos cupons usados. 
    - **Quantidade (244):**
        - Os cupons mais usados são o de valor R$15,00 com 46 e o de R$10,00 com 44.
3. Pass Minecraft;
    - **Pass Minecraft (R$ 3.880,00)**
        - Valor total arrecadado do passe com valor de 20 reais. Apenas liberado com os planos: Standard e Ultimate
    - **Assinantes (194)**
        - Clientes que assinaram o passe Minecraft.
4. Pass EA Play;
    - **Pass EA Play (R$ 2.940,00)**
        - Valor total arrecadado do passe com valor de 30 reais. Apenas liberado com o plano Ultimate.
    - **Assinantes (98)**
        - Clientes que assinaram o passe EA Play.
   
## Insights:
- **Baixo ticket médio pode indicar sensibilidade ao preço**
    - Gasto médio por cliente: R$ 25,87
    - Mediana: R$ 20,00
- A diferença entre a média e mediana mostra que a maioria dos clientes está gastando menos de R$ 25,87. Isso pode indicar um público sensível ao preço e tambem considerando o uso massivo de cupons.
    - **Sugestão: Reforce estratégias de upsell "Incentivar o cliente a comprar serviços mais caros do que ele escolheu de inicio" como pacotes, jogos  e skins combinados em passes e promova testes de planos premium por x dias com preços acessíveis ou com bônus temporários.**
---
- **Clientes de maior valor estão em risco de deixar o serviço**
    - 21 clientes fizeram compras de R$ 62,00
    - 13 não renovaram o plano
- 62% dos clientes com maior valor de compra não renovaram o plano. Podendo indicar insatisfação com o serviço ofertado.
    - **Sugestão: Criar campanhas de retenção específicas para esse público, como bônus exclusivos ou cupons personalizados. Também é importante investigar o motivo de não renovação deste grupo.**
---
- **Cupons têm alto impacto no comportamento de compra**
    - Total de cupons usados: R$ 2.122,00
    - 244 cupons utilizados (quase um por assinante)
    - Mais populares: R$15 (46x), R$10 (44x)
- O público responde bem a incentivos financeiros.
    - **Sugestão: Testar cupons em datas estratégicas, como lançamentos de novidades dos passes ou da empresa, ou ligados a renovação automática. Também vale segmentar por perfil de gasto (usuários de baixo valor vs. alto valor), podendo trazer bônus para cupons usados por usuarios de alto valor.**
---
- **Alto Interesse nos Passes — Potencial para venda cruzada**
    - Minecraft Pass: R$ 3.880,00 com 194 assinantes (66% dos clientes totais)
    - EA Play Pass: R$ 2.940,00 com 98 assinantes (33% dos clientes totais)
-  O Minecraft Pass tem uma adesão muito maior, provavelmente por ser liberado com dois tipos de plano (Standard e Ultimate), enquanto o EA Play está limitado ao plano Ultimate.
    - **Sugestão: Tornar o EA Play acessível para o plano Standard (com funcionalidades limitadas e preços menores) isto pode aumentar a adesão. Tambem Oferecer combos de passes com desconto para incentivar múltiplas assinaturas por cliente.**
---
- **Gráfico de barras verticais / Total Value of Subscription Type or Plan:**
    - Este gráfico de barras verticais apresenta a **distribuição da receita total obtida a partir dos diferentes tipos de inscrição e dos planos oferecidos**. O objetivo é identificar os principais geradores de receita, entender o comportamento dos clientes e sugerir ações estratégicas.
    1. Monthly (R$ 3.571,00) = (46,78%): Valor total das assinaturas mensais.
    2. Quarterly (R$ 2.308,00) = (30,24%): Valor total das assinaturas trimestrais.
    3. Annual (R$ 1.754,00) = (22,98%): Valor total das assinaturas anuais.
        - As assinaturas mensais são responsáveis por quase metade da receita. Enquanto os planos anuais representam menos de 25% da receita. Isso pode indicar resistência a compromissos mais longos ou falta de incentivo atrativo. O modelo trimestral tem uma presença intermediária, o que pode ser explorado como uma alternativa mais estável em relação ao mensal.
    - Valor total gerado pelos 3 tipos de planos:
    1. Ultimate (R$ 5.388,00)= (70,59%): 
    2. Standard (R$ 1.801,00) = (23,59%): 
    3. Core (R$ 444,00) = (5,82%): 
        - O plano Ultimate é responsável por mais de 70% da receita. Isso mostra que há uma alta procura por parte dos clientes. O plano Standard aparece com quase um quarto da receita. O plano Core tem participação muito baixa, o que levanta a questão sobre sua efetividade.
- Insights:
    - Promoções e incentivos para planos anuais: Criar campanhas com descontos progressivos ou benefícios extras pode aumentar a adesão aos planos de longo prazo, melhorando a previsibilidade de receita.
    - Campanhas específicas para o plano Standard: Considerando sua base razoável de receita, o plano Standard pode ser um ponto de crescimento se bem trabalhado com upgrades e diferenciação de valor.
    - Revisão do plano Core: Avaliar se ele deve ser mantido como está, reposicionado como um plano de entrada gratuito ou mesmo descontinuado.
    - Foco no plano Ultimate: Como principal fonte de receita, o plano Ultimate deve receber atenção especial para retenção.


4. Total Monthly Automatic Renewals:

Este gráfico de linhas mostra a tendência do número total de renovações automáticas de assinaturas ao longo dos meses (janeiro a dezembro).
Os números acima de cada ponto da linha indicam o valor exato de renovações automáticas para cada mês.
É possível observar variações no número de renovações automáticas ao longo do ano.
5. Automatic Subscription Renewal Fee:

Este gráfico de semicírculo (gauge chart) indica a porcentagem da taxa de renovação automática de assinaturas, que está em 50,17%.
Ele compara a taxa atual com o intervalo de 0% a 100%.
6. Total Cumulative Subscription and Pass Prices by Plan:

Este gráfico de barras horizontais comparativas mostra o preço total acumulado de diferentes planos de assinatura e passes (Minecraft e EA Play), discriminados por tipo de plano (Ultimate, Standard, Core).
Cada barra é dividida em segmentos coloridos representando:
Soma de Subscription Price: Valor total dos preços das assinaturas do plano.
Soma de Minecraft Season Pa...: Valor total relacionado ao "Minecraft Season Pass" para aquele plano.
Soma de EA Play Seaso...: Valor total relacionado ao "EA Play Season" para aquele plano.
Soma de Coupon Value: Valor total de cupons utilizados para aquele plano.
Os valores ao lado de cada barra indicam o valor total acumulado para cada plano. Este visual permite comparar o valor total de diferentes ofertas e a contribuição de cada componente (assinatura, passes, cupons).
7. Total Cumulative Value per month:

Este gráfico de linhas e barras combinadas exibe a evolução do valor total acumulado ao longo dos meses (janeiro a dezembro).
A linha azul escura representa a "Soma de Total Value" acumulada por mês, referenciada no eixo vertical esquerdo (R$).
As barras verdes representam a "Média de Coupon Value" por mês, também referenciada no eixo vertical esquerdo (R$).
A linha verde clara representa a "Contagem de Coupon Value" por mês, referenciada no eixo vertical direito (R$ 20).
Este visual permite analisar a tendência da receita total, o valor médio dos cupons utilizados e a quantidade de cupons utilizados ao longo do tempo. 






4.Análise e Insights Gerais:


Após explicar cada visual, faça uma análise geral dos principais insights que o dashboard proporciona.
Quais são as tendências mais importantes?
Há algum ponto que merece atenção (ex: baixa adesão a um tipo de assinatura, alto número de clientes sem renovação automática)?
Como essas informações podem ser usadas para tomar decisões de negócios? (ex: campanhas de marketing focadas nos tipos de assinatura mais populares, incentivar a renovação automática, analisar a efetividade dos cupons).

- O valor total médio de R$ 25,87 indica que, em média, cada cliente está contribuindo com esse montante por transação. Embora esse número represente uma boa base de faturamento, ele também revela uma oportunidade clara de crescimento: ao aumentar ligeiramente o ticket médio – por exemplo, com upsell de produtos complementares, combos promocionais ou programas de fidelidade – é possível ampliar significativamente a receita total sem necessariamente aumentar o número de clientes.
Exemplo: Um aumento de apenas R$ 5,00 no ticket médio elevaria o valor para R$ 30,87. Em 1.000 vendas mensais, isso significaria um incremento de R$ 5.000,00 na receita mensal.


5.Conclusão:
