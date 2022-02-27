# cotas-genero-e-proposicoes-legislativas
TCC da pós-graduação em Inteligência Artificial e Aprendizado de Máquina da @pucminas (em construção)

[Descrever objetivo do projeto + hipóteses (perguntas) + adicionar relatóorio técnico após a aprovação + linkar relatório no readme]

# Instalando

# Sugestão de leitura dos notebooks
Sugiro que os notebooks sejam lidos de acordo com o pipeline de uma análise de dados:

```
                       ┌─────────────┐ ┌─────────────┐
                       │             │ │             │
                       │ Tratamento  │ │ Analise     │
             ┌─Candid ─┤ de dados    ├─┤ de dados    │
             │ eleitas │ candidaturas│ │ candidaturas│
             │         │ eleitas     │ │ eleitas     │
             │         │             │ │             │
             │         └─────────────┘ └─────────────┘
             │
┌─────────┐  │
│         │  │         ┌────────────┐ ┌────────────┐ ┌───────────┐ ┌──────────┐ ┌────────────┐
│         │  │         │            │ │            │ │           │ │Classifi- │ │            │
│Coleta de│  │         │Tratamento  │ │Tratamento  │ │Tratamento │ │cador de  │ │Analise     │
│dados    ├──┼─Propo ──┤de dados    ├─┤de dados    ├─┤de dados   ├─┤proposi-  ├─┤de dados    │
│         │  │ legis   │legislaturas│ │proposicoes │ │criacao    │ │coes      │ │proposicoes │
│         │  │         │            │ │legislativas│ │vocabulario│ │legislati-│ │legislativas│
└─────────┘  │         │            │ │            │ │           │ │vas       │ │            │
             │         └────────────┘ └────────────┘ └───────────┘ └──────────┘ └────────────┘
             │
             │         ┌──────────┐ ┌───────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐
             │         │          │ │           │ │          │ │          │ │          │
             │         │Tratamento│ │ Tratamento│ │Tratamento│ │Tratamento│ │Classifi- │
             └─Modelo──┤de dados  ├─┤ de dados  ├─┤de dados  ├─┤de dados  ├─┤cador de  │
               aprend  │legisla-  │ │ candida-  │ │proposi-  │ │criacao   │ │proposi-  │
               maquina │turas     │ │ turas     │ │coes      │ │vocabu-   │ │coes      │
                       │          │ │ eleitas   │ │legisla-  │ │lario     │ │legislati-│
                       │          │ │           │ │tivas     │ │          │ │vas       │
                       │          │ │           │ │          │ │          │ │          │
                       └──────────┘ └───────────┘ └──────────┘ └──────────┘ └──────────┘
```

Links para os notebooks:
- [Coleta de dados](coleta.ipynb)
- [Tratamento de dados - candidaturas eleitas](tratamento-dados/tratamento-candidaturas-eleitas.ipynb)
- [Tratamento de dados - legislaturas](tratamento-dados/tratamento-legislaturas.ipynb)
- [Tratamento de dados - proposicões legislativas](tratamento-dados/tratamento-proposicoes.ipynb)
- [Tratamento de dados - criação de vocabulário](tratamento-dados/criacao-vocabulario.ipynb)
- [Tratamento de dados - predição](tratamento-dados/tratamento-predicao.ipynb)
- [Análise de dados - candidaturas eleitas](analise-dados/analise-candidaturas-eleitas.ipynb)
- [Análise de dados - proposicões legislativas](analise-dados/analise-proposicoes.ipynb)
- [Modelo de aprendizado de máquina - Predição do percentual de proposições...](prever-percentual-proposicoes-beneficentes-grupos-historicamente-marginalizados.ipynb)
