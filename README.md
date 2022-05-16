
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
- https://www.redhat.com/pt-br/topics/containers/what-is-container-orchestration


# Ferramentas de orquestração de containers e clusters
- <b>Kubernetes: </b>
    - Comumente estilizado como K8s é um sistema de orquestração de contêineres open-source que automatiza a implantação, o dimensionamento e a gestão de aplicações em contêineres. Ele foi originalmente projetado pelo Google e agora é mantido pela Cloud Native Computing Foundation. Ele funciona com uma variedade de ferramentas de conteinerização, incluindo Docker.
    Muitos serviços de nuvem oferecem uma plataforma baseada em Serviço (Paas ou Iaas), onde o kubernetes pode ser implantado sob serviço gerenciado. Muitos fornecedores também provém sua própria marca de distribuição de kubernetes.
    - Alguns serviços de com Cluster Kubernetes já configurados são:
        - EKS - Elastic Kubernetes Service
        - AKS - Azure Kubernetes Service
        - GKE - Google Kubernetes Engine
    - Um dos mais conhecidos pela comunidade
    - https://kubernetes.io/pt-br/

- <b>Docker Swarm</b>
    - O Docker Swarm é um recurso do Docker que fornece funcionalidades de orquestração de contêiner, incluindo clustering nativo de hosts do Docker e agendamento de cargas de trabalho de contêineres. 
    Um grupo de hosts do Docker formam um cluster "Swarm" quando seus mecanismos do Docker estão em execução juntos no "modo Swarm". 
    - https://docs.microsoft.com/pt-br/virtualization/windowscontainers/manage-containers/swarm-mode

- <b>Openshift</b>
    - OpenShift é um produto de software de computador da Red Hat para implantação e gerenciamento de softwares baseados em container. 
    Ele é uma distribuição suportada do Kubernetes usando Docker e ferramentas DevOps para desenvolvimento acelerado de aplicações.
    - O Red Hat OpenShift é uma solução de nível empresarial que oferece a tecnologia do Kubernetes e muito mais.
    Vem com todos os elementos extras que tornam o Kubernetes potente e viável para as empresas, incluindo componentes de registro, rede, telemetria, segurança, automação e serviços.
    - https://developers.redhat.com/products/rhoar/overview

- <b>AWS ECS</b>
    - O Amazon ECS facilita a implantação, o gerenciamento e o dimensionamento de contêineres do Docker que executam aplicativos, serviços e processos em lote. O Amazon ECS coloca contêineres em seu cluster com base em suas necessidades de recursos e é integrado a recursos conhecidos como Elastic Load Balancing, grupos de segurança do EC2, volumes do EBS e funções do IAM.
    - https://us-east-1.console.aws.amazon.com/ecs/home?region=us-east-1#/getStarted

- <b>Apache Mesos</b>
    - Desenvolvido na Universidade da Califórnia, Berkley, o Apache Mesos é um gerenciador de cluster de código aberto. Seu objetivo é fornecer isolamento e compartilhamento eficientes de recursos em estruturas ou aplicativos distribuídos. Em outras palavras, ajuda no compartilhamento de recursos de maneira refinada, melhorando assim a utilização do cluster. O Apache Mesos é considerado a base para um grande número de sistemas distribuídos.
    - O Apache Mesos foi construído com os mesmos princípios que o Linux Kernel. Alguns dos principais recursos do Apache Mesos são escalabilidade para milhares de nós, agendamento de vários recursos, interface com o usuário da web para visualização do estado do cluster, separação entre tarefas com contêineres do Linux e mestre replicado tolerante a falhas usando o Zookeeper. O Mesos, de certa forma, pode ser considerado o oposto da virtualização, pois a virtualização divide um único recurso físico em vários recursos virtuais, enquanto o Mesos combina vários recursos físicos em um único recurso virtual. 
    - O Apache Mesos consiste em processos e estruturas mestre, com o processo mestre gerenciando daemons escravos em execução em cada nó do cluster e estruturas cuidando das tarefas desses escravos. Os recursos oferecem uma lista de recursos gratuitos em vários escravos.
    Semelhante aos recursos de gerenciamento de sistemas operacionais de PC, o Apache Mesos pode alternar recursos de uma estrutura para outra conforme e quando necessário. Ele pode ajudar a reduzir muitas etapas manuais na implantação de aplicativos e pode ajudar a mudar as cargas de trabalho automaticamente para manter as taxas de utilização altas. O Apache Mesos, com a ajuda de um módulo de alocação conectável, ajuda as organizações a oferecer suporte a diversas políticas de alocação entre estruturas. 
    - O Apache Mesos está localizado entre a camada de aplicação e o sistema operacional. Isso facilita a implantação e pode gerenciar aplicativos com mais eficiência em ambientes em cluster de larga escala. Ele também pode executar vários aplicativos em um conjunto de nós compartilhados dinamicamente. O Apache Mesos também pode fornecer desempenho mais rápido do aplicativo.
    - O Apache Mesos foi adotado por várias empresas de software, incluindo a Apple.
    - Para os containers é possivel utilizar o docker compose para deployar containers dentro de uma estrutura com Apache Mesos
    - https://mesos.apache.org/
    - https://pt.theastrologypage.com/apache-mesos
    - https://thiagoviola.wordpress.com/2017/10/09/orquestratacao-de-containers-parte-1-conheca-kubernetes-docker-swarm-apache-mesos/
    - https://codefresh.io/kubernetes-tutorial/kubernetes-vs-docker-swarm-vs-apache-mesos/
