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

> O Termo de Abertura do Projeto (TAP) representa o ponto de partida oficial para o empreendimento.
> Ele sintetiza de maneira clara e concisa os objetivos, escopo, partes interessadas envolvidas, entregas esperadas, cronograma preliminar e recursos necessários para a execução bem-sucedida do projeto.
> O TAP funciona como um contrato inicial entre a equipe do projeto e as partes interessadas, estabelecendo as bases para uma compreensão compartilhada dos propósitos e limites do projeto.
> Ao delinear esses elementos de forma detalhada, o Termo de Abertura do Projeto (TAP) fornece uma direção sólida para orientar as atividades subsequentes, facilitando a gestão eficaz do projeto desde o início até o encerramento.
> Essa documentação garante a clareza, alinhamento e comprometimento de todos os envolvidos, contribuindo assim para o sucesso do projeto.

> Você pode utilizar como referência o seguinte documento:
> [Termo de Abertura do Projeto](artefatos/termo-abertura-projeto.docx)

## Estimativa de Custo

A avaliação da viabilidade econômica busca determinar a sustentabilidade financeira e o retorno sobre o investimento do empreendimento.  
Este processo envolve a análise dos custos associados ao projeto, incluindo investimentos iniciais, despesas operacionais e potenciais custos de manutenção.  
Simultaneamente, são examinados os benefícios esperados, como receitas, economias de custos e ganhos tangíveis e intangíveis.  
A elaboração de projeções financeiras realistas e a aplicação de métricas como o Valor Presente Líquido (VPL) e a Taxa Interna de Retorno (TIR) contribuem para uma avaliação abrangente da viabilidade econômica do projeto.  
Este processo permite que os gestores de projeto e as partes interessadas tomem decisões informadas sobre a continuidade, ajustes ou mesmo a interrupção do projeto, garantindo uma alocação eficiente de recursos e maximizando os benefícios econômicos esperados.

### Tabela de Estimativa de Custo

| Item de Custo           | Descrição                                                 | Qtd. horas | Valor / hora | Valor total     |
|-------------------------|-----------------------------------------------------------|------------|--------------|-----------------|
| Recursos Humanos        | Equipe de desenvolvedores e especialistas em ML/AI         | 1200       | R$ 150,00    | R$ 180.000,00   |
| Hardware                | Câmeras e computadores de processamento  | -          | -            | R$ 50.000,00    |
| Serviços de Rede        | Configuração de rede para coleta de dados                  | 200        | R$ 50,00     | R$ 10.000,00    |
| Hospedagem e Nuvem      | Serviços Cloud (Rekognition, S3, EC2, etc.)                  | 300        | R$ 100,00    | R$ 30.000,00    |
| Software de terceiros   | Licenças para ferramentas de análise e detecção de objetos | 150        | R$ 100,00    | R$ 15.000,00    |
| Serviços e treinamento  | Treinamento para equipe e suporte ao usuário final         | 400        | R$ 50,00     | R$ 20.000,00    |
| Manutenção do Sistema   | Atualizações e ajustes no sistema pós-implementação        | 300        | R$ 120,00    | R$ 36.000,00    |
| Marketing e Divulgação  | Campanhas de divulgação do sistema e seus benefícios       | 100        | R$ 80,00     | R$ 8.000,00     |
| Consultoria de Segurança| Consultoria para garantir conformidade com normas de segurança | 100   | R$ 200,00    | R$ 20.000,00    |
| Testes e Validação      | Testes de campo para validação da solução em ambientes reais| 250       | R$ 80,00     | R$ 20.000,00    |
| **Total Geral**         |                                                           | -          | -            | **R$ 389.000,00** |


## Estimativa de Prazo

A estimativa de prazo orienta tanto o cliente quanto a equipe de desenvolvimento do projeto em termos do tempo necessário para a conclusão do projeto como um todo.  
Esta estimativa possibilita a criação de um cronograma realista e viável, permitindo o planejamento adequado das fases do projeto, alocação de recursos de maneira eficiente e antecipação de eventuais desafios.  
Uma estimativa precisa orienta a execução do projeto, contribui para a gestão de expectativas e para o estabelecimento de metas alcançáveis.

- **Prazo previsto (em horas):** 4000 horas  
- **Data de início:** 08/08/2024  
- **Data de término:** 21/12/2024  

## Escopo Preliminar e Premissas

Os requisitos preliminares fornecem uma visão inicial do escopo, funcionalidades-chave e as expectativas a serem atendidas.

## Declaração de Escopo

> Você pode utilizar como referência o seguinte documento:
- [Declaração de Escopo](artefatos/declaracao-escopo.docx)

> Enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:
>
> - [Requisitos Funcionais (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
    >   correspondem a uma funcionalidade que deve estar presente na
    >   plataforma (ex: cadastro de usuário).
>
> - [Requisitos Não Funcionais (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
    >   correspondem a uma característica técnica, seja de usabilidade,
    >   desempenho, confiabilidade, segurança ou outro (ex: suporte a
    >   dispositivos iOS e Android).
>
> Lembre-se que cada requisito deve corresponder à uma e somente uma
> característica alvo da sua solução. Além disso, certifique-se de que
> todos os aspectos capturados nas Histórias de Usuário foram cobertos.
>
> **Links Úteis**:
>
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)


### Requisitos Funcionais

......  ATUALIZE OS REQUISITOS FUNCIONAIS DO SISTEMA (MÍNIMO 10) ......

A tabela a seguir apresenta os requisitos funcionais do projeto.

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|-------|
|RF-001| Permitir que o usuário cadastre tarefas | ALTA | 
|RF-002| Emitir um relatório de tarefas no mês   | MÉDIA |

### Requisitos Não Funcionais

......  ATUALIZE OS REQUISITOS NÃO FUNCIONAIS DO SISTEMA (MÍNIMO 5) ......

A tabela a seguir apresenta os requisitos não funcionais do projeto.

|ID     | Descrição do Requisito                                            |Prioridade |
|-------|-------------------------------------------------------------------|-----------|
|RNF-001| O sistema deve ser responsivo para rodar em um dispositivos móvel | MÉDIA     | 
|RNF-002| Deve processar requisições do usuário em no máximo 3s             | BAIXA     | 


### Restrições

......  ATUALIZE AS RESTRIÇÕES DO SISTEMA (MÍNIMO 5) ......

A tabela a seguir apresenta as restrições do projeto.

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|-------|
|RE-001| Permitir que o usuário cadastre tarefas | ALTA | 
|RE-002| Emitir um relatório de tarefas no mês   | MÉDIA |


### Contra-Escopo

| ID    | Descrição do Contra-Escopo                                                   | 
|-------|------------------------------------------------------------------------------|
| CE-001| Treinamento de modelo de linguagem natural (LLM).                             |
| CE-002| Pesquisa de viabilidade do mercado.                                           |
| CE-003| Desenvolvimento de hardware proprietário para captura de imagens.             |
| CE-004| Monitoramento de condições ambientais, como temperatura e umidade.            |
| CE-005| Suporte a plataformas de nuvem que não sejam Cloud.                             |
| CE-006| Implementação de funcionalidades de gestão de projetos dentro do sistema.     |
| CE-007| Desenvolvimento de aplicativos móveis nativos para plataformas específicas.   |


### Condições para início do Projeto

| ID     | Descrição de Condições para Início do Projeto                                  | 
|--------|--------------------------------------------------------------------------------|
| CI-001 | Assinatura de contrato de prestação de serviços.                               |
| CI-002 | Apresentação de garantias definidas no contrato.                               |
| CI-003 | Disponibilidade de acesso aos recursos e serviços Cloud necessários.              |
| CI-004 | Aquisição e configuração das câmeras para a segurança nas obras.                    |
| CI-005 | Treinamento inicial da equipe de segurança para uso do sistema.                 |

## Marcos Agendados e Entregas

| ID   | Marco do Projeto                                                                 | 
|------|-----------------------------------------------------------------------------------|
| M-1  | Liberação do sistema para cadastro de informações e configuração inicial.         |
| M-2  | Permissão para uso do sistema por usuários focais.                                |
| M-3  | Conclusão da integração com câmeras para a segurança.               |
| M-4  | Desenvolvimento e integração do painel de monitoramento em tempo real.            |
| M-5  | Testes de desempenho e conformidade.                                              |
| M-6  | Entrega final da solução e início do treinamento do usuário final.                |
| M-7  | Auditoria de conformidade com segurança após 3 meses de uso.                      |
| M-8  | Lançamento da versão 2.0 com melhorias baseadas no feedback do usuário.           |

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

......  COLOQUE AQUI O SEU TEXTO ......

> Apresente a divisão de papéis e tarefas entre os membros do grupo.
> Indique as responsabilidades de cada membro do grupo no projeto.

## Ferramentas

......  COLOQUE AQUI O SEU TEXTO - SIGA O EXEMPLO DA TABELA ABAIXO  ......

> Liste as ferramentas empregadas no desenvolvimento do projeto, justificando a escolha delas, sempre que possível.
> Todas as ferramentas utilizadas devem ser listadas.
> Qualquer tipo de ferramenta que for utilizada para construção de um artefato deve ser identificada, uma vez que podem ser necessárias alterações.
> A necessidade de uso de licenças e possíveis custos relacionados devem ser indicados.

| Ambiente              | Plataforma         | Link de Acesso             | Justificativa |
|-----------------------|--------------------|----------------------------|---------------|
| Quadro Kanban         | Github             | https://github.com/XXXXXXX | Centralização e organização do projeto no próprio repositório. |
| Repositório de código | GitHub             | https://github.com/XXXXXXX |               |
| Protótipo Interativo  | MavelApp ou Figma  | https://figma.com/XXXXXXX  |               |
| Documentos Textuais   | LibreOffice Writer | N/A                        |               |
| Planilhas e Gráficos  | Google Planilhas   | https://docs.google.com/   |               |
| EAP / WBS             | | | |
| Cronograma do Projeto | | | |
| Matriz RACI           | | | |

```diff
+ Tarefa 03:
+ Fim da seção a ser atualizada.
```

----
