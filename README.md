# Cotas de gênero e seu impacto nas eleições e proposições legislativas da Câmara dos Deputados Federais: uma análise entre 1934 e 2021

> Notebooks do trabalho de conclusão de curso apresentado ao curso de pós-graduação em Inteligência Artificial e Aprendizado de Máquina da @pucminas. O relatório técnico pode ser lido em [link em breve]

Neste repositório são analisados os dados das candidaturas eleitas para a Câmara dos Deputados do país a partir de 1934 - um ano após a primeira eleição cujas mulheres puderam votar e serem votadas - a fim de identificar o impacto da legislação com ações afirmativas de gênero em eleições proporcionais no quantitativo de mulheres eleitas para o cargo de deputada federal. Além disso, também são analisadas as proposições legislativas (exclusivamente, projetos de lei, de resolução e de decreto) apresentadas no mesmo período, com o objetivo de verificar a existência de correlação entre os pontos citados anteriormente. 

Vale ressaltar que existem registros apenas de algumas proposições tramitadas entre os anos de 1934 e 1945, além disso os dados das proposições legislativas entre os anos de 1946 e 2000 estão parcialmente disponibilizados - estão abertos apenas os referentes às “proposições de tipos que poderiam se tornar (ou se tornaram) leis e normas jurídicas” (Brasil, [2021?]), sendo assim as análises realizadas com os dados desse período podem não refletir a realidade.

Além disso, ressalta-se, também, que não foi realizado um estudo aprofundado em Ciência da Informação para a criação de vocabulário controlado usado neste relatório, sendo assim esta análise destina-se apenas ao exercício proposto para este trabalho de conclusão de curso.

## Requisitos

- Matplotlib
- NLTK
- Numpy
- Pandas
- NLTK
- Scikit-learn
- Seaborn

## Instalação e execução

1. Instale/Ative um ambiente virtual;
2. Instale os requisitos:
   `pip install requirements.txt`
3. Rode os notebooks:
   `jupyter lab`

## Sugestão de leitura
Os notebooks devem ser lidos de acordo com o seguinte fluxo:

```
                       ┌─────────────┐ ┌─────────────┐
                       │             │ │             │
               Analise │ Tratamento  │ │ Analise     │
             ┌─Candid ─┤ de dados    ├─┤ de dados    │
             │ eleitas │ candidaturas│ │ candidaturas│
             │         │ eleitas     │ │ eleitas     │
             │         │             │ │             │
             │         └─────────────┘ └─────────────┘
             │
┌─────────┐  │
│         │  │         ┌───────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌────────┐
│         │  │         │           │ │          │ │          │ │          │ │Classifi- │ │        │
│Coleta de│  │ Analise │Tratamento │ │Tratamento│ │Tratamento│ │Tratamento│ │cador de  │ │Analise │
│dados    ├──┼─Propo ──┤de dados   ├─┤de dados  ├─┤de dados  ├─┤de dados  ├─┤proposi-  ├─┤de dados│
│         │  │ legis-  │candida-   │ │legisla-  │ │propo     │ │criacao   │ │coes      │ │propo   │
│         │  │ lativas │turas      │ │tivas     │ │legisla-  │ │vocabu-   │ │legislati-│ │legisla-│
└─────────┘  │         │eleitas    │ │          │ │tivas     │ │lario     │ │vas       │ │tivas   │
             │         └───────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └────────┘
             │
             │
             │         ┌──────────┐ ┌───────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐
             │         │Tratamento│ │ Tratamento│ │Tratamento│ │Tratamento│ │Classifi- │
             └─Modelo──┤de dados  ├─┤ de dados  ├─┤de dados  ├─┤de dados  ├─┤cador de  │
               aprend  │legisla-  │ │ candida-  │ │proposi-  │ │criacao   │ │proposi-  │
               maquina │turas     │ │ turas     │ │coes      │ │vocabu-   │ │coes      │
                       │          │ │ eleitas   │ │legisla-  │ │lario     │ │legislati-│
                       │          │ │           │ │tivas     │ │          │ │vas       │
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
- [Modelo de aprendizado de máquina - Classificador de proposições legislativas](classifica-proposicoes.ipynb)

## Licença
MIT