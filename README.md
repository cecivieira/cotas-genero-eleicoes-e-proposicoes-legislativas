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
                ┌─Candidaturas─┤ de dados    ├─┤ de dados    │
                │ eleitas      │ candidaturas│ │ candidaturas│
                │              │ eleitas     │ │ eleitas     │
                │              │             │ │             │
                │              └─────────────┘ └─────────────┘
                │
   ┌─────────┐  │
   │         │  │              ┌────────────┐ ┌────────────┐ ┌───────────┐ ┌────────────┐
   │         │  │              │            │ │            │ │           │ │            │
   │Coleta de│  │              │Tratamento  │ │Tratamento  │ │Tratamento │ │Analise     │
   │dados    ├──┼─Proposicoes──┤de dados    ├─┤de dados    ├─┤de dados   ├─┤de dados    │
   │         │  │ legislativas │legislaturas│ │proposicoes │ │criacao    │ │proposicoes │
   │         │  │              │            │ │legislativas│ │vocabulario│ │legislativas│
   └─────────┘  │              │            │ │            │ │           │ │            │
                │              └────────────┘ └────────────┘ └───────────┘ └────────────┘
                │
                │              ┌────────────┐ ┌────────────┐ ┌───────────┐ ┌──────────┐ ┌────────────┐
                │              │            │ │            │ │           │ │          │ │Prever      │
                │              │Tratamento  │ │Tratamento  │ │Tratamento │ │Tratamento│ │percentual  │
                └─Modelo de────┤de dados    ├─┤de dados    ├─┤de dados   ├─┤de dados  ├─┤proposicoes │
                  aprendizado  │legislaturas│ │proposicoes │ │criacao    │ │predicao  │ │beneficentes│
                  de maquina   │            │ │legislativas│ │vocabulario│ │          │ │grupos hist │
                               │            │ │            │ │           │ │          │ │marginalizados
                               └────────────┘ └────────────┘ └───────────┘ └──────────┘ └─────────────

   
```

Links para os notebooks:
[Coleta de dados]()
[Tratamento de dados - candidaturas eleitas]()
[Tratamento de dados - proposicões legislativas]()
[Tratamento de dados - criação de vocabulário]()
[Análise de dados - candidaturas eleitas]()
[Análise de dados - proposicões legislativas]()