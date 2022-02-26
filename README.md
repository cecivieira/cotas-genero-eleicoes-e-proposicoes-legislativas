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
│         │  │         ┌────────────┐ ┌────────────┐ ┌───────────┐ ┌────────────┐
│         │  │         │            │ │            │ │           │ │            │
│Coleta de│  │         │Tratamento  │ │Tratamento  │ │Tratamento │ │Analise     │
│dados    ├──┼─Propo ──┤de dados    ├─┤de dados    ├─┤de dados   ├─┤de dados    │
│         │  │ legis   │legislaturas│ │proposicoes │ │criacao    │ │proposicoes │
│         │  │         │            │ │legislativas│ │vocabulario│ │legislativas│
└─────────┘  │         │            │ │            │ │           │ │            │
             │         └────────────┘ └────────────┘ └───────────┘ └────────────┘
             │
             │         ┌──────────┐ ┌───────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌───────────┐
             │         │          │ │           │ │          │ │          │ │          │ │Prever     │
             │         │Tratamento│ │ Tratamento│ │Tratamento│ │Tratamento│ │Tratamento│ │percentual │
             └─Modelo──┤de dados  ├─┤ de dados  ├─┤de dados  ├─┤de dados  ├─┤de dados  ├─┤proposi-   │
               aprend  │legisla-  │ │ candida-  │ │proposi-  │ │criacao   │ │predicao  │ │coes em    │
               maquina │turas     │ │ turas     │ │coes      │ │vocabu-   │ │          │ │favor de   │
                       │          │ │ eleitas   │ │legisla-  │ │lario     │ │          │ │grupos hist│
                       │          │ │           │ │tivas     │ │          │ │          │ │margina    │
                       │          │ │           │ │          │ │          │ │          │ │lizados    │
                       └──────────┘ └───────────┘ └──────────┘ └──────────┘ └──────────┘ └───────────┘ 
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
