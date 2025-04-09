# Previsão de Variação de Ações com Redes Neurais LSTM

O mercado financeiro é altamente volátil, com oscilações de preços que ocorrem de forma imprevisível devido a fatores como notícias econômicas, clima, política e comportamento coletivo dos investidores. Antecipar essas variações é um desafio complexo, mas essencial para analistas e investidores que desejam tomar decisões mais assertivas.

Este projeto tem como objetivo desenvolver um modelo de previsão de preços de ações utilizando uma **Rede Neural Recorrente do tipo LSTM (Long Short-Term Memory)**, uma técnica de Deep Learning especialmente eficaz na modelagem de séries temporais com padrões complexos, ruídos e comportamento não linear.

---

## Objetivo

Construir um pipeline completo de previsão de séries temporais financeiras com:

- Limpeza e tratamento de dados históricos
- Visualização e exploração dos padrões de variação
- Criação de variáveis derivadas como média móvel
- Normalização e estruturação dos dados para redes neurais
- Treinamento e validação de uma rede LSTM
- Avaliação com métricas de erro (MSE, RMSE, MAE)
- Discussão dos resultados e limitações

---

## Por que LSTM?

As **Redes Neurais Recorrentes (RNNs)** são modelos projetados para lidar com dados sequenciais, onde a ordem importa — como no caso de séries temporais. No entanto, RNNs tradicionais enfrentam dificuldades em reter informações por longos períodos devido ao problema do **desvanecimento ou explosão do gradiente**.

A **LSTM** foi criada para resolver esse problema. Ela possui uma arquitetura interna com **"portas de memória"** que controlam o fluxo de informação:

- **Porta de entrada**: decide quais informações entram na memória
- **Porta de esquecimento**: determina o que deve ser descartado
- **Porta de saída**: filtra o que será passado adiante para as próximas etapas

Isso permite que o modelo **"lembre" de eventos importantes mesmo após muitas etapas**, sendo ideal para séries com dependências temporais de longo prazo, como o comportamento dos preços de ações.

Além disso, a LSTM **não exige que os dados sejam estacionários**, e se adapta bem a **oscilações bruscas e ruídos**, sendo mais robusta que técnicas tradicionais como médias móveis ou regressões simples.

---

## Aplicação

Este projeto foi desenvolvido como parte da disciplina de Redes Neurais, com foco na aplicação prática de IA no contexto financeiro. No final, o modelo poderá ser adaptado para outras séries temporais, como previsão de vendas, demanda energética ou métricas de marketing digital.

A estrutura do notebook segue uma pipeline lógica e didática, facilitando o entendimento do processo completo — desde o tratamento dos dados até a análise final dos resultados preditivos.
