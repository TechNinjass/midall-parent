## 03/04/2023 a 23/04/2023

<span id="topo">

<h1 align="center">:bookmark: Segunda Entrega - SPRINT 2</h1>

<p align="center">
    <a href="#objetivos">Objetivos da sprint</a> &nbsp |&nbsp &nbsp
    <a href="#entregas">Entregas</a> &nbsp |&nbsp &nbsp
    <a href="#burndown">Burndown</a> &nbsp |&nbsp &nbsp
    <a href="#backlogs">Backlogs</a>
</p>

Temos um desafio de autenticar o usuário através do token de segurança das nuvens, também desenvolvemos um dashboard (v1) para análise dos dados transferidos.
    
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
    
### :heavy_check_mark: RF 08: Criar dashboard para acompanhamento das execuções (ferramenta de BI)
    
📊 Escolhemos o LuckerStudio para elaborar o dashboard, devido à sua experiência em desenvolvimento de aplicativos como serviço, interface de usuário simplificada, gerenciamento de erros e alertas, habilidades em gerenciamento de dados e análise, experiência em construção de dashboards e suporte técnico e pós-implantação confiáveis.
    
1- Dentro do LookerStudio, escolhemos o metodo de conexão Microsoft SQL Server.
    
<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/1dash.jpg" /></h1>
    
2- [Neste link](https://support.google.com/looker-studio/answer/11283389#zippy=%2Cneste-artigo%2Cmostrar-a-lista-de-endere%C3%A7os-ip) conseguimos acessar o IP utilizado pelo looker studio, e este deverá ser liberado dentro da nuvem (Azure).
    
<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/2dash.jpg" /></h1>
    
3- Nas configurações de rede fazemos a liberação para duas faixas de IP, conforme apresentado abaixo.
    
<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/3dash.jpg" /></h1>
    
4- Com esses passos concluídos, podemos preencher os dados dos métodos de conexão:
    
<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/4dash.jpg" /></h1>
    
##  📉 Resultado do Dashboard v.1.0
    
- Listagem dos Arquivos Transferidos
- Filtros de Período, Tamanho e Nome do arquivo.
- Indicadores Medida (Total, Média, Arquivo mais pesado/leve)
- Indicadores de Formato (Quantidade, Tamanho Médio e Total)
    
<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/dashboardcompleto.jpg" /></h1>

### :heavy_check_mark: RNF 13: Melhorias na listagem dos arquivos (Data e Tamanho)
    
Em Construção 🏗    
    
### :heavy_check_mark: RF 14: Deletar o arquivo ao ser transferido
    
Elaboramos uma lógica que faz o arquivo ser deletado do Google Drive ao ser transferido para Azure. Razões pelas quais pode ser importante considerar a exclusão dos arquivos originais após a transferência para outra nuvem no projeto:    
    
**Economia de espaço de armazenamento:** A transferência de arquivos para outra nuvem pode consumir espaço de armazenamento na plataforma de origem. Ao excluir os arquivos originais após a transferência, você pode liberar espaço de armazenamento e otimizar o uso dos recursos disponíveis.

**Segurança dos dados:** Excluir os arquivos originais após a transferência pode ajudar a garantir a segurança dos dados. Ao remover os arquivos originais, você diminui a exposição a possíveis riscos de segurança, como acesso não autorizado ou vazamento de dados, especialmente se os arquivos contiverem informações sensíveis.

**Consistência dos dados:** Ao excluir os arquivos originais após a transferência, você evita a possibilidade de ter várias versões do mesmo arquivo, o que pode causar inconsistências nos dados e dificultar a análise e interpretação correta dos resultados.  
    
<br>
    
<span id="burndown">
    
## :chart_with_upwards_trend: Burndown

O acompanhamento de atividades, de responsabilidade do Scrum Master, se encontra na imagem adiante, que contém o gráfico Burndown gerado pela equipe (onde o eixo X são os dias trabalhados na sprint e os valores do eixo Y representam as entregas e esforços realizados com o passar do tempo), incluindo as quantidade de atividades desenvolvidas.
    
- Linha Ideal (Vermelho)
- Linha Real (Azul)
    
<div align="center">
    
![Burndown Chart](https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/burndown-sprint2-2304.png)
</div>

- Gráfico atualizado no dia 23/04/2023
  
<br>
  
<span id="backlogs">

## :dart: Backlogs, Épicos & User Stories

<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/Backlogs-3.png" /></h1>

<br>
  
→ [Voltar ao topo](#topo)
