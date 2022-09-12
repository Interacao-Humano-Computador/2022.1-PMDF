# Protótipo de Papel

## Teste Piloto

### 1. Metodologia

O objetivo é submeter um usuário, ou ao menos um candidato a usuário, ao protótipo de papel objetivando que ele simule o fluxo pelas telas
do sistema sob o comando de um orientador.

O grupo selecionou dois integrantes, para que um fosse o orientador e outro o orientando do teste-piloto. No caso:

- Orientador: Guilherme Brito
- Orientando: Bernardo Pissuti

Segue vídeo do teste-piloto do grupo

<iframe width="560" height="315" src="https://www.youtube.com/embed/R6R91GvxjXg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Relato da Avaliação

### 1. Objetivo e escopo da avaliação

Na etapa Relato dos resultados, ultima etapa para a realização da avaliação heuristica do protótipo de papel, Temos como objetivo revisar os problemas encontrados, julgar a gravidade e recomendar correções para o design.

### 2. Metodologia

Visando facilitar o entendimento  dos problemas encontrados foi utilizado o método proposto por Nielsen e referenciado pelo livro da Simone, onde propõe descrever  violação ocorrida, o local (onde foram violados os critérios da avaliação heuristica), uma escala de severidade e a recomendação (buscando solucionar o problema).

Para a Escala de severidade temos:

|identificador| problema |descrição |
|----|-----|-----|
|1|Problema cosmético| Não precisa ser consertado com urgência |
|2|Problema pequeno| O conserto possui baixa prioridade |
|3|Problema grande| O conserto desse problema prejudica nos objetivos do usuário e deve receber alta prioridade |
|4|Problema catastrófico| O conserto desse problema deve ser feito antes do lançamento, pois impede o usuário de atingir os objetivos |

Tabela 1: Legenda Escala de severidade utilizada por Nielsen

### 3. Participantes

(Avaliador) Guilherme brito e (Usuário) Luis henrique brito, que não de se adequa ao perfil de usuário.

### 4. Dados Coletados

Cada avaliador deve inspecionar individualmente cada tela selecionada e cada um de seus
elementos, com o objetivo de identificar se as diretrizes foram respeitadas ou violadas. Cada violação
de diretriz é considerada um problema potencial de IHC

### 5. Interpretação e Análise de dados

Para a interpretação, o avaliador deve considerar os focos da análise (quais dados devem ser analisados 
sob quais perspectivas de análise) tendo em vista o método de avaliação escolhido (Barbose, Simone; p. 278), nesse caso
uma entrevista.

### 6. Problemas Encontrados

1. Visibilidade do estado do sistema: O componente de navegação não possui uma indicação para o usuário que ele está em um devido local.
   - local: se localiza na tab de navegação
   - severidade: 2 (problema pequeno), o usuário pode se perder e não saber onde ele está.
   - recomendação: destacar o local de navegação em comparação aos outros locais.
2. Reconhecimento em vez de memorização: O link para acessar não está facilmente visivel para o usuário.
   - local: se localiza na pagina de Servidores
   - severidade: 3 (problema grande), o usuário pode não encontrar o link para o acesso do salário dos servidores, impedindo de executar seu objetivo.
   - recomendação: destacar em azul (convenção) o link para o salário

### 7. Sugestões e Criticas do usuário

1. Para a tarefa de acesso ao intranet: Mostrar o popup de erro ao acessar a intranet centralizado impedindo que o usuário tente novamente sem antes perceber que errou algo.


### 8. Video da avaliação

<iframe width="560" height="315" src="https://www.youtube.com/embed/Vi7MhnIE0hE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



## Referências Bibliográficas

Barbosa, S. D. J.; Silva, B. S. da; Silveira, M. S.; Gasparini, I.; Darin, T.; Barbosa, G. D. J. (2021)
Interação Humano-Computador e Experiência do usuário. Autopublicação. ISBN: 978-65-00-19677-1.R



## Histórico de Versões

| Versão  | Data       | Descrição                            | Autor             | Revisor |
|---------|------------|--------------------------------------|-------------------|---------|
| 1.0     | 04/09/2022 | Adição do teste piloto               | Bernardo Pissutti | -       |
| 1.1     | 05/09/2022 | Criação do Relato protótipo de papel | Arthur            | Cicero  |
| 1.2     | 12/09/2022 | Adição Opiniões do usuário  | Arthur            | -  |
