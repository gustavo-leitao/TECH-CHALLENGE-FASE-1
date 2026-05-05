# Análise de NPS e Recompra

## Objetivo do Projeto

Este projeto tem como objetivo analisar os principais fatores operacionais que impactam a satisfação do cliente (NPS/CSAT) e sua relação com a recompra.

A análise busca responder:

* Quais fatores operacionais mais influenciam o NPS?
* Como antecipar problemas antes da coleta de satisfação?
* Como a experiência do cliente impacta a recompra?

---

## Descrição da Base de Dados

A base contém informações operacionais e de experiência do cliente:

* csat_interno: indicador de satisfação operacional
* nps_score: nota dada pelo cliente
* recompra_30d: indicador de recompra em até 30 dias
* tempo_resolucao: tempo para resolução
* qtd_reclamacoes: volume de reclamações
* status_pedido: status do pedido
* regiao_cliente: localização
* idade_cliente: idade

---

## Metodologia

1. Limpeza e preparação dos dados

* Tratamento de valores nulos
* Padronização de colunas
* Criação de variáveis derivadas

2. Análise exploratória

* Distribuição do NPS
* Análise por segmentos
* Relação entre variáveis operacionais

3. Criação de faixas

* CSAT: baixo, médio, alto
* Tempo de resolução: agrupamentos

4. Análise de impacto

* CSAT vs recompra
* Tempo de resolução
* Reclamações

5. Visualizações

* Boxplots
* Scatter plots
* Médias por grupo

---

## Principais Insights

* CSAT alto aumenta a recompra
* Tempo de resolução alto reduz recompra
* Muitas reclamações reduzem drasticamente a recompra
* Existe uma cadeia: Operação → CSAT → NPS → Recompra

---

## Como Executar o Projeto

### 1. Clonar o repositório

```bash
git clone <url-do-repositorio>
cd <nome-do-repositorio>
```

### 2. Criar ambiente virtual

```bash
python -m venv venv
source venv/bin/activate
venv\Scripts\activate
```

### 3. Instalar dependências

```bash
pip install -r requirements.txt
```

### 4. Executar

```bash
jupyter notebook
```

Abrir:

```
notebooks/EDA_nps.ipynb
```

---

## Como Reproduzir os Resultados

1. Utilizar dados da pasta data/raw
2. Executar o notebook completo
3. Garantir versões compatíveis das bibliotecas

---

## Boas Práticas Aplicadas

* Código organizado
* Variáveis padronizadas
* Comentários explicativos
* Estrutura de pastas clara
* Separação de dados
* Reprodutibilidade

---

## Próximos Passos

* Modelo preditivo de NPS
* Identificação de drivers
* Alertas operacionais
* Automação da análise
