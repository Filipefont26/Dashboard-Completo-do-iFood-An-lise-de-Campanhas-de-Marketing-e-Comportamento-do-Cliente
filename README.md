# Dashboard-Completo-do-iFood-An-lise-de-Campanhas-de-Marketing-e-Comportamento-do-Cliente

Recentemente desenvolvi um dashboard completo de análise de marketing utilizando dados reais do iFood disponíveis no Kaggle. O projeto explora padrões de consumo, segmentação de clientes e performance de campanhas tudo isso em um dashboard interativo e visualmente atrativo.

O Desafio

Com mais de 2.200 registros de clientes e 29 variáveis, o desafio era transformar dados brutos em insights claros que pudessem responder perguntas estratégicas como:

Gastos por produto
Gasto por canal de compra
Qual faixa salarial gasta mais?
Quem gasta mais por nivel de educação
Clientes com filhos gastam menos?
Quem gasta mais por estado civil
Quais campanhas de marketing tiveram melhor performance?
Clientes que aceitaram pelo menos 1 Campanha
Estrutura do Dashboard

O dashboard foi dividido em 3 páginas principais:

Página 1: Visão Geral
- KPIs principais: Receita Total, Sálario medio anual , Total de Clientes
- Distribuição de vendas por canal (Web, Catálogo, Loja)
- Mix de produtos vendidos

Página 2: Análise de Clientes
- Segmentação por faixa salarial
- Perfil de gastos por nível educacional
- Impacto de ter filhos nos gastos
- Análise por estado civil

Write on Medium
Página 3: Performance de Campanhas
- Taxa de aceitação por campanha
- Clientes que Aceitaram pelo menos 1 Camapanha

Principais Insights

O Sweet Spot Salarial
Clientes na faixa de 70k-90k são os campeões de gastos, mais do que qualquer outra faixa. Surpreendentemente, quem ganha acima de 90k gasta menos, possivelmente por serem um grupo menor ou terem outras opções de consumo.

Filhos Impactam o Comportamento
Clientes sem filhos gastam significativamente mais, provavelmente por terem maior renda disponível. Isso sugere oportunidades para campanhas segmentadas focadas em conveniência para famílias.

Campanhas 4 e 3 Lideram
As campanhas 4 e 3 tiveram as melhores taxas de aceitação (7.4% cada), enquanto a campanha 2 teve o pior desempenho (1.4%). Isso indica necessidade de revisão da estratégia de algumas campanhas.

Engajamento é Minoritário
Apenas uma parcela dos clientes aceitou pelo menos uma campanha, sugerindo grande potencial de melhoria nas estratégias de marketing e personalização.

Desafios Técnicos e Soluções

Unpivot para Flexibilidade
Um dos maiores desafios foi trabalhar com múltiplas colunas de categorias de produtos (Vinhos, Frutas, Carnes, etc.). A solução foi fazer unpivot no Power Query, transformando 6 colunas em 2:
- Categoria_Produto
- Valor_Gasto`

Isso permitiu criar visualizações dinâmicas com um simples arrastar de campos.

Criação de Segmentos Inteligentes
Utilizei DAX para criar segmentações personalizadas:

Múltiplas Tabelas para Diferentes Análises
Criei tabelas separadas (original e com unpivot) para manter flexibilidade nas análises sem comprometer a estrutura dos dados.

Aprendizados

Este projeto reforçou a importância de:

Entender o negócio antes da técnica Saber quais perguntas responder é mais importante do que dominar ferramentas
2. Estrutura de dados flexível Unpivot e normalização facilitam análises futuras
3. Visualização focada no usuário Dashboards devem contar histórias, não apenas mostrar números
4. Iteração constante O dashboard evoluiu muito desde a primeira versão

<img width="1311" height="738" alt="Captura de tela 2026-04-18 153052" src="https://github.com/user-attachments/assets/6a571f9f-dce2-41a6-a65f-35c45231f4f1" />
<img width="1314" height="735" alt="Captura de tela 2026-04-18 153105" src="https://github.com/user-attachments/assets/c571d735-0ce5-475a-9435-9331246e3add" />
<img width="1312" height="730" alt="Captura de tela 2026-04-18 153115" src="https://github.com/user-attachments/assets/f40ea1b1-ff5e-4c55-9f06-15aa7c9b7e4e" />


