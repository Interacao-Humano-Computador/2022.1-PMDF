# Análise de Tarefas

## 1. Introdução

Segundo Perce [1], a análise de tarefas trata-se de um termo "guarda-chuva"  
que abrange técnicas utilizadas na investigação de situações existentes e cujo objetivo é
identificar o andamento e o propósito do que está sendo realizado pelo usuário. Essas técnias costumam, também,
avaliar a situação em pequenos detalhes e em um alto nível de abstração. Alguns exemplos delas são a análise de tarefa KLM e CMN, a árvore de
tarefas concorrentes CTT e, principalmente, a Análise Hierárquica de Tarefas HTA.

Barbosa e Silva [2] complementa a afirmação de Pierce [1] ao pontuar que a análise
de tarefas pode ser utilizada para a análise da situação atual, para o (re)design
de um sistema computacional ou para a avaliação do resultado de uma intervenção que inclua a introdução de um (novo) sistema
computacional.

## 3. GOMS (<i>Goals, Operators, Methods and Selection Rules</i>)

Trata-se de um método para descrever tarefas que pontua o conhecimento do usuário
sobre como realizá-la tendo em vista seus objetivos (<i>goals</i>), os operadores utilizados (<i>operators</i>),
os métodos (<i>methods</i>) disponíveis e as regras de seleção (<i>selection rules</i>), cuja descrição consta na Tabela 1.

|Elementos |                                  Descrição                                  |
| :------: |:----------------------------------------------------------------------------:|
Objetivos | O que o usuário pretende realizar ao utilizar o software                        |         
Operadores | Ações disponibilizadas pelo sistema que de fato o usuário pode realizar        |
Métodos |  Sequências de operadores utilizadas para atingir um objetivo dentro do sistema                                         | 
Regras de seleção | Referem-se a tomada de decisão por parte do usuário diante da possibilidade de possuir mais de um método para utilizar |
_Tabela 1: Elementos da abordagem GOMS_

### 3.1 KLM - GOS

Estratégia prática que implementa os princípios do GOMS limitando os operadores a um conjunto pré-definido. O nome e a descrição 
acompanhados do tempo médio para execução, elementos dessa estratégia, constam na Tabela 2.

|Operador |                                  Descrição                                  | Tempo médio para execução |
| :------: |:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
*K* | Pressionar e soltar uma tecla                      |   0,25s      |
*P*  | Levar o cursor até algo na tela        | 1,10s |
*B*  | Soltar ou pressionar um botão do mouse        |   0,10s |
*H*  | Transitar a mão entre teclado e mouse       |  0,40s |
*M*  | Preparação mental       | 1,20s |
*T(n)*  | Digitação de cadeia de caracteres        |   (n x K) s    |
*W(t)*  | Espera do usuário pela resposta do sistema        | dependente do sistema      |
Tabela 1: Elementos da implementação KLM - GOS

#### 3.1.1 Análise de tarefa: consultar salário de servidor

|Operador |                                  Descrição                                  | Tempo médio para execução |
| :------: |:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
*M* | preparação                      |   1,50s      |
*P*  | levar o cursor até o botão "Servidores"        | 0,50s |
*B*  | pressionar o botão "Servidores"        | 0,05s |
*B*  | soltar o botão "Servidores"        | 0,05s |
*P*  | levar o mouse até o link do portal da transparência        |   0,05s |
*B*  | soltar o link do portal da transparência        | 0,05s |
Tabela 2: Elementos da implementação KLM - GOS para a consulta de salário de servidor

### 3.2 CMN - GOS

O CMN-GOMS possui uma hierarquia estrita de objetivos na qual os operadores são executados 
estritamente em ordem sequencial e os métodos são representados numa notação semelhante 
a um pseudocódigo, que inclui submétodos e condicionais. 

#### 3.1.1 Análise de tarefa: consultar salário de servidor

~~~
Goal 0: Consultar salário de servidor
    Goal 1: Encontrar o link para consulta do salário do servidor
    METHOD 1.A: Encontrar através do menu lateral
        OP: Levar cursor até o menu lateral.
        OP: Levar o cursor até o botão "Servidores" .
        OP: Levar o mouse até o link do portal da transparência.
        OP: clicar com o botão direito do mouse.
        
~~~

## Histórico de Versões

| Versão | Data       | Descrição                                              | Autor                    |
|--------|------------|--------------------------------------------------------|--------------------------|
|  1.0      |  18/07/2022          |  Criação e documentação das primeiras análises |   Nicolas Mantzos                       |
