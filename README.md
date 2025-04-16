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
- **Gráficos** 
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

- **Gráfico de linhas / Total Monthly Automatic Renewals:**
    - Este gráfico de linhas mostra a **tendência do número total de renovações automáticas de assinaturas ao longo dos meses (janeiro a dezembro)**. O objetivo é visualizar o padrão das renovações e identificar períodos de maior ou menor recorrência de assinaturas.
    - Nos meses (Março até Novembro) os valores 30 e 31 se repetiram
    - É possível observar baixas significativas entre os meses (janeiro,Fevereiro) Já que só teve 4 assinantes neste periodo.
    - O mês de Dezembro a razão é uma queda da metade das assinaturas.
    - meses de baixa renovação podem ser analisados como falta de comunicação, perda de interesse ou ausência de novidades no serviço.
- Insights:
    - Campanhas de retenção direcionadas: Para meses com tendência de queda, é possível planejar ações de retenção, como envio de e-mails de lembrete, ofertas exclusivas ou melhorias no conteúdo antes da data de renovação.

- **Gráfico de semicírculo / Automatic Subscription Renewal Fee:**
    - Este gráfico em formato de gauge mostra a **taxa atual de renovação automática das assinaturas**, atualmente em 50,17%. Essa taxa indica que aproximadamente metade dos usuários opta por manter a renovação automática ativa.
    - Um valor abaixo de 60% pode ser um sinal de que os clientes ainda têm inseguranças ou não percebem vantagens claras em manter a renovação automática.
- Insights:
    - Melhorar comunicação de valor: Investir em destacar os benefícios da renovação contínua, como acesso ininterrupto, descontos ou recompensas.
    - Incentivos para ativação da renovação automática: Implementar benefícios exclusivos para quem ativa a renovação automática pode elevar essa taxa.Exemplo: 1 mês gratuito após 6 renovações consecutivas.
    - Segmentação de campanhas: Analisar o perfil de usuários que não ativam a renovação pode ajudar a criar campanhas específicas para esse público, com mensagens mais personalizadas.

- **Gráfico de barras horizontais comparativas / Total Cumulative Subscription and Pass Prices by Plan:**
    - Este gráfico mostra a **comparação do valor total acumulado por plano, incluindo preço das assinaturas, passes de jogos (Minecraft e EA Play) e cupons usados**.
    1. Subscription Price: Valor total das assinaturas. Linha azul
        - Com um total de R$2.935,00 nos 3 planos, tendo 38,45% do valor total do ano.
    2. Minecraft Season Pass: Valor total acumulado de passes do Minecraft. Linha verde
        - Se destaca nos planos que o contem.
    3. EA Play Season Pass: Valor total acumulado de passes do EA Play.Linha vermelha
        - Tem o maior ganho individual
    4. Coupon Value: Valor total de cupons aplicados no plano.Linha roxa
        - Teve o valor mais alto no Standard
- Insights:
    - Entender a composição de valor por plano: Saber qual parte da receita vem dos passes (Minecraft / EA Play) ou dos cupons utilizados ajuda a ajustar os planos para melhorar a percepção de valor. Se os passes agregam muito valor, podem ser promovidos como diferenciais.
    - Reposicionar planos com menor valor acumulado: Planos como o Core, se apresentarem pouco retorno, podem ser ajustados em termos de preço, benefícios ou foco (ex: torná-lo um plano de entrada gratuito com upsell posterior).

- **Gráfico combinado (linhas e barras) / Total Cumulative Value per Month:**
    - Este gráfico exibe a **relação entre o valor gerado e o uso de cupons**.combinando três informações:
    1. Barras verdes: Soma do valor total acumulado.
        - Se manteve constante do mês de março até novembro, o pico mais alto foi outubro com R$832,00, mais baixo foi junho com R$ 770,00 uma diferença de 62 reais (7,46%). 
    2. Linha azul escura: Média de valores de cupons aplicados por mês.
        - De março até novembro a maior média foi no mês de junho com R$ 9,20, a menor foi em março com R$ 7,86,00.
    3. Linha verde clara: Contagem de cupons utilizados por mês.
    - De março até novembro a contagem se repete, 25 e 26 cupons. Neste mesmos meses o a média de rendimento do Minecraft foi de R$ 400,00 e da Ea Play de R$ 300,00.
- Insights:
    - Há um ponto de equilíbrio entre o valor do cupom e a propensão de compra. Cupons muito altos podem não gerar retorno proporcional. É importante testar limites de desconto e analisar elasticidade de preço para cada perfil de cliente.
    - Considerando o alto peso dos passes, campanhas promocionais com foco específico em passes (e não nos planos) podem ser mais eficientes. Por exemplo: Combo promocional: “Assine o Ultimate + Passe EA Play com 20% OFF”

4. **Insights Extras**:

    - Aumentar o Valor Médio por Cliente: O valor médio de cada cliente  por transação é de R$ 25,87. O objetivo é conseguir aumentar esse valor em para R$ 30,00 ,(15,95%) — por exemplo, com ofertas de produtos extras, combos ou um programa de fidelidade.
        - Exemplo: Se cada pessoa gastar R$ 5,00 a mais, o valor médio vai pra R$ 30,87. Se forem feitas 1.000 vendas no mês, isso representa R$ 5.000,00 a mais de receita no mês.

    - Campanhas de Lançamento e Atração Inicial: Campanha de pré-lançamento com vantagens especiais. 
        - Exemplo: destravar 1 mês grátis ou liberar conteúdos antes do lançamento pode ajudar a chamar atenção.

    - Atrair com as Redes Sociais: Usar anúncios pagos (Google Ads, redes sociais). Importante direcionar os anúncios para o público que mais combina com o serviço. Parcerias com influenciadores do nicho, pessoas que o público já segue e confia podem ajudar muito a divulgar.

    - Criar um plano especial para os primeiros inscritos. Pode oferecer benefícios únicos, como acesso vitalício a algumas funções ou bônus exclusivos.

    - Promoções Inteligentes e Testes de Upgrade: Promoções com upgrade automático por um tempo limitado para o cliente vizualizar os bônus do plano superior ao seu.
        - Exemplo: quem assinar o plano básico (Standard) ganha acesso ao plano mais completo (Ultimate) por 30 dias.

    - Mostrar conteúdos relevantes logo no início: Disponibilizar videos em redes sociais ou no site do serviço com o intuito de ensinar o cliente a usar os serviços e mostrar vantagens. Personalizar essa experiência ajuda o cliente a ver valor rapidamente.

    - Incentivar a Renovação Automática: Dar desconto progressivo pra quem ativa a renovação automática.
        - Exemplo: 10% de desconto na segunda fatura, 15% na terceira.


    - Distribuição de cupons de desconto: Compartilhar cupons de boas-vindas com prazo curto, ofertas que o cliente ganha um cupom de desconto por cada amigo que indicar.

    - Análise de Dados e Feedback dos Clientes: Recorrer a pesquisas rápidas nos primeiros 7 a 14 dias. Isso ajuda a entender o que está funcionando e o que pode melhorar.

    - Criar um canal direto com os usuarios do serviço.
        - Exemplo: Um grupo no Discord ou um fórum fechado para ouvir opiniões e sugestões.

    - Gamificação para Engajamento e Retenção: Criar um sistema de pontos ou recompensas por fidelidade para engajar os clientes e não criar o sentimento de esquecimento do cliente por parte da XBOX.
        - Exemplo: o cliente ganha conquistas por continuar renovando o plano ou por fazer upgrades.


5. **Conclusão**:
    - Analisando os dados do dashboard, fica claro que o serviço da XBOX tem um bom potencial de crescimento, mas ainda existem pontos importantes que precisam de atenção para melhorar os resultados. O gasto médio por cliente é baixo (R$ 25,87), o que mostra que os usuários são sensíveis ao preço e usam bastante cupons. Indicando que precisa criar estratégias de upsell e fidelização, mostrando mais valor nos planos mais completos como o Ultimate, que hoje já representa mais de 70% da receita. Por outro lado, vemos que clientes com maior valor de compra estão deixando o serviço (62% deles não renovaram), o que liga um alerta. Talvez essas pessoas estejam esperando mais benefícios, ou sentindo falta de novidades. A criação de campanhas específicas e benefícios exclusivos pode ajudar a reter esse público. A adesão aos passes de jogos também chama atenção, principalmente o de Minecraft, com 66% de uso entre os clientes. Isso mostra que há um alto interesse em conteúdo extra, o que abre oportunidades para criar combos, pacotes promocionais ou testes gratuitos, incentivando a assinatura de múltiplos serviços. A renovação automática ainda está em 50,17%, o que é baixo. Melhorar a comunicação sobre seus benefícios e oferecer vantagens exclusivas para quem ativa a renovação pode ser um bom caminho. Por fim, os dados mostram que os cupons influenciam muito nas decisões de compra, então vale usar isso a favor em campanhas estratégicas e bem planejadas.

**Ferramentas e Tecnologias Utilizadas:**
- Power BI (DAX, Power Query)
- Excel (Modelagem de dados)
- Figma (Design)
- GitHub (versionamento)
