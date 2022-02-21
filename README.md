# cotas-genero-e-proposicoes-legislativas
TCC da pós-graduação em Inteligência Artificial e Aprendizado de Máquina da @pucminas (em construção)

[Descrever objetivo do projeto + hipóteses (perguntas) + adicionar relatóorio técnico após a aprovação + linkar relatório no readme]

# Instalando

# Sugestão de leitura dos notebooks
Sugiro que os notebooks sejam lidos de acordo com o pipeline de uma análise de dados:

```
                                 ┌──────────────┐     ┌──────────────┐
                                 │ Tratamento   │     │ Analise      │
                  ┌─Candidaturas─┤ de dados     ├─────┤ de dados     │
┌────────────┐    │ eleitas      │ candidaturas │     │ candidaturas │
│ Coleta de  │    │              │ eleitas      │     │ eleitas      │
│ dados      │    │              └──────────────┘     └──────────────┘
│            ├────┤
└────────────┘    │              ┌──────────────┐     ┌──────────────┐    ┌──────────────┐
                  │              │ Tratamento   │     │ Tratamento   │    │ Analise      │ 
                  └─Proposicoes──┤ de dados     ├─────┤ de dados     ├────┤ de dados     │
                    legislativas │ proposicoes  │     │ criacao      │    │ proposicoes  │ 
                                 │ legislativas │     │ vocabulario  │    │ legislativas │ 
                                 └──────────────┘     └──────────────┘    └──────────────┘    
```