# Política de Branches

Padronização das branches no projeto. 

## Histórico de Versões


| Data       | Versão | Descrição                                 | Autor             |
| :--------: | :----: | :----------:                              | :---------------: |
| 10/08/2021 |  0.1   | Criação da política de branch             | [Lameque Fernandes](https://github.com/LamequeFernandes)|
| 11/08/2021 |  0.2   |            Alterações                     | [Lameque Fernandes](https://github.com/LamequeFernandes)|
| 16/08/2021 |  0.3   |Adição da explicação sobre a branch develop| [Lameque Fernandes](https://github.com/LamequeFernandes)|


## Padronização das Branches

### Prefixos:
- ```feature/```
- ```hotfix/```
- ```documentation/```
- ```improvement/```

### Formato:
```
<prefixo>(#número da issue): assunto
```
Não esquecer de dividir as palavras do assunto com "-".
Exemplo: 
```
feature(#87)/novo-menu
```

### Branches:

- **Branch main:** Branch que contém o código em nível de produção, será o código mais consolidado existente na aplicação. Nenhum integrante dos times é autorizado a fazer commits diretamente na *main.*

- **Branch develop:** 
A main irá contér todo código já testado, versionado que será entregue ao cliente e a **develop** é onde todo fluxo de trabalho irá ocorrer antes de fazer o release versionado que será feito merge na main.
Quando as features são terminadas, elas são juntadas nesta branch, testadas e somente depois as atualizações da develop passam pelo processo de juntar as novas atualizações com a branch main;
A **develop** deve sempre conter o código mais atual, onde as branchs de features serão ramificadas tendo ela como base.


- **Branches feature:** Como o nome já diz, são branches na qual são desenvolvidos novos recursos ao projeto. São criadas começando com o prefixo **feature/**.
Exemplo: ```feature(#22)/novo-layout```

- **Branchs hotfix:** Branches no qual são realizadas correções de bugs São criadas começando com o prefixo **hotfix/**.
Exemplo: ```hotfix(#02)/correcao-botao```

- **Branches documentation:** Branches na qual são desenvolvidos os documentos do projeto. São ciradas começando com o prefixo **documentation/**
Exemplo: ```documentation(#49)/template-documento```

- **Branches improvement:** Branche para melhoria de algum componente e afins, seja de performance, de escrita de layout, etc. Exemplo: ```improvement(#101)/otimizacao-layout```

### Princípios:
- Por ser um projeto voltado totalmente para um público brasileiro e por toda equipe ter mais afinidade com o português, foi decidido que todas as braches serão em pt-BR.

## Referências

DULCETTI, Bruno. Padrões e nomenclaturas no Git. *BrunoDulcetti*. Disponível em: <https://www.brunodulcetti.com/padroes-e-nomenclaturas-no-git/>. Acesso em: 10 de ago. de 2021.

Políticas de Branches. Disponível em: <https://fga-eps-mds.github.io/2018.2-ComexStat/docs/politicaBranches>. Acesso em: 10 de ago. de 2021

HADLER, Mikael. Utilizando o fluxo Git Flow. *Medium*. Disponível em: <https://medium.com/trainingcenter/utilizando-o-fluxo-git-flow-e63d5e0d5e04>. Acesso em: 16 de ago. de 2021