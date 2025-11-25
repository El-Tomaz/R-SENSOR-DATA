# Análise de dados de sensores em R

Este é o meu primeiro projeto em R!!! 

A aquisição dos dados foi realizada utilizando 6 termopares tipo K, junto com módulos MAX6675 e esp32, se tiver interesse em acompanhar o desenvolvimento do hardware, pode conferi-lo neste outro repositório: [https://github.com/El-Tomaz/TELEMETRIA-PAINEL-SOLAR](https://github.com/El-Tomaz/TELEMETRIA-PAINEL-SOLAR).

Os dados foram coletados durante 5 ensaios de temperatura, nos quais os termopares foram inseridos dentro de um banho termoestático, com precisão de temperatura de ~ +- 0.1 °C. Além disso, utilizei um termometro de mercúrio para conferir a temperatura do banho durante todo o processo. Cada medição durou 5 minutos, garantindo tempo suficiente para estabilização térmica dos sensores.

As temperaturas selecionadas em cada ensaio foram 20°C, 25°C, 30°C, 35°C e 40°C.

## Descrição do repositório

- [termopar2.Rmd](./termopar2.Rmd): Código em RMarkdown, aqui está todo o código em R que desenvolvi, visite este arquivo para conferir o meu trabalho.
- [termopar2.pdf](./termopar2.pdf): Arquivo gerado através do código que desenvolvi. Confira-o para ver o resultado deste projeto. 
- [termopar.csv](./termopar.csv): dados de temperatura dos sensores "crus".

- termopar.Rmd: Código em RMarkdown antigo, deixei apenas para comparação, mas não foi finalizado. Se quiser ver a versão mais atualizada, configura termopar2.Rmd.
- termopar.pdf: PDF antigo gerado. Está incompleto, para ver a versão final vá para termopar2.pdf. Se quiser ver a versão mais atualizada, configura termopar2.pdf. 

## Algumas prints do resultado

Configura todo o conteúdo em [termopar2.pdf](./termopar2.pdf).

![](./prints/tab.PNG)

![](./prints/bin.PNG)
![](./prints/dot.PNG)

## O que aprendi 

Durante este projeto aprendi:

- **Sintaxe básica da linguagem R**, principais operadores, controle de fluxo, loops, tipos básicos
- **Criação e manipulação de Dataframes**, uso de funções como subset, lapply,sapply
- **Converção entre formatos wide e long** com funções `pivot_longer` e `pivot_wider`
- **Criação de gráficos com ggplot2** , mapeamento, uso de diferentes geometrias, facets e classificações.
- **Uso do RMarkdown**, incluindo configuração básica do Knitr (algo que pretendo aprender melhor, assim como o pandoc)

Pacotes que utilizei:
- [ggplot2](https://ggplot2.tidyverse.org/)
- [tidyr](https://tidyr.tidyverse.org/)
- [lubridate](https://lubridate.tidyverse.org/)
- [lemon_print](https://cran.r-project.org/web/packages/lemon/vignettes/lemon_print.html)