# 🔍 Análise de Evasão de Clientes (Churn)

## 📌 Introdução

O objetivo deste projeto é analisar dados de clientes de uma empresa de telecomunicações para entender o comportamento de evasão (churn). O churn representa os clientes que encerraram seus contratos, e entender os fatores que levam a isso é essencial para desenvolver estratégias de retenção e fidelização.

---

## 🧹 Limpeza e Tratamento de Dados

Durante esta etapa, foram realizadas as seguintes ações:

- **Importação dos dados brutos** de um arquivo `.csv`.
- **Transformação de colunas aninhadas (JSON)** em colunas regulares.
- **Conversão de variáveis categóricas** para formatos numéricos (por exemplo, "Sim"/"Não" para 1/0), o que facilita a análise.
- **Remoção de valores ausentes e duplicados**, garantindo a integridade dos dados.
- **Criação da coluna `Contas_Diarias`**, que representa o valor médio pago por dia, derivado do faturamento mensal dividido por 30 dias.
- **Renomeação de colunas** para termos mais compreensíveis, facilitando a leitura e interpretação dos resultados.

---

## 📊 Análise Exploratória de Dados (EDA)

A análise exploratória permite observar o comportamento dos dados e identificar padrões associados à evasão de clientes.

### 🎯 Distribuição Geral do Cancelamento

Visualizamos a proporção de clientes que cancelaram vs. os que permaneceram utilizando gráficos de barras e de pizza. Isso ajuda a entender a gravidade do churn no negócio.

### 👥 Cancelamento por Variáveis Categóricas

Foram analisadas variáveis como:

- Gênero (`gender`)
- Tipo de contrato (`contract`)
- Método de pagamento (`paymentmethod`)
- Serviços adicionais como suporte técnico e segurança online
- Presença de dependente ou parceiro

Com essas comparações, foi possível observar **quais grupos de clientes estão mais propensos a cancelar**.

### 📈 Cancelamento por Variáveis Numéricas

Variáveis como:

- `Faturamento_Total`
- `Faturamento_Mensal`
- `tenure` (tempo de contrato)
- `Contas_Diarias`

foram analisadas por meio de **boxplots** e **histogramas** para verificar diferenças estatísticas no comportamento entre clientes que cancelaram e os que não cancelaram.

---

## 🧠 Conclusões e Insights

A partir da análise, os principais achados foram:

- **Clientes com contratos mensais** têm muito mais chance de cancelamento do que os com contratos anuais.
- **Clientes sem suporte técnico ou segurança online** apresentaram taxas mais altas de evasão.
- A maioria dos cancelamentos ocorre **nos primeiros meses do contrato**, indicando a importância da retenção inicial.
- **Clientes com menor faturamento total** e **valores diários mais altos** mostraram maior propensão ao churn.

---

## 💡 Recomendações

Com base nas descobertas, recomenda-se:

1. **Oferecer benefícios ou descontos em contratos mais longos** (anual ou bianual).
2. **Incluir serviços adicionais como suporte técnico gratuito** nos primeiros meses.
3. **Focar em ações de retenção nos 3 primeiros meses de contrato.**
4. **Identificar clientes com alto custo diário** e atuar preventivamente com atendimento proativo.
5. **Incentivar métodos de pagamento automáticos** para evitar cancelamentos por esquecimento ou inadimplência.

---

## ✅ Encerramento

A análise permitiu mapear os principais fatores que influenciam a evasão de clientes. Com essas informações, a empresa pode desenvolver estratégias mais eficazes de retenção, melhorando a experiência do cliente e reduzindo perdas financeiras.
