# Dashboard Completo do iFood — Análise de Campanhas de Marketing e Comportamento do Cliente

Com mais de 2.200 registros de clientes e 29 variáveis, dados brutos raramente contam histórias sozinhos. Neste projeto, desenvolvi um dashboard completo de análise de marketing utilizando dados reais do iFood disponíveis no Kaggle, com o objetivo de transformar esse volume de informação em insights claros sobre padrões de consumo, segmentação de clientes e performance de campanhas — tudo em um dashboard interativo e visualmente atrativo.

---

## O Desafio

O ponto de partida eram perguntas estratégicas que qualquer time de marketing gostaria de responder:

- Qual faixa salarial gasta mais?
- Clientes com filhos gastam menos?
- Quem gasta mais por nível de educação e estado civil?
- Quais campanhas de marketing tiveram melhor performance?
- Quantos clientes aceitaram pelo menos 1 campanha?
- Como se distribuem os gastos por produto e por canal de compra?

Responder essas perguntas com clareza exigiu não apenas visualização, mas uma estrutura de dados bem pensada desde o início.

---

## Estrutura do Dashboard

O dashboard foi dividido em 3 páginas principais, cada uma com um foco analítico distinto:

**Página 1 — Visão Geral**
- KPIs principais: Receita Total, Salário Médio Anual e Total de Clientes
- Distribuição de vendas por canal — Web, Catálogo e Loja
- Mix de produtos vendidos

**Página 2 — Análise de Clientes**
- Segmentação por faixa salarial
- Perfil de gastos por nível educacional
- Impacto de ter filhos nos gastos
- Análise por estado civil

**Página 3 — Performance de Campanhas**
- Taxa de aceitação por campanha
- Total de clientes que aceitaram pelo menos 1 campanha

---

## Principais Insights

**O Sweet Spot Salarial**

Clientes na faixa de 70k–90k são os campeões de gastos, superando qualquer outra faixa salarial. Surpreendentemente, quem ganha acima de 90k gasta menos — possivelmente por ser um grupo menor ou por ter acesso a outras opções de consumo. Esse dado é valioso para priorizar segmentos nas próximas campanhas.

**Filhos Impactam o Comportamento**

Clientes sem filhos gastam significativamente mais, provavelmente por terem maior renda disponível. Isso sugere uma oportunidade clara para campanhas segmentadas focadas em conveniência para famílias — um público com alta frequência de compra, mas ticket médio menor.

**Campanhas 4 e 3 Lideram**

As campanhas 4 e 3 tiveram as melhores taxas de aceitação (7,4% cada), enquanto a campanha 2 registrou o pior desempenho (1,4%). Essa diferença expressiva indica necessidade de revisão profunda na estratégia das campanhas com menor engajamento.

**Engajamento é Minoritário**

Apenas uma parcela dos clientes aceitou pelo menos uma campanha, sugerindo grande potencial de melhoria nas estratégias de marketing e personalização. O dado levanta uma pergunta importante:

> Como aumentar a taxa de conversão sem aumentar o volume de campanhas?

---

## Desafios Técnicos e Soluções

**Unpivot para Flexibilidade**

Um dos maiores desafios foi trabalhar com múltiplas colunas de categorias de produtos — Vinhos, Frutas, Carnes, entre outros. A solução foi aplicar unpivot no Power Query, transformando 6 colunas em 2:

- `Categoria_Produto`
- `Valor_Gasto`

Essa transformação permitiu criar visualizações dinâmicas com um simples arrastar de campos, sem necessidade de medidas separadas para cada categoria.

**Criação de Segmentos Inteligentes**

Utilizei DAX para criar segmentações personalizadas — faixas salariais, perfis de família e grupos de engajamento — que não existiam diretamente nos dados brutos, mas eram essenciais para as análises de comportamento.

**Múltiplas Tabelas para Diferentes Análises**

Criei tabelas separadas — original e com unpivot — para manter flexibilidade nas análises sem comprometer a estrutura dos dados. Cada tabela serve um propósito analítico específico dentro do modelo.

---

## Aprendizados

Este projeto reforçou a importância de alguns princípios que vão além das ferramentas:

**Entender o negócio antes da técnica** — Saber quais perguntas responder é mais importante do que dominar ferramentas. O dashboard só faz sentido se as perguntas certas foram feitas antes de abrir o Power BI.

**Estrutura de dados flexível** — Unpivot e normalização não são apenas boas práticas técnicas — elas facilitam análises futuras e tornam o modelo mais sustentável a longo prazo.

**Visualização focada no usuário** — Dashboards devem contar histórias, não apenas mostrar números. Cada visual precisa ter um propósito claro para quem vai consumir a informação.

**Iteração constante** — O dashboard evoluiu muito desde a primeira versão. A melhoria contínua é parte do processo, não uma exceção.

---

## Conclusão

Este projeto reforça como a análise de dados de marketing vai muito além de gráficos bonitos — ela revela comportamentos, identifica oportunidades e orienta onde investir energia e orçamento.

Quando bem estruturada, a análise de campanhas permite não apenas medir o passado, mas desenhar estratégias mais inteligentes para o futuro.

---

Desenvolvido por **Felipe** — [LinkedIn](#) · [GitHub](#)

<img width="1311" height="738" alt="Captura de tela 2026-04-18 153052" src="https://github.com/user-attachments/assets/6a571f9f-dce2-41a6-a65f-35c45231f4f1" />
<img width="1314" height="735" alt="Captura de tela 2026-04-18 153105" src="https://github.com/user-attachments/assets/c571d735-0ce5-475a-9435-9331246e3add" />
<img width="1312" height="730" alt="Captura de tela 2026-04-18 153115" src="https://github.com/user-attachments/assets/f40ea1b1-ff5e-4c55-9f06-15aa7c9b7e4e" />


