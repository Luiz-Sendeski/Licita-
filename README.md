# 📘 LICITA+ — Aplicação de IA na Fiscalização de Licitações Públicas  
*(TCC – IFPR, 2025)*

Este repositório contém o projeto **LICITA+**, desenvolvido como Trabalho de Conclusão de Curso no Instituto Federal do Paraná.  
O objetivo é aplicar **Grandes Modelos de Linguagem (LLMs)** para identificar possíveis irregularidades em licitações públicas, como:

- Ambiguidade em descrições  
- Itens duplicados  
- Possível superfaturamento  
- Inconsistências textuais que dificultam a fiscalização  

O sistema analisa **descrições textuais brutas** de editais — sem pré-processamento — e compara o desempenho de três modelos:

- **GPT-4o-mini (OpenAI)**  
- **Claude Sonnet 4.5 (Anthropic)**  
- **DeepSeek-V2 (DeepSeek AI)**  

---

## 🎯 Objetivo Geral

Desenvolver e validar um sistema baseado em Inteligência Artificial capaz de interpretar descrições de itens licitatórios e estimar preços médios reais, contribuindo para a transparência e fiscalização pública.

---

## 🧩 Tecnologias Utilizadas

- Python 3.10+  
- Google Colab  
- OpenAI API  
- Anthropic API  
- DeepSeek API  
- Pandas, NumPy, SciPy  
- Matplotlib  
- OpenPyXL  

---

## 📂 Estrutura do Repositório

```text
/
├── data/                # Dados brutos e organizados (editais, planilhas, cotações)
├── src/                 # Scripts e pipeline (prompts, chamada às APIs, validações)
├── results/             # Gráficos, métricas e inferências geradas
├── documento/           # Versão final do TCC em PDF/LaTeX
└── README.md            # Este arquivo

## 📁 Arquivos Complementares no Google Drive

Alguns materiais utilizados no desenvolvimento deste projeto estão disponíveis também no Google Drive, incluindo documentos auxiliares, versões intermediárias de planilhas e arquivos de apoio:

🔗 **Acessar pasta no Google Drive:**
https://drive.google.com/drive/folders/1g0RWxph3-KLcATF7IRY0Rql7pchmRdjA?usp=sharing
