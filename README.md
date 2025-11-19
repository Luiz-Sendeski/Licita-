 README.md — LICITA+ (Descrição para o GitHub)
 LICITA+ — Aplicação de LLMs na Identificação de Irregularidades em Licitações Públicas

Trabalho de Conclusão de Curso — IFPR (2025)

Este repositório reúne todo o código, dados, documentação e artefatos do projeto LICITA+, um sistema experimental desenvolvido para aplicar Grandes Modelos de Linguagem (LLMs) na análise de licitações públicas brasileiras.

O objetivo central é identificar possíveis irregularidades, como ambiguidades descritivas, duplicidade de itens e indícios de sobrepreço, utilizando modelos modernos de IA diretamente sobre textos brutos de editais — sem pré-processamento textual.

- Objetivo do Projeto

O LICITA+ foi criado para:

Analisar descrições de itens licitatórios usando LLMs

Detectar inconsistências textuais que podem indicar irregularidades

Estimar preços médios reais do varejo para comparação com valores licitados

Avaliar o desempenho de três modelos de IA:

GPT-4o-mini (OpenAI)

Claude Sonnet 4.5 (Anthropic)

DeepSeek-V2 (DeepSeek AI)

Disponibilizar todos os resultados em formato aberto, promovendo transparência e ciência reprodutível

- Tecnologias e Ferramentas Utilizadas

Python 3.10+

Google Colab (pipeline experimental)

APIs OpenAI, Anthropic e DeepSeek

Pandas, NumPy, SciPy, Matplotlib

OpenPyXL (planilhas de referência)

Git/GitHub — repositório aberto

Dataset próprio com editais das 10 maiores cidades do Paraná (2021–2024)

- Estrutura do Repositório
/
├── data/
│   ├── licitacoes_raw/          # Descrições brutas coletadas nos editais
│   ├── dataset_licita+.xlsx     # Dataset final após curadoria
│   └── valores_referencia/      # Cotações utilizadas como “ground truth”
│
├── src/
│   ├── prompts/                 # Prompts padronizados para cada modelo
│   ├── pipeline_colab.ipynb     # Pipeline completo (inferência e análise)
│   └── utils/                   # Funções auxiliares
│
├── results/
│   ├── inferencias/             # Respostas brutas dos LLMs
│   ├── metricas/                # Cálculo de MAE, MAPE, acurácia etc.
│   └── graficos/                # Visualizações geradas para o TCC
│
├── documento/
│   ├── TCC.pdf                  # Versão final da monografia
│   └── anexos/
│
└── README.md                    # (este arquivo)

- Métricas Avaliadas

Os modelos foram avaliados com base em:

MAE – Erro Absoluto Médio

MAPE – Erro Percentual Absoluto Médio

Acurácia de Identificação (produto correto × descrição original)

Concordância entre avaliadores humanos

- Recorte da Pesquisa

10 maiores cidades do Paraná

2021 a 2024 (pós-pandemia e Nova Lei de Licitações)

Segmentos analisados:

Materiais escolares

Equipamentos de informática

Esses dois grupos foram escolhidos pela alta recorrência em licitações e risco de superfaturamento.

- Referências principais do projeto

VASWANI et al. Attention is All You Need (2017)

JURAFSKY; MARTIN. Speech and Language Processing (2020)

OpenAI (2024–2025), Anthropic (2024), DeepSeek AI (2024)

BERGER et al. (2024) — Ferramenta Julius

MORENO et al. (2022); LIMA; FERREIRA (2023)

Lei 14.133/2021 — Nova Lei de Licitações

Lei 12.527/2011 — Lei de Acesso à Informação

- Como Reproduzir o Pipeline

Clone o repositório

Instale as dependências

Configure suas variáveis de ambiente com as chaves das APIs

Execute o notebook pipeline_colab.ipynb

Gere métricas e gráficos automaticamente

- Licença

Este projeto está sob a licença Creative Commons BY-NC-ND 4.0, conforme presente em seu TCC.
Uso permitido com atribuição, sem fins comerciais e sem modificações.

- Contato

Autor: Luiz Eduardo Zanatta Sendeski

Coautor: Robson Barbieri Candido

Instituição: Instituto Federal do Paraná – Campus Palmas

Orientação: Prof.ª Andreia Marini • Prof. Tarlis Tortelli Portela
