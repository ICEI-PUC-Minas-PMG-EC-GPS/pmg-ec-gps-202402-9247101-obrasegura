# Iniciação

> A fase de iniciação, em gerência de projetos, é o estágio que estabelece as bases para o sucesso do empreendimento.
> Durante essa etapa, os objetivos definidos, identificando-se suas metas, escopo, partes interessadas (*stakeholders*) e restrições.
> É o momento em que a viabilidade do projeto é avaliada, analisando-se recursos necessários, riscos potenciais e benefícios esperados.
> Nesta etapa é elaborado o Termo de Abertura do Projeto (TAP).
> Essa fase serve como um alicerce estratégico, proporcionando uma compreensão abrangente do que o projeto busca alcançar e delineando as diretrizes que orientarão as etapas subsequentes.
> O sucesso na fase de iniciação contribui significativamente para a eficácia do gerenciamento de projetos como um todo.

# Estrutura do Documento

- [Fase de Iniciação](#iniciação)
- [Introdução](#introdução)
  - [Problema](#problema)
  - [Objetivos](#objetivos)
  - [Justificativa](#justificativa)
  - [Critérios de Sucessos](#critérios-de-sucesso)
- [Partes Interessadas](#partes-interessadas)
  - [Identificação das Partes Interessadas](#identificação-das-partes-interessadas)
  - [Avaliação das Partes Interessadas](#avaliação-das-partes-interessadas)
- [Termo de Abertura do Projeto](#termo-de-abertura-do-projeto)
  - [Estimativa de Custo](#estimativa-de-custo)
  - [Estimativa de Prazo](#estimativa-de-prazo)
  - [Escopo Preliminar e Premissas](#escopo-preliminar-e-premissas)
    - [Requisitos Funcionais](#requisitos-funcionais)
    - [Requisitos Não Funcionais](#requisitos-não-funcionais)
    - [Restrições](#restrições)
    - [Contra-Escopo](#contra-escopo)
    - [Condições para início do Projeto](#condições-para-início-do-projeto)
  - [Marcos Agendados e Entregas](#marcos-agendados-e-entregas)
- [Metodologia](#metodologia)
  - [Divisão de Papéis](#divisão-de-papéis)
  - [Ferramentas](#ferramentas)

# Introdução

```diff
+ Tarefa 01:
+ Tema do projeto e lista de Stakeholders
```

## Problema

> A segurança no ambiente de trabalho em obras de construção civil é uma questão crítica, onde a ausência de Equipamentos de Proteção Individual (EPIs) pode levar a acidentes graves, resultando em lesões ou até mesmo mortes. A supervisão manual do uso de EPIs é um processo falho e ineficiente, propenso a erros humanos e limitações de alcance.  
Além disso, a falta de um sistema automatizado dificulta a monitorização em tempo real, comprometendo a capacidade de resposta rápida e proativa para evitar incidentes. Diante desse contexto, existe a necessidade de desenvolver uma solução que permita a detecção automática da presença ou ausência de EPIs, garantindo a conformidade com as normas de segurança e a proteção dos trabalhadores.

## Objetivos

> **Objetivo Geral:**  
Detectar em tempo real Equipamentos de Proteção Individual (EPIs) em obras de construção civil.

> **Objetivos Específicos:**
> - Detecção de Objetos em Tempo Real: Utilização de modelos de machine learning para a identificação de EPIs em imagens e vídeos capturados no ambiente de trabalho;
> - Integração com Serviços Cloud: Implementação dos serviços Cloud, como Cloud Rekognition para detecção de objetos e Cloud S3 para armazenamento de imagens e vídeos;
> - Alertas Automáticos: Desenvolvimento de um sistema de notificação que alerta os supervisores de segurança quando EPIs obrigatórios não são detectados;
> - Dashboard de Monitoramento: Criação de uma interface que permite o acompanhamento em tempo real do uso de EPIs na obra, com relatórios e estatísticas;
> - Treinamento e Aperfeiçoamento do Modelo: Coleta e rotulação de dados para treinar o modelo de detecção, com ajustes contínuos para melhorar a precisão.

<!-- 
> **Link Útil**:
> - [Objetivo geral e objetivo específico: como fazer e quais verbos utilizar](https://blog.mettzer.com/diferenca-entre-objetivo-geral-e-objetivo-especifico/) 
-->

## Justificativa


> A segurança no ambiente de trabalho é uma prioridade inegociável, especialmente em obras de construção civil, onde os riscos de acidentes são elevados. A presença e o uso adequado de Equipamentos de Proteção Individual (EPIs) desempenham um papel crucial na mitigação desses riscos, garantindo a integridade física dos trabalhadores e a conformidade com as normas de segurança. Contudo, o processo de supervisão manual da utilização desses equipamentos tem se mostrado falho e ineficiente. Esse método não apenas está sujeito a erros humanos, mas também é limitado em termos de alcance e capacidade de monitoramento contínuo.
> Neste contexto, a adoção de uma solução automatizada para a detecção de EPIs se torna essencial. Utilizando tecnologias avançadas de machine learning e serviços em nuvem da Cloud, é possível desenvolver um sistema robusto que oferece monitoramento em tempo real, notificando instantaneamente qualquer ausência de EPIs obrigatórios. Essa abordagem não só aumenta a eficiência do processo de supervisão, mas também reduz drasticamente a probabilidade de incidentes, promovendo um ambiente de trabalho mais seguro.

> Além dos benefícios imediatos de redução de acidentes e conformidade regulamentar, a implementação de tal sistema contribui para a otimização dos recursos da empresa. Ao automatizar tarefas repetitivas e críticas, como a verificação do uso de EPIs, os supervisores de segurança podem redirecionar seu foco para outras áreas de risco, melhorando a eficiência operacional. Adicionalmente, a geração de dashboards e relatórios detalhados oferece uma visibilidade completa e contínua sobre o uso de EPIs, fortalecendo a cultura de responsabilidade e transparência na obra.
> Outro ponto relevante é o impacto positivo que essa iniciativa pode ter na reputação da empresa. Ao demonstrar um compromisso sólido com a segurança dos trabalhadores, a organização não apenas se protege de possíveis sanções legais, mas também ganha a confiança de clientes, investidores e da comunidade em geral. Assim, o desenvolvimento deste projeto não apenas atende a uma necessidade crítica de segurança, mas também posiciona a empresa como uma líder em inovação e responsabilidade no setor de construção civil.

> - Redução de Acidentes: A detecção em tempo real de EPIs permitirá uma resposta imediata à ausência de equipamentos de segurança, reduzindo significativamente o risco de acidentes.

> - Conformidade Regulamentar: O sistema ajudará as empresas a se manterem em conformidade com as exigências legais e regulamentares, evitando multas e penalidades associadas à falta de EPIs.

> - Eficiência Operacional: Automatizar o processo de monitoramento libera os supervisores de segurança para focarem em outras atividades críticas, aumentando a eficiência operacional e reduzindo custos com inspeções manuais.

> - Transparência e Responsabilidade: O uso de dashboards e relatórios fornecerá visibilidade contínua sobre a conformidade com os EPIs, promovendo a responsabilidade entre os trabalhadores e a administração.

> - Reputação e Confiança: Um ambiente de trabalho mais seguro melhora a reputação da empresa, aumentando a confiança de clientes, investidores e colaboradores.

## Critérios de Sucesso

> Para garantir que o projeto alcance os objetivos estabelecidos e traga os benefícios esperados, serão adotados os seguintes critérios de sucesso:

> - Acurácia da Detecção: O modelo de machine learning implementado deve demonstrar uma elevada acurácia na identificação de EPIs, mesmo em condições adversas, como variações de iluminação, ângulos variados e diferentes tipos de equipamentos. A meta é atingir uma taxa de acurácia mínima de 95%, garantindo que o sistema seja confiável e eficaz em diferentes cenários operacionais.

> - Tempo de Resposta: A capacidade de resposta em tempo real é um dos pilares do projeto. O sistema deve ser capaz de detectar e notificar a ausência de EPIs obrigatórios em menos de 5 segundos, permitindo que ações corretivas sejam tomadas de forma imediata, antes que qualquer incidente ocorra.

> - Conformidade e Auditoria: A solução deve facilitar a geração de relatórios detalhados que comprovem a conformidade contínua com as normas de segurança estabelecidas. Esses relatórios serão essenciais para auditorias internas e externas, demonstrando o comprometimento da empresa com a segurança dos trabalhadores.

> - Satisfação dos Stakeholders: A aceitação e satisfação dos principais stakeholders, incluindo supervisores de segurança, trabalhadores e administradores, são fundamentais para o sucesso do projeto. Para isso, serão realizadas pesquisas de feedback com o objetivo de atingir uma taxa de satisfação mínima de 90%, garantindo que o sistema atenda às expectativas e necessidades de todos os envolvidos.

> - Entrega Dentro do Prazo e Orçamento: A gestão eficiente do projeto é crucial para o seu sucesso. O desenvolvimento e implementação da solução devem ser concluídos dentro do cronograma estabelecido e sem ultrapassar o orçamento aprovado, demonstrando a capacidade da equipe de gerenciamento em utilizar os recursos de forma eficaz.

> - Aprimoramento Contínuo: O sistema deve ser projetado para se adaptar e melhorar continuamente, incorporando novos dados e feedback ao longo do tempo. Esse processo de aprendizado contínuo garantirá que a solução permaneça eficaz e relevante à medida que surgem novos desafios e requisitos no ambiente de trabalho. requisitos e expectativas das partes interessadas, bem como a gestão eficaz de riscos, são considerados aspectos importantes para determinar o sucesso de um projeto.

# Partes Interessadas

> Relacione as partes interessadas no seu projeto.
> Você deve descrever as partes interessadas e indicar qual o nível de influência em relação ao projeto.
> Indique as principais pessoas (clientes, fornecedores, etc), indicando possíveis expectativas, nível de influência e possível importância para o sucesso do projeto.

> Você pode utilizar como referência o seguinte documento:
> [Registro de Partes Interessadas](artefatos/registro-partes-interessadas.xlsx)

## Identificação das Partes Interessadas

| Nome            | Posição / Cargo      | Papel Projeto                               | E-mail                     | Telefone        |
|-----------------|----------------------|---------------------------------------------|----------------------------|-----------------|
| Wagner Moura    | Analista de testes   | Validação e Qualidade                       | moura.wagner@testes.dev    | (29) 4229-8621  |
| Julia Rocha     | Desenvolvedora       | Interface gráfica                           | juliarocha@mail.google     | (15) 4567-4563  |
| Marcio Costa    | Desenvolvedor        | Detecção de EPI                             | marciocosta@dev.ai         | (86) 5639-2690  |
| Ricardo Almeida | Parceiro             | Patrocinador do projeto                     | recardo@almeida.perceiros  | (43) 5595-1150  |
| Samira Santos   | Gerencia de produção | Administração do hardware usado na produção | samira@santos-producoes.br | (56) 97415-4102 |
| Construtoras    | Usuários             | Usuários do sistema                         | --                         | --              |

## Avaliação das Partes Interessadas

| Nome            | Expectativa no Projeto                           | Influência | Importância / Poder | Apoio    | Observações |
|-----------------|--------------------------------------------------|------------|---------------------|----------|-------------|
| Wagner Moura    | Garantia de estabilidade e qualidade do projeto  | Alta       | Alta                | Positivo |             |
| Julia Rocha     | Melhora da experiencia do cliente                | Baixa      | Média               | Neutro   |             |
| Marcio Costa    | Aumento na precisão da detecção                  | Média      | Alta                | Positivo |             |
| Ricardo Almeida | Maior orçamento para o desenvolvimento           | Alta       | Médio               | Neutro   |             |
| Samira Santos   | Melhora na produção e monitoramento de qualidade | Baixa      | Média               | Neutro   |             |
| Construtoras    | --                                               | Baixa      | Baixo               | Neutro   |             |

```diff
+ Tarefa 01
+ Fim da seção a ser atualizada.
```


-----
```diff
+ Tarefa 02
+ Termo de Abertura do Projeto
```

# Termo de Abertura do Projeto

O projeto tem como objetivo desenvolver uma solução automatizada para a detecção de Equipamentos de Proteção Individual (EPIs) em ambientes de construção civil, utilizando a plataforma AWS e suas ferramentas de inteligência artificial. A segurança no ambiente de trabalho é uma prioridade em obras de construção, e a ausência de EPIs pode resultar em acidentes graves. Com o uso de tecnologias avançadas, como visão computacional e machine learning, este projeto visa identificar em tempo real a presença ou ausência dos EPIs obrigatórios em trabalhadores, proporcionando um sistema de monitoramento eficiente e proativo.

Ao longo do semestre, o foco será na criação de um modelo capaz de analisar imagens capturadas no local da obra e detectar automaticamente se os trabalhadores estão utilizando EPIs, como capacetes, luvas e demais itens de segurança. A implementação dessa solução contribuirá significativamente para a prevenção de acidentes e para a conformidade com as normas de segurança.

## Possíveis Funcionalidades e Recursos Necessários

- **Detecção de Objetos em Tempo Real:** Utilização de modelos de machine learning para a identificação de EPIs em imagens e vídeos capturados no ambiente de trabalho.
  
- **Integração com Serviços em cloud :** Implementação dos serviços em plataforma nuvem, como AWS Rekognition para detecção de objetos e AWS S3 para armazenamento de imagens e vídeos.
  
- **Alertas Automáticos:** Desenvolvimento de um sistema de notificação que alerta os supervisores de segurança quando EPIs obrigatórios não são detectados.
  
- **Dashboard de Monitoramento:** Criação de uma interface que permite o acompanhamento em tempo real do uso de EPIs na obra, com relatórios e estatísticas.
  
- **Treinamento e Aperfeiçoamento do Modelo:** Coleta e rotulação de dados para treinar o modelo de detecção, com ajustes contínuos para melhorar a precisão.

Recursos necessários incluem a utilização de câmeras de alta definição para captura de imagens, acesso à plataforma AWS, além de conhecimentos em machine learning, visão computacional, e desenvolvimento de software em cloud.

## Estimativa de Custo

A avaliação da viabilidade econômica busca determinar a sustentabilidade financeira e o retorno sobre o investimento do empreendimento.  
Este processo envolve a análise dos custos associados ao projeto, incluindo investimentos iniciais, despesas operacionais e potenciais custos de manutenção.  
Simultaneamente, são examinados os benefícios esperados, como receitas, economias de custos e ganhos tangíveis e intangíveis.  
A elaboração de projeções financeiras realistas e a aplicação de métricas como o Valor Presente Líquido (VPL) e a Taxa Interna de Retorno (TIR) contribuem para uma avaliação abrangente da viabilidade econômica do projeto.  
Este processo permite que os gestores de projeto e as partes interessadas tomem decisões informadas sobre a continuidade, ajustes ou mesmo a interrupção do projeto, garantindo uma alocação eficiente de recursos e maximizando os benefícios econômicos esperados.

### Tabela de Estimativa de Custo

| Item de Custo            | Descrição                                                      | Qtd. horas | Valor / hora | Valor total       |
|--------------------------|----------------------------------------------------------------|------------|--------------|-------------------|
| Recursos Humanos         | Equipe de desenvolvedores e especialistas em ML/AI             | 1200       | R$ 150,00    | R$ 180.000,00     |
| Hardware                 | Câmeras e computadores de processamento                        | -          | -            | R$ 50.000,00      |
| Serviços de Rede         | Configuração de rede para coleta de dados                      | 200        | R$ 50,00     | R$ 10.000,00      |
| Hospedagem e Nuvem       | Serviços Cloud (Rekognition, S3, EC2, etc.)                    | 300        | R$ 100,00    | R$ 30.000,00      |
| Software de terceiros    | Licenças para ferramentas de análise e detecção de objetos     | 150        | R$ 100,00    | R$ 15.000,00      |
| Serviços e treinamento   | Treinamento para equipe e suporte ao usuário final             | 400        | R$ 50,00     | R$ 20.000,00      |
| Manutenção do Sistema    | Atualizações e ajustes no sistema pós-implementação            | 300        | R$ 120,00    | R$ 36.000,00      |
| Marketing e Divulgação   | Campanhas de divulgação do sistema e seus benefícios           | 100        | R$ 80,00     | R$ 8.000,00       |
| Consultoria de Segurança | Consultoria para garantir conformidade com normas de segurança | 100        | R$ 200,00    | R$ 20.000,00      |
| Testes e Validação       | Testes de campo para validação da solução em ambientes reais   | 250        | R$ 80,00     | R$ 20.000,00      |
| **Total Geral**          |                                                                | -          | -            | **R$ 389.000,00** |


## Estimativa de Prazo

A estimativa de prazo orienta tanto o cliente quanto a equipe de desenvolvimento do projeto em termos do tempo necessário para a conclusão do projeto como um todo.  
Esta estimativa possibilita a criação de um cronograma realista e viável, permitindo o planejamento adequado das fases do projeto, alocação de recursos de maneira eficiente e antecipação de eventuais desafios.  
Uma estimativa precisa orienta a execução do projeto, contribui para a gestão de expectativas e para o estabelecimento de metas alcançáveis.

- **Prazo previsto (em horas):** 4000 horas  
- **Data de início:** 08/08/2024  
- **Data de término:** 21/12/2024  

## Escopo Preliminar e Premissas

A seguir, os requisitos foram classificados em dois grupos: Requisitos Funcionais (RF) e Requisitos Não Funcionais (RNF). Cada requisito corresponde a uma característica específica da solução.

#### Requisitos Funcionais (RF)

1. **RF01 - Detecção de EPIs em Tempo Real:** O sistema deve identificar a presença ou ausência de EPIs, como capacetes e luvas, em trabalhadores a partir de imagens capturadas no ambiente de construção.
2. **RF02 - Notificações Automáticas:** O sistema deve enviar alertas automáticos para os supervisores de segurança quando um EPI obrigatório não for detectado.
3. **RF03 - Integração com AWS Rekognition:** A solução deve integrar-se ao AWS Rekognition para realizar a detecção de objetos em imagens e vídeos.
4. **RF04 - Armazenamento de Imagens e Vídeos:** O sistema deve utilizar o AWS S3 para armazenar de forma segura todas as imagens e vídeos capturados.
5. **RF05 - Dashboard de Monitoramento:** Deve ser desenvolvido um painel de controle que permita o acompanhamento em tempo real do uso de EPIs na obra, com relatórios e estatísticas.

### Requisitos Funcionais

A tabela a seguir apresenta os requisitos funcionais do projeto.

| ID     | Descrição do Requisito                            | Prioridade |
|--------|---------------------------------------------------|------------|
| RF-001 | Acesso ao feed das câmeras com os overlays         | ALTA       | 
| RF-002 | Detectar a presença de EPI                        | ALTA       | 
| RF-003 | Verificar se uma pessoa foi detectada sem EPI     | ALTA       |
| RF-004 | Salvar imagens de momentos de violação            | ALTA       |
| RF-005 | Marcar a área e momento da violação               | MÉDIA      |
| RF-006 | Salvar momento do vídeo no momento da violação    | MÉDIA      |
| RF-007 | Interface web para acesso em qualquer dispositivo | ALTA       |
| RF-008 | Permitir que o usuário cadastre                   | ALTA       |
| RF-009 | Envio de relatório diário                         | MÉDIA      |
| RF-010 | Detectar movimento                                | MÉDIA      |

### Requisitos Não Funcionais

A tabela a seguir apresenta os requisitos não funcionais do projeto.

| ID      | Descrição do Requisito                                            | Prioridade |
|---------|-------------------------------------------------------------------|------------|
| RNF-001 | O sistema deve ser responsivo para rodar em um dispositivo móvel  | MÉDIA      | 
| RNF-002 | Deve processar requisições do usuário em no máximo 3 segundos     | MÉDIA      | 
| RNF-003 | Funcionar com vários tipos de câmeras                             | BAIXA      | 
| RNF-004 | Enviar notificação em caso de violação                            | MÉDIA      | 
| RNF-005 | Customização de requisitos                                        | BAIXA      | 

### Restrições

A tabela a seguir apresenta as restrições do projeto.

| ID     | Descrição da Restrição                      | Prioridade |
|--------|---------------------------------------------|------------|
| RE-001 | Permitir que o usuário cadastre             | ALTA       | 
| RE-002 | Interface para acesso ao conteúdo           | ALTA       |
| RE-003 | Verificar se uma pessoa foi detectada sem EPI | ALTA       |
| RE-004 | Salvar imagens de momentos de violação      | MÉDIA      |
| RE-005 | Detectar a presença de EPI                  | MÉDIA      |

### Contra-Escopo

A tabela a seguir apresenta as funcionalidades que não estão incluídas no escopo do projeto.

| ID     | Descrição do Contra-Escopo                                                  | 
|--------|-----------------------------------------------------------------------------|
| CE-001 | Treinamento de modelo de linguagem natural (LLM).                           |
| CE-002 | Pesquisa de viabilidade do mercado.                                         |
| CE-003 | Desenvolvimento de hardware proprietário para captura de imagens.           |
| CE-004 | Monitoramento de condições ambientais, como temperatura e umidade.          |
| CE-005 | Suporte a plataformas de nuvem que não sejam AWS.                           |
| CE-006 | Implementação de funcionalidades de gestão de projetos dentro do sistema.   |
| CE-007 | Desenvolvimento de aplicativos móveis nativos para plataformas específicas. |

### Condições para Início do Projeto

A tabela a seguir apresenta as condições que devem ser atendidas para o início do projeto.

| ID     | Descrição de Condições para Início do Projeto                        | 
|--------|----------------------------------------------------------------------|
| CI-001 | Assinatura de contrato de prestação de serviços.                     |
| CI-002 | Apresentação de garantias definidas no contrato.                     |
| CI-003 | Disponibilidade de acesso aos recursos e serviços AWS necessários.   |
| CI-004 | Aquisição e configuração das câmeras para a segurança nas obras.     |
| CI-005 | Treinamento inicial da equipe de segurança para uso do sistema.      |

## Marcos Agendados e Entregas

A tabela a seguir apresenta os marcos e entregas previstas para o projeto.

| ID  | Marco do Projeto                                                          | 
|-----|---------------------------------------------------------------------------|
| M-001 | Liberação do sistema para cadastro de informações e configuração inicial. |
| M-002 | Permissão para uso do sistema por usuários focais.                        |
| M-003 | Conclusão da integração com câmeras para a segurança.                     |
| M-004 | Desenvolvimento e integração do painel de monitoramento em tempo real.    |
| M-005 | Testes de desempenho e conformidade.                                      |
| M-006 | Entrega final da solução e início do treinamento do usuário final.        |
| M-007 | Auditoria de conformidade com segurança após 3 meses de uso.              |
| M-008 | Lançamento da versão 2.0 com melhorias baseadas no feedback do usuário.   |


```diff
+ Tarefa 02
+ Fim da seção a ser atualizada.
```

-----
```diff
+ Tarefa 03:
+ Metodologia do Projeto
```

# Metodologia

......  COLOQUE AQUI O SEU TEXTO ......

> Nesta parte do documento, você deve apresentar a metodologia adotada pelo grupo, descrevendo o processo de trabalho baseado nas metodologias ágeis, a divisão de papéis e tarefas e as ferramentas empregadas.
>
> Coloque detalhes sobre o processo utilizado e a implementação do Framework Scrum seguido pelo grupo.
> O grupo deverá gerenciar as tarefas utilizando o GitHub Project para acompanhar o andamento do projeto, a execução das tarefas e o status de desenvolvimento da solução.
>
> **Links Úteis**:
> - [Github Project](https://docs.github.com/en/issues/planning-and-tracking-with-projects/creating-projects/creating-a-project)
> - [O que é o GitHub Projects? | Guia de Iniciantes](https://www.youtube.com/watch?v=vxYTpsFKdiQ&ab_channel=JulioArruda)
> - [Introduction to GitHub Project Boards](https://www.youtube.com/watch?v=idZyqNIrt84&list=PLiO7XHcmTslc5hGrbnnmHIb0SeJLTpOEu&ab_channel=MickeyGousset)
> - [11 Passos Essenciais para Implantar Scrum no seu Projeto](https://mindmaster.com.br/scrum-11-passos/)
> - [Scrum em 9 minutos](https://www.youtube.com/watch?v=XfvQWnRgxG0)

## Divisão de Papéis
<!-- 
......  COLOQUE AQUI O SEU TEXTO ......

> Apresente a divisão de papéis e tarefas entre os membros do grupo.
> Indique as responsabilidades de cada membro do grupo no projeto. 
-->
#### A divisão de papéis e tarefas entre os membros do grupo foi realizada da seguinte forma:

- Product Owner: Responsável por definir as prioridades e garantir que a equipe esteja focada nos objetivos do projeto.
- Scrum Master: Facilitador do processo Scrum, garantindo que a equipe siga as práticas ágeis e removendo impedimentos.
- Desenvolvedores: Responsáveis pela implementação das funcionalidades do projeto.
- Designers: Responsáveis pela criação dos protótipos e interfaces do usuário.
- Testers: Responsáveis por garantir a qualidade do software através de testes contínuos.

## Ferramentas

<!--
......  COLOQUE AQUI O SEU TEXTO - SIGA O EXEMPLO DA TABELA ABAIXO  ......

> Liste as ferramentas empregadas no desenvolvimento do projeto, justificando a escolha delas, sempre que possível.
> Todas as ferramentas utilizadas devem ser listadas.
> Qualquer tipo de ferramenta que for utilizada para construção de um artefato deve ser identificada, uma vez que podem ser necessárias alterações.
> A necessidade de uso de licenças e possíveis custos relacionados devem ser indicados. 
-->

| Ambiente              | Plataforma         | Link de Acesso             | Justificativa                                                  |
|-----------------------|--------------------|----------------------------|----------------------------------------------------------------|
| Quadro Kanban         | Github             | [Quadro do projeto](https://github.com/orgs/ICEI-PUC-Minas-PMG-EC-GPS/projects/32) | Centralização e organização do projeto no próprio repositório. |
| Repositório de código | GitHub             | [Repositório no github](https://github.com/orgs/ICEI-PUC-Minas-PMG-EC-GPS/teams/g9-obrasegura) | Padronização do projeto em uma única plataforma. |
| Protótipo Interativo  | MavelApp ou Figma  | https://figma.com/XXXXXXX | Projetar e refinar produtos com sua equipe, em um único arquivo de design compartilhado. |
| Documentos Textuais   | LibreOffice Writer | [Aplicativo](https://www.libreoffice.org/download/download-libreoffice/) | Ferramenta gratuita para criação de documentos textuais. |
| Planilhas e Gráficos  | Google Planilhas   | [Google Sheets](https://docs.google.com/) | Ferramenta online gratuita para criação e compartilhamento de planilhas e gráficos. |
| EAP / WBS | | | |
| Cronograma do Projeto | | | |
| Matriz RACI | | | |

```diff
+ Tarefa 03:
+ Fim da seção a ser atualizada.
```

----
