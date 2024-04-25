---
title: "Modelagem e avaliação de escolas brasileiras utilizando dados abertos educacionais"
collection: publications
permalink: /publication/modelagem_escolas_jepex
excerpt: ''
date: 2016-10
venue: 'XVI JEPEX (2016)'
paperurl: ''
citation: 'SANTOS, P., FERREIRA, R. (2016). &quot;Modelagem e avaliação de escolas brasileiras utilizando dados abertos educacionais.&quot; <i>JEPEX</i>, 16a edição.'
---

Dados abertos educacionais (DAE) são informações eletronicamente gravadas relativas a estatísticas, administração, infraestrutura e pedagogia de instituições de ensino, e são de acesso fácil e gratuito a todos. Nesse estudo, foi proposto uma ferramenta automática para extração de informação dentro da base de conhecimento do MEC. O principal objetivo do trabalho é determinar quais características estruturais e não-estruturais das escolas da cidade do Recife são determinantes para justificar a nota média do ENEM obtida por cada escola participante do Exame. O ENEM foi usado como objetivo do estudo por ser a maior fonte de DAE no Brasil. A metodologia foi elaborada em algumas etapas. A partir do portal Educação Inteligente, que agrega, organiza e republica DAE vindos de diferentes fontes, obtivemos arquivo XML com dados de escolas do Recife. Esses dados foram transformados em um arquivo arff, para ser utilizado pela ferramenta de apredizagem de máquina utilizada (WEKA). O WEKA foi utilizado para selecionar atributos e classificar os dados. Quatro conjuntos de atributos denominados S1, S2, S3 e S4 foram criados com métodos automatizados de seleção, e a classificação foi realizada com estes e ainda o conjunto completo de atributos. As métricas Acurácia, Precisão, Cobertura e Medida-F foram utilizadas para determinar qual conjunto de atributos, nesse grupo de escolas, tem melhor desempenho em explicar as notas do ENEM obtidas por elas. O classificador escolhido foi o J48 gerando regras visualmente compreensíveis por pessoas. O conjunto S4, contendo 19 atributos, foi o vencedor, com Acurácia de 72,3881%, Precisão 0,689, Cobertura 0,724 e Medida-F 0,706. Ele foi gerado aplicando FilteredSubsetEval + GreedyStepwise ao conjunto completo de atributos. Concluiu-se que, para as escolas de Recife participantes do ENEM, os seguintes atributos melhor explicam a nota obtida: aguaFiltrada, aguaPublica, alimentacao, atividadeComplementar, auditorio, computadores, computadoresAdm, ejaFundamental, ejaMedio, ensinoEja, fimDeSemana, lavanderia, lixoRecicla, patioDescoberto, salaLeitura, salaProfessores, sanitarioForaPredio, formacaoDocente, socioEconomico. Essa informação obtida é primeiramente útil para gestores de escolas e administradores públicos, pois estão diretamente envolvidos com educação, mas também apresenta conhecimento aproveitável por toda a sociedade para lidar com diversas questões, sejam sociais, econômicas, educacionais, políticas ou outras.