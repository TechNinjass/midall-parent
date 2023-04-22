## 03/04/2023 a 23/04/2023

<span id="topo">

<h1 align="center">:bookmark: Segunda Entrega - SPRINT 2</h1>

<p align="center">
    <a href="#objetivos">Objetivos da sprint</a> &nbsp |&nbsp &nbsp
    <a href="#entregas">Entregas</a> &nbsp |&nbsp &nbsp
    <a href="#burndown">Burndown</a> &nbsp |&nbsp &nbsp
    <a href="#backlogs">Backlogs</a>
</p>

Temos um desafio de automatizar a jornada dos arquivos armazenados na nuvem "A", realizando uma transferência para nuvem "B".

<span id="objetivos">
    
## :dart: Objetivos da Sprint
Os requisitos (tanto do cliente como da instituição de ensino) abrangidos para primeira sprint são:
- **RF 05:** Criação da tela para configuração da conta de acesso a API (Drive e Azure)
- **RF 08:** Criar dashboard para acompanhamento das execuções (ferramenta de BI)
- **RF 14:** Deletar o arquivo ao ser transferido
- **RNF 11:** Testes (Requisito Fatec)
- **RNF 13:** Melhorias na listagem dos arquivos (Data e Tamanho)
    
<br>
 
**:link: Clique no link abaixo para visualizar o *Kanban* de atividades da equipe:** 
> [Kanban Projects GitHub](https://github.com/orgs/TechNinjass/projects/2)
  
<br>
    
<span id="entregas">
  
## :heavy_check_mark: Entregas
 
### :heavy_check_mark: RF 05: Criação da tela para configuração da conta de acesso a API (Drive e Azure)

Fizemos a tela de autenticação de acesso com token entre as nuvens, essa tela foi importante nesse projeto por várias razões:

**Segurança:** A autenticação com token é uma forma de garantir que somente usuários autorizados possam acessar a aplicação e configurar os parâmetros necessários para o serviço de download. Isso ajuda a proteger a aplicação contra acessos não autorizados e garante que apenas os usuários com as devidas permissões possam utilizar a funcionalidade.

**Privacidade:** Ao lidar com arquivos de vídeos armazenados em uma plataforma de vídeos, é possível que esses arquivos contenham informações sensíveis ou confidenciais. A autenticação com token ajuda a garantir que apenas usuários autorizados possam acessar e baixar esses arquivos, mantendo a privacidade dessas informações.

**Rastreabilidade:** A utilização de tokens de autenticação permite rastrear e auditar as ações dos usuários na aplicação. Isso pode ser útil para fins de monitoramento, análise de resultados e identificação de possíveis erros ou atividades suspeitas.

**Integração segura com serviços externos:** A integração com a plataforma de vídeos e o serviço de cloud para transferência de arquivos requer autenticação segura para garantir a integridade e a confidencialidade dos dados. A utilização de tokens de autenticação ajuda a estabelecer essa comunicação de forma segura, protegendo os dados durante a transferência.
    
<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/tela%20do%20token%20de%20acesso.png" /></h1>
    
<br>
    
<span id="burndown">
    
## :chart_with_upwards_trend: Burndown

Em prol de um melhor aproveitamento das habilidades de cada integrante, o time foi separado em duas frentes: frontend e backend, onde, na primeira sprint, o time de frontend ficou responsável pela confecção do protótipo, projeto frontend e integração de funcionalidades enquanto o time de backend ficou responsável pela criação dos serviços necessários e identificação dos metadados que serão armazenados no dashboard futuramente.

- O acompanhamento de atividades, de responsabilidade do Scrum Master, se encontra na imagem adiante, que contém o gráfico Burndown gerado pela equipe (onde o eixo X são os dias trabalhados na sprint e os valores do eixo Y representam as entregas e esforços realizados com o passar do tempo), incluindo as atividades desenvolvidas e seus responsáveis.
    
<div align="center">
    
![Burndown Chart](https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/burndown-sprint2-1704.png)
</div>

- Gráfico atualizado no dia 17/04/2023
  
<br>
  
<span id="backlogs">

## :dart: Backlogs, Épicos & User Stories

<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/Backlogs-3.png" /></h1>

<br>
  
→ [Voltar ao topo](#topo)
