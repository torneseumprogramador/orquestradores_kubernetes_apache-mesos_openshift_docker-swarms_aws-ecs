
# Visão geral
<p>A orquestração automatiza a implantação, o gerenciamento, a escala e a rede dos containers. Empresas que precisam implantar e gerenciar centenas ou milhares de containers Linux e hosts podem se beneficiar da orquestração de containers.</p>

<p>É possível usar a orquestração em todos os ambientes em que você usa os containers. Com ela, você implanta a mesma aplicação em ambientes diferentes sem precisar reprojetá-la. Além disso, com os microsserviços em containers, é mais fácil orquestrar serviços, incluindo armazenamento, rede e segurança.</p>

<p>Os containers oferecem às aplicações baseadas em microsserviços uma unidade de implantação e um ambiente de execução autônomo ideais. Eles possibilitam a execução independente de várias partes de uma aplicação em microsserviços no mesmo hardware, com um controle muito maior sobre os componentes individuais e ciclos de vida.</p>

<p>Usar a orquestração no gerenciamento do ciclo de vida dos containers também oferece suporte às equipes de DevOps que integram fluxos de trabalho de CI/CD a ele. Com as interfaces de programação de aplicações (APIs) e as equipes de DevOps, os microsserviços em containers são os pilares das aplicações nativas em nuvem.</p>

<p>Veja uma introdução à orquestração de containers empresariais com o Kubernetes</p>

# Qual é a finalidade da orquestração de containers?
Use a orquestração de containers para automatizar e gerenciar tarefas como:
- Provisionamento e implantação
- Configuração e programação
- Alocação de recursos
- Disponibilidade dos containers
- Escala ou remoção de containers com base no balanceamento de cargas de trabalho na infraestrutura
- Balanceamento de carga e roteamento de tráfego
- Monitoramento da integridade do container
- Configuração da aplicação com base no container em que ela será executada
- Proteção das interações entre os containers

# Ferramentas de orquestração de containers
- <b>Kubernetes: </b>
    - Comumente estilizado como K8s é um sistema de orquestração de contêineres open-source que automatiza a implantação, o dimensionamento e a gestão de aplicações em contêineres. Ele foi originalmente projetado pelo Google e agora é mantido pela Cloud Native Computing Foundation. Ele funciona com uma variedade de ferramentas de conteinerização, incluindo Docker.
    Muitos serviços de nuvem oferecem uma plataforma baseada em Serviço (Paas ou Iaas), onde o kubernetes pode ser implantado sob serviço gerenciado. Muitos fornecedores também provém sua própria marca de distribuição de kubernetes.
    - Alguns serviços de com Cluster Kubernetes já configurados são:
        - EKS - Elastic Kubernetes Service
        - AKS - Azure Kubernetes Service
        - GKE - Google Kubernetes Engine
    - Um dos mais conhecidos pela comunidade
- <b>Docker Swarm</b>
    - O Docker Swarm é um recurso do Docker que fornece funcionalidades de orquestração de contêiner, incluindo clustering nativo de hosts do Docker e agendamento de cargas de trabalho de contêineres. 
    Um grupo de hosts do Docker formam um cluster "Swarm" quando seus mecanismos do Docker estão em execução juntos no "modo Swarm". 
    - https://docs.microsoft.com/pt-br/virtualization/windowscontainers/manage-containers/swarm-mode
- <b>Apache Mesos</b>
    - 
- <b>Openshift</b>
- <b>AWS ECS</b>


### Referência
- https://www.redhat.com/pt-br/topics/containers/what-is-container-orchestration