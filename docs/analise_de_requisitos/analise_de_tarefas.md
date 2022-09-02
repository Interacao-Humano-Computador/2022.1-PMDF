# Análise de Tarefas 

## 1. Introdução

Segundo Perce [1], a análise de tarefas trata-se de um termo "guarda-chuva" que abrange técnicas utilizadas na investigação de situações existentes e cujo objetivo é
identificar o andamento e o propósito do que está sendo realizado pelo usuário. Essas técnias costumam, também,
avaliar a situação em pequenos detalhes e em um alto nível de abstração. Alguns exemplos delas são a análise de tarefa KLM e CMN, a árvore de
tarefas concorrentes CTT e, principalmente, a Análise Hierárquica de Tarefas HTA.

Barbosa e Silva [2] complementa a afirmação de Pierce ao pontuar que a análise
de tarefas pode ser utilizada para a análise da situação atual, para o (re)design
de um sistema computacional ou para a avaliação do resultado de uma intervenção que inclua a introdução de um (novo) sistema
computacional.

## 2. Análise Hierárquica de tarefas (HTA)

Auxilia a indentificar o que as pessoas fazem, o porquê e as consequências caso não façam corretamente, ideia baseada na psicologia funcional. Nesse tipo de análise são utilizadas tarefas, onde são definidas como pequenas partes do trabalho que precisam ser realizadas, ou objetivos. Segundo diaper podemos utilizar da decomposição de tarefas ou redescrição para dividir em objetivos e subobjetivos tarefas mais complexas.

O HTA busca examinar objetivos de alto nível e decompor estes em subojetivos, subojetivos são relacionados com outros objetivos indicando um plano, que definem os subojetivos para que os objetivos maiores sejam atingidos.

Segundo dados obtidos através do questionário é podemos inferir que a funcionalidade intranet é a mais utilizada pelos usuário e será nosso objeto de estudo para a
Objetivo: Modificar um sistema existente.

### 2.1 Objetivo: Logar na Intranet

#### Representação Gráfica

| ![image](https://user-images.githubusercontent.com/60429513/180089432-2413ef7c-8188-4e37-88b7-f13d0ef10c1e.png) |
|-----------------------------------------------------------------------------------------------------------------|
| Figura 1: representação do objetivo de logar na intranet; Fonte: autoria própria.                               |

#### Representação Textual

| Objetivo                               | input / Action / feedback / Problema                                                                                                                                                                                                 |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 0. Logar no Intranet                   | -                                                                                                                                                                                                                                    |
| 1. acessar página intranet             | Input: área descrita "intranet", action: clicar no botão "intranet", Problema: pequena caixa para inserir nome de usuário e senha , Recomendação: utilizar uma pagina facilitando a visualização para usuários com problema de vista |
| 1.1 Informar Dados do usuário          | -                                                                                                                                                                                                                                    |
| 1.1.1 Informar nome de usuário e senha | Inputs: áreas descritas "nome de usuário" e "senha", action: digitar dados                                                                                                                                                           |
| 2. clicar em fazer login               | Input: inputs: área descrita "fazer login" action: clicar em botão "fazer login"                                                                                                                                                     |

Tabela 1: Elementos do objetivo - logar na intranet

## 3. GOMS (<i>Goals, Operators, Methods and Selection Rules</i>)

Trata-se de um método para descrever tarefas que pontua o conhecimento do usuário
sobre como realizá-la tendo em vista seus objetivos (<i>goals</i>), os operadores utilizados (<i>operators</i>),
os métodos (<i>methods</i>) disponíveis e as regras de seleção (<i>selection rules</i>), cuja descrição consta na Tabela 2.

|              Elementos              |                                                       Descrição                                                        |
|:-----------------------------------:|:----------------------------------------------------------------------------------------------------------------------:|
|      Objetivos (<i>Goal</i>)        |                                          O que o usuário pretende realizar ao utilizar o software                      |
|       Operadores (<i>OP</i>)        |                        Ações disponibilizadas pelo sistema que de fato o usuário pode realizar                         |
|       Métodos (<i>METHOD</i>)       |                     Sequências de operadores utilizadas para atingir um objetivo dentro do sistema                     |
| Regras de seleção (<i>SEL.RULE</i>) | Referem-se a tomada de decisão por parte do usuário diante da possibilidade de possuir mais de um método para utilizar |

Tabela 2: Elementos da abordagem GOMS

### 3.1 KLM - GOS

Estratégia prática que implementa os princípios do GOMS limitando os operadores a um conjunto pré-definido. O nome e a descrição
acompanhados do tempo médio para execução, elementos dessa estratégia, constam na Tabela 2.

| Operador |                 Descrição                  | Tempo médio para execução |
|:--------:|:------------------------------------------:|:-------------------------:|
|  _K_     |          Pressionar e soltar uma tecla     |               0,25s       |
|   _P_    |      Levar o cursor até algo na tela       |           1,10s           |
|   _B_    |   Soltar ou pressionar um botão do mouse   |           0,10s           |
|   _H_    |   Transitar a mão entre teclado e mouse    |           0,40s           |
|   _M_    |             Preparação mental              |           1,20s           |
|  _T(n)_  |     Digitação de cadeia de caracteres      |         (n x K) s         |
|  _W(t)_  | Espera do usuário pela resposta do sistema |   dependente do sistema   |

Tabela 3: Elementos da implementação KLM - GOS

#### 3.1.1 Análise de tarefa: consultar salário de servidor

| Operador |                      Descrição                      | Tempo médio para execução |
|:--------:|:---------------------------------------------------:|:-------------------------:|
|  _M_     |                           preparação                |             1,50s         |
|   _P_    |       levar o cursor até o botão "Servidores"       |           0,50s           |
|   _B_    |           pressionar o botão "Servidores"           |           0,05s           |
|   _B_    |             soltar o botão "Servidores"             |           0,05s           |
|   _P_    | levar o mouse até o link do portal da transparência |           0,05s           |
|   _B_    |      soltar o link do portal da transparência       |           0,05s           |

Tabela 4: Elementos da implementação KLM - GOS para a consulta de salário de servidor

### 3.2 CMN - GOS

O CMN-GOMS possui uma hierarquia estrita de objetivos na qual os operadores são executados
estritamente em ordem sequencial e os métodos são representados numa notação semelhante
a um pseudocódigo, que inclui submétodos e condicionais.

#### 3.1.1 Análise de tarefa: consultar salário de servidor

```
Goal 0: Consultar salário de servidor
    Goal 1: Encontrar o link para consulta do salário do servidor
    METHOD 1.A: Encontrar através do menu lateral
        OP: Levar cursor até o menu lateral.
        OP: Levar o cursor até o botão "Servidores" .
        OP: Levar o mouse até o link do portal da transparência.
        OP: clicar com o botão direito do mouse.
```

## Referências Bibliográficas

Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021) Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1.R

## Histórico de Versões

| Versão  | Data  | Descrição                   | Autor           | Revisor           |
|---------|-------|-----------------------------|-----------------|-------------------|
| 1.0     | 20/07 | Análise de tarefas          | Arthur          | Bernardo Pissutti |
| 1.1     | 20/07 | Adição de novas estratégias | Nícolas Mantzos | Bernardo Pissutti |
