# Verificação

## 1. Introdução

Segundo _Serrano_, a verificação pode ser entendida como _uma análise de modelos sem que haja direta comparação com o Universo de Informações_, sendo essa análise uma tarefa desempenhada tanto por seres humanos quanto por software, seguindo regras bem definidas e cujo objetivo principal é analisar se os artefatos estão sendo construídos corretamente.

## 2. Metodologia

As verificações utilizarão, primariamente, as seis etapas definidas pelo método de Fagan (1976) adaptadas. Sendo elas:

### 2.1 Planejamento

Alguém tem que fazer isso...

### 2.2 Visão Geral

Pois é...alguém tem que ver isso..

### 2.3 Preparação

Um conjunto de perguntas serão elicitadas e listadas a partir da avaliação do professor nas apresentações, dos monitores nos relatórios e da bibliografia, a fim de cobrir os aspectos mais variados e relevantes do artefato. Cada pergunta estará acompanhada de um identificador para referência posterior, como consta na tabela exemplificativa 1 abaixo.

| Pergunta        | Identificador   |
| --------------- | --------------- |
| _p<sub>1</sub>_ | _i<sub>1</sub>_ |
| _p<sub>2</sub>_ | _i<sub>2</sub>_ |
| _p<sub>3</sub>_ | _i<sub>3</sub>_ |
| ...             | ...             |
| _p<sub>n</sub>_ | _i<sub>n</sub>_ |

_Tabela 1: Tabela exemplificativa de itens e seus identificadores_

### 2.4 Inspeção

Os itens destacados na etapa de preparação serão inspecionados justapondo-os em uma tabela com duas colunas: _Identificador_ e _Situação_, referindo-se, respectivamente ao n-ésimo _i<sub>n</sub>_ da tabela 1
e a um dos ícones da tabela 3. No caso, "✅" qualificando o item como "Atendido" e "❌" o tornando "Não atendido", como pode ser visto na tabela 2.

| Identificador   | Situação |
| --------------- | -------- |
| _i<sub>1</sub>_ | ✅       |
| _i<sub>2</sub>_ | ✅       |
| _i<sub>3</sub>_ | ❌       |
| _i<sub>4</sub>_ | ✅       |
| ...             | ...      |
| _i<sub>n</sub>_ | ❌       |

_Tabela 2: Tabela exemplificativa de inspeção de itens (checklist)_

| Símbolo | Significado  |
| :-----: | :----------: |
|   ✅    |   Atendido   |
|   ❌    | Não atendido |

_Tabela 3: Símbolos utilizados nas checklists e seus significados_

A partir dessa resposta, um gráfico de pizza como o da figura 1, compilando a porcentagem de itens atendidos e
não atendidos, será montado para facilitar a análise dos resultados e melhorar o rastreamento dos itens
nas próximas fases.

| ![imagemGráfico](../_media/grafico_guiadeestilo.png)            |
| --------------------------------------------------------------- |
| Figura 1: Exemplo de gráfico de itens atendidos e não atendidos |

Por fim, haverá uma conclusão determinando se o artefato deve ou não ser corrigido, quais pontos devem ser priorizados em uma eventual correção etc

### 2.5 Correção

Nesta fase, um membro da equipe será alocado para realizar a correção do artefato a partir do que foi apontado na etapa de inspeção.

### 2.6 Acompanhamento

Nesta fase, um membro da equipe será alocado para acompanhar a tarefa de correção, realizando uma nova inspeção para a fiscalização dos itens que ainda não tenham sido atendidos.

## 3. Verificações

### 3.1 Análise de Requisitos

[Verificação 01 : Perfil do Usuário](analise/verificacoes/verif_perfil_de_usuario.md)<br>
[Verificação 02 : Personas](analise/verificacoes/verificacao_personas.md)<br>
[Verificação 03 : Análise de Tarefas](analise/verificacoes/)<br>
[Verificação 04 : Princípios Gerais](analise/verificacoes/verif_principios_gerais.md)<br>
[Verificação 05 : Metas de Usabilidade](analise/verificacoes/verificacao_metas.md)<br>
[Verificação 06 : Guia de Estilo](analise/verificacoes/verificacao_guia_estilo.md)<br>


### 3.2 Design, Avaliação e Desenvolvimento

#### 3.2.1 Nível 1

[Verificação 01 : Planejamento da avaliação da Análise de Tarefas](analise/verificacoes/verificacao_planejamento_analise_tarefas.md)<br>
[Verificação 02 : Planejamento da avaliação do Storyboard](analise/verificacoes/)<br>
[Verificação 03 : Planejamento dos Relatos](analise/verificacoes/)<br>
[Verificação 03 : Planejamento dos Relatos](analise/verificacoes/verif_storyboards.md)<br>

#### 3.2.2 Nível 2

[Verificação 01 : Planejamento da avaliação do Protótipo de Papel](analise/verificacoes/verificacao_planejamento_prototipacao_papel.md)<br>

## Referências Bibliográficas

SERRANO, Maurício; SERRANO, Milene. Requisitos - Aula 20. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.

Fagan, M. (1976) Design and Code Inspections to Reduce Errors in Software Development. IBM Systems Journal, 15, 182-211.

## Histórico de Versões

| Versão | Data       | Descrição                                         | Autor                    |
| ------ | ---------- | ------------------------------------------------- | ------------------------ |
| 1.0    | 15/08/2022 | Criação da Introdução, Metodologia e Verificações | Leonardo Vitoriano       |
| 1.1    | 17/08/2022 | Reescrita com maior detalhamento                  | Nícolas Georgeos Mantzos |
