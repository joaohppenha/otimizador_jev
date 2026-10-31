# Dynamic Support Lane Optimizer (Jev AI)

Um motor lógico de triagem assíncrona para suporte de alta demanda (padrão Big Tech / Delivery) utilizando as primitivas de decisão estruturada do Jev (TypeSafe AI). 

Este projeto demonstra como substituir arquiteturas baseadas em LLMs tradicionais (System Two) por um cérebro lógico de alta velocidade (System One), gerando respostas determinísticas diretamente na borda da API com foco em eficiência de custo e latência.

---

## Filosofia de Design: IA Invisível

O sistema atua em segundo plano nas esteiras de atendimento para otimizar a experiência do usuário sem criar atritos visuais:
* **Zero Atrito:** Relatos cotidianos de baixa complexidade recebem soluções expressas de forma instantânea via API.
* **Acolhimento Inteligente:** Casos complexos ou com métricas atípicas de governança são encaminhados silenciosamente para esteiras de especialistas humanos, sem a exibição de alertas invasivos ou mensagens de erro.

---

## Passo a Passo do Projeto

O desenvolvimento do projeto foi dividido de forma modular em três etapas principais dentro do notebook:

### 1. Modelagem do Motor Jev (Score e Choice)
Configuração da inteligência analítica do sistema utilizando o modelo de decisão estruturada:
* **Mapeamento de Contexto (Score):** Avaliação não estruturada do corpo do relato, histórico do usuário e volumetria financeira, convertendo os dados em um índice linear de complexidade de 1 a 10.
* **Roteamento Determinístico (Choice):** Seleção imediata da esteira de destino ideal com base na complexidade calculada.

### 2. Estruturação do Dataset de Cenários
Criação de uma base de simulação contendo relatos comuns do cotidiano de um suporte de delivery (como itens faltantes, problemas com embalagens e usuários com alto índice de chamados recentes), isolando as variáveis para auditoria do motor lógico.

### 3. Dashboard e Análise de Infraestrutura
Processamento das requisições simulando a latência em milissegundos nativa do Jev, consolidando as ações e métricas em um dataframe estruturado para tomada de decisão gerencial.

---

## Estudo de Viabilidade Técnica e Financeira

Abaixo está o gráfico comparativo demonstrando o impacto de desempenho e eficiência de custos entre a arquitetura utilizando o Jev contra uma LLM Generativa Comercial tradicional (como o GPT-4o) para cada 1 milhão de requisições:

![Comparativo de Eficiência Jev vs GPT-4o](./otimizador_jev/IMG/img.png)



### Diagnóstico da Infraestrutura:
* **Velocidade:** O Jev entrega respostas cerca de 160 vezes mais rápidas que uma LLM convencional, reduzindo o tempo de espera no chat para a casa dos milissegundos.
* **Sustentabilidade Financeira:** Redução drástica do custo por chamada, viabilizando o processamento em tempo real de milhões de transações diárias.

---

## Como Executar

1. Abra o arquivo do notebook no Google Colab.
2. Execute as células em sequência para inicializar o motor, carregar o conjunto de cenários e visualizar o dashboard de operações com os gráficos de indicadores de desempenho.
