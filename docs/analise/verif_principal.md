# Verificação

## 1. Introdução

Segundo _Serrano_, a verificação pode ser entendida como _uma análise de modelos sem que haja direta comparação com o Universo de Informações_, sendo essa análise uma tarefa desempenhada tanto por seres humanos quanto por software, seguindo regras bem definidas e cujo objetivo principal é analisar se os artefatos estão sendo construídos corretamente.

## 2. Metodologia

As verificações utilizarão, primariamente, as seis etapas definidas pelo método de Fagan (1976) adaptadas. Sendo elas:

### 2.1 Planejamento (*Planning*)

O objetivo é organizar o ambiente, físico ou virtual, no qual a inspeção se dará, reunindo os participantes e separando os materiais necessários.

### 2.2 Visão Geral (*Overview*)

Nesta etapa, os participantes da tarefa de inspeção são deixados a par dos materiais em análise e funções são atribuídas a cada um deles, determinando quem avaliará qual artefato. 

### 2.3 Preparação (*Preparation*)

Nesta etapa, segundo Fagan, *os participantes revisam o item a ser inspecionado e o material de apoio, anotando quaisquer dúvidas ou possíveis defeitos encontrados.*
Nesse sentido, optamos por elicitar e listar os "defeitos encontrados" como perguntas advindas da avaliação do professor nas apresentações, dos monitores nos relatórios e da bibliografia, a fim de cobrir os aspectos mais variados e relevantes do artefato. 
Cada pergunta estará acompanhada de um identificador para referência posterior, como consta na tabela exemplificativa 1 abaixo.

| Pergunta        | Identificador   |
|-----------------|-----------------|
| _p<sub>1</sub>_ | _i<sub>1</sub>_ |
| _p<sub>2</sub>_ | _i<sub>2</sub>_ |
| _p<sub>3</sub>_ | _i<sub>3</sub>_ |
| ...             | ...             |
| _p<sub>n</sub>_ | _i<sub>n</sub>_ |

_Tabela 1: Tabela exemplificativa de itens e seus identificadores_

### 2.4 Inspeção (*Meeting/Inspection*)

Aqui, os defeitos são encontrados. Para tal, os itens destacados na etapa de preparação serão inspecionados justapondo-os em uma tabela com duas colunas: _Identificador_ e _Situação_, referindo-se, respectivamente ao n-ésimo _i<sub>n</sub>_ da tabela 1
e a um dos ícones da tabela 3. No caso, "✅" qualificando o item como "Atendido" e "❌" o tornando "Não atendido", como pode ser visto na tabela 2.

| Identificador   | Situação  |
|-----------------|-----------|
| _i<sub>1</sub>_ | ✅         |
| _i<sub>2</sub>_ | ✅         |
| _i<sub>3</sub>_ | ❌         |
| _i<sub>4</sub>_ | ✅         |
| ...             | ...       |
| _i<sub>n</sub>_ | ❌         |

_Tabela 2: Tabela exemplificativa de inspeção de itens (checklist)_

| Símbolo   | Significado   |
|:---------:|:-------------:|
|     ✅     |   Atendido    |
|     ❌     | Não atendido  |

_Tabela 3: Símbolos utilizados nas checklists e seus significados_

A partir dessa resposta, um gráfico de pizza como o da figura 1, compilando a porcentagem de itens atendidos e
não atendidos, será montado para facilitar a análise dos resultados e melhorar o rastreamento dos itens
nas próximas fases.

| ![imagemGráfico](../_media/grafico_guiadeestilo.png)            |
|-----------------------------------------------------------------|
| Figura 1: Exemplo de gráfico de itens atendidos e não atendidos |

Por fim, haverá uma conclusão determinando se o artefato deve ou não ser corrigido, quais pontos devem ser priorizados em uma eventual correção etc

### 2.5 Correção/retrabalho (*Rework*)

A correção (ou retrabalho) é a *etapa na qual os defeitos encontrados durante a inspeção são resolvidos pelo autor, projetista ou programador*.
Para esta fase, portanto, foi(ram) alocado(s) o(s) membro(s) da equipe responsável(eis) pela criação do artefato.

### 2.6 Acompanhamento (*Follow-up*)

Na fase de acompanhamento, todos os defeitos devem ser efetivamente corrigidos, sendo de responsabilidade de um
moderador verificar se isso realmente aconteceu. Além disso, ele deve se certificar de que nenhum novo defeito foi introduzido no processo de correção.
Foi alocado, para esse papel, um membro da equipe que não realizou a inspeção nem participou da criação do artefato, objetivando evitar enviesamento.

O fluxo do processo de inspeção de Fagan pode ser observado na figura 2 abaixo.

| ![imagemGráfico](../_media/verificacao_inspecao_fagan.jpeg)       |
|-------------------------------------------------------------------|
| Figura 2: Fluxo da inspeção de Fagan                              |

## 3. Verificação

### 3.1 Análise de Requisitos

[Verificação 01 : Perfil do Usuário](analise/verificacoes/verif_perfil_de_usuario.md)<br>
[Verificação 02 : Personas](analise/verificacoes/verificacao_personas.md)<br>
[Verificação 03 : Análise de Tarefas](analise/verificacoes/verif_analiseTarefa)<br>
[Verificação 04 : Princípios Gerais](analise/verificacoes/verif_principios_gerais.md)<br>
[Verificação 05 : Metas de Usabilidade](analise/verificacoes/verificacao_metas.md)<br>
[Verificação 06 : Guia de Estilo](analise/verificacoes/verificacao_guia_estilo.md)<br>
[Verificação 07 : Storyboard](analise/verificacoes/verif_storyboards.md)<br>

### 3.2 Design, Avaliação e Desenvolvimento

#### 3.2.1 Nível 1

[Verificação 01 : Planejamento da Avaliação da Análise de Tarefas](analise/verificacoes/verificacao_planejamento_analise_tarefas.md)<br>
[Verificação 02 : Planejamento da Avaliação do Storyboard](analise/verificacoes/verificacao_planejamento_da_avaliacao_do_storyboard.md)<br>
[Verificação 03 : Planejamento dos Relatos do StoryBoard e Análise de Tarefas](analise/verificacoes/verificacao_planejamento_dos_relatos)<br>

#### 3.2.2 Nível 2

[Verificação 01 : Planejamento da Avaliação do Protótipo de Papel](analise/verificacoes/verificacao_planejamento_prototipacao_papel.md)<br>
[Verificação 02 : Planejamento do Relato do Protótipo de Papel](analise/verificacoes/verificacao_planejamento_dos_relatos_do_prototipo_de_papel.md)<br>

## Referências Bibliográficas

SERRANO, Maurício; SERRANO, Milene. Requisitos - Aula 20. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.

Fagan, M. (1976) Design and Code Inspections to Reduce Errors in Software Development. IBM Systems Journal, 15, 182-211.

## Histórico de Versões

| Versão  | Data       | Descrição                                         | Autor                    | Revisor         |
|---------|------------|---------------------------------------------------|--------------------------|-----------------|
| 1.0     | 15/08/2022 | Criação da Introdução, Metodologia e Verificações | Leonardo Vitoriano       | Nícolas Mantzos |
| 1.1     | 17/08/2022 | Reescrita com maior detalhamento                  | Nícolas Georgeos Mantzos | Nicolas Mantzos |
