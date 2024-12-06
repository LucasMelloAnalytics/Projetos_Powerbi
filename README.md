# Dashboard de Análise de Resultados

Este projeto apresenta um dashboard interativo desenvolvido no Power BI, utilizando uma base de dados fictícia em formato CSV. O objetivo é analisar resultados de negócios, identificando tendências, métricas de desempenho e insights estratégicos para a tomada de decisões mais assertivas.

---

## 🗂️ Etapas do Desenvolvimento

### 1. **Coleta e Tratamento de Dados**
Os dados foram importados de arquivos CSV e tratados no Power Query. As ações realizadas incluem:
- Exclusão de linhas em branco.
- Remoção de duplicatas em colunas que não deveriam conter duplicidades.
- Substituição de erros por valores nulos.
- Correção de tipos de dados para garantir integridade.
- Ajuste do formato de datas para o padrão local (dd/mm/yyyy).
- Substituição de valores nas colunas de sexo: `M` para **Masculino** e `F` para **Feminino**.
- Combinação das colunas **Nome** e **Sobrenome** em uma única coluna.

### 2. **Modelagem de Dados**
- Utilizou-se o formato **Snowflake** para a modelagem dos dados.
- Criou-se uma **Dimensão Tempo** para facilitar análises temporais.

### 3. **Definição de KPIs e Visualizações**
Após analisar os requisitos do projeto:
- Identifiquei os principais **KPIs** relevantes para a análise.
- Planejei os visuais mais adequados para representar os indicadores de forma clara e informativa.

### 4. **Criação de Medidas**
Diversas medidas foram criadas para atender aos requisitos de análise, divididas em:
- **Medidas de Performance:** Indicadores para avaliar desempenho.
- **Medidas de Inteligência de Tempo:** Análise de tendências e variações ao longo do tempo.
- **Medidas de Agregação:** Sumarização de dados em níveis desejados.
- **Medidas Aritméticas:** Cálculos diretos, como médias e proporções.

### 5. **Design e Layout**
- Desenvolvi um **template visual** para garantir organização e estética nas visualizações.
- Os visuais foram organizados de maneira a facilitar a interpretação e navegação.

---

## 📊 Indicadores Principais

### Indicadores de Desempenho
- **Receita Bruta:** Total de receita antes de descontos e deduções.
- **Receita Líquida:** Receita após deduções e descontos.
- **Descontos:** Soma total de descontos aplicados.
- **Preço de Custo:** Valor associado ao custo de produção ou aquisição.
- **Margem:** Diferença percentual entre receita líquida e custo.
- **Ticket Médio:** Valor médio por venda.

### Indicadores de Inteligência de Tempo
- **Share:** Participação percentual em relação a períodos ou categorias específicas.
- **Variação:** Diferença percentual entre períodos comparados.
- **YoY (Year-over-Year):** Comparação de desempenho com o mesmo período do ano anterior.
- **LY (Last Year):** Valor correspondente ao mesmo período do ano anterior.

---

## 🛠️ Ferramentas Utilizadas
- **Power BI:** Modelagem e visualização dos dados.
- **Power Query:** Para o tratamento inicial dos dados.

---

## 🔍 Principais Funções DAX Utilizadas

### Funções de Cálculo e Agregação
- **`SUM`**: Soma os valores de uma coluna.
- **`SUMX`**: Soma os valores de uma expressão avaliada em cada linha de uma tabela.
- **`DIVIDE`**: Realiza divisões, tratando divisões por zero de forma segura.

### Funções de Contexto e Filtragem
- **`CALCULATE`**: Modifica o contexto de cálculo de uma medida.
- **`ALL`**: Remove filtros de colunas ou tabelas especificadas.
- **`ALLSELECTED`**: Remove filtros externos, preservando aqueles aplicados dentro de um visual.

### Funções de Inteligência de Tempo
- **`SAMEPERIODLASTYEAR`**: Retorna o mesmo período no ano anterior.

### Funções Condicionais e Lógicas
- **`SWITCH`**: Avalia uma expressão e retorna diferentes resultados com base em condições especificadas.
- **`IF`**: Retorna diferentes valores dependendo de uma condição.
- **`ISINSCOPE`**: Verifica se uma coluna está no escopo de uma agregação atual.

### Método de Medida Dinâmica
Utilizei o **`SWITCH`** em conjunto com uma **variável** para criar uma medida dinâmica que ajusta os KPIs com base nos filtros selecionados pelo usuário.

---

## 📥 Como Executar
1. Faça o download do arquivo `.pbix` presente neste repositório.
2. Abra o arquivo no Power BI Desktop.
3. Explore o dashboard interativo e os visuais.
4. Ou acesso o esse link - > [Dash_AnaliseDeResultados]([url](https://app.powerbi.com/view?r=eyJrIjoiODM4YTZlYzktM2Y1MC00OTZhLWFjYmUtZDcyZWQ4YTBjYzMxIiwidCI6IjFlZTQ1Y2QyLTUzMTMtNDBjOS1hYTJlLTJhZDg2MDkwMmQ3MCJ9))

---

## 🖼️ Demonstração


---

## 📧 Contato
Se tiver dúvidas ou quiser saber mais sobre este projeto, entre em contato comigo em:
- **Email:** lucas.moreira.mello@outlook.com
- **LinkedIn:** [https://www.linkedin.com/in/lucas-moreira-de-mello/)
