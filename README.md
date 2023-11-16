# Cloud_computing_curso_AdaTech
Nesse documento apresento meus aprendizados no módulo de Cloud Computing da trilha digital da Ada Tech.

## Cloud Computing

Cloud computing é um modelo de computação que permite o acesso a recursos de computação, como armazenamento, processamento de dados, servidores, redes e software, pela internet, em vez de depender de recursos locais ou de hardware físico localizado em um local específico. Em vez de ter servidores e sistemas físicos, os usuários acessam e utilizam esses recursos por meio da internet, geralmente pagando apenas pelo que consomem.

O conceito de computação em nuvem teve origens em ideias e tecnologias anteriores, mas sua popularidade e adoção generalizada começaram a ganhar força no início dos anos 2000. Empresas como Amazon, Google e Microsoft foram pioneiras na oferta de serviços de computação em nuvem, desenvolvendo infraestruturas maciças para fornecer recursos computacionais sob demanda.

A ideia fundamental por trás da computação em nuvem é a virtualização de recursos, permitindo que os usuários acessem poder computacional, armazenamento e serviços através da internet, escalando conforme suas necessidades sem ter que investir em infraestrutura própria.

Os principais modelos de serviços de nuvem são:

1. **IaaS (Infraestrutura como Serviço)**: Fornecimento de recursos de TI, como máquinas virtuais, armazenamento e redes.
2. **PaaS (Plataforma como Serviço)**: Oferta de uma plataforma completa de desenvolvimento e implantação de aplicativos.
3. **SaaS (Software como Serviço)**: Disponibilização de software por meio da nuvem, acessado geralmente por navegadores web ou APIs.

A computação em nuvem revolucionou a maneira como empresas e usuários individuais lidam com dados e recursos de computação, permitindo mais flexibilidade, escalabilidade e redução de custos em comparação com a infraestrutura de TI tradicional.

## Cloud privada x publica

As nuvens públicas e privadas são duas formas distintas de implementar serviços de computação em nuvem, cada uma com suas características específicas:

**Nuvem Pública:**
- **Acesso Público:** Os serviços de nuvem pública são oferecidos por provedores de serviços em nuvem para o público em geral através da internet. Grandes empresas como Amazon Web Services (AWS), Microsoft Azure e Google Cloud Platform (GCP) oferecem serviços de nuvem pública.
- **Recursos Compartilhados:** Os recursos, como servidores, armazenamento e redes, são compartilhados entre múltiplos usuários ou organizações. Isso permite escalabilidade rápida e eficiente, mas pode gerar preocupações com segurança e privacidade.
- **Custo Variável:** Normalmente, os usuários pagam pelos recursos que consomem, seguindo um modelo de pagamento por uso. Isso pode ser vantajoso para pequenas e médias empresas que não querem investir em infraestrutura própria.

**Nuvem Privada:**
- **Infraestrutura Dedicada:** A nuvem privada é operada exclusivamente para uma única organização. Pode ser hospedada localmente ou em um data center de terceiros, sendo dedicada a essa organização e não compartilhada com outros usuários externos.
- **Maior Controle e Segurança:** Geralmente, oferece um nível maior de controle sobre a segurança, conformidade e personalização, o que pode ser fundamental para setores regulamentados ou que lidam com informações sensíveis.
- **Custo e Complexidade:** As nuvens privadas tendem a ser mais caras de se configurar e manter, devido à necessidade de infraestrutura dedicada e gerenciamento especializado.

**Híbrida e Multicloud:**
Além desses dois modelos, existem abordagens híbridas e multicloud, que combinam elementos de nuvens públicas e privadas. 
- **Nuvem Híbrida:** Combina recursos de nuvens públicas e privadas, permitindo que aplicativos e dados sejam compartilhados entre elas.
- **Multicloud:** Envolvem o uso de várias nuvens públicas de diferentes provedores, aproveitando as vantagens específicas de cada provedor para diferentes cargas de trabalho ou serviços.

A escolha entre nuvem pública e privada geralmente depende das necessidades de segurança, conformidade, custo e flexibilidade de uma organização. Algumas empresas optam por uma abordagem híbrida ou multicloud para obter o melhor dos dois mundos.

Modelos IaaS, PaaS, SaaS e Serverless

Esses modelos representam diferentes níveis de serviços oferecidos na computação em nuvem:

1. **IaaS (Infraestrutura como Serviço):**
   - Fornece recursos fundamentais de infraestrutura de TI pela internet.
   - Os usuários têm controle sobre sistemas operacionais, armazenamento, redes e algumas aplicações.
   - Exemplos: Amazon Web Services (AWS) EC2, Microsoft Azure Virtual Machines.

2. **PaaS (Plataforma como Serviço):**
   - Oferece um ambiente de desenvolvimento e implantação completo para criar aplicativos pela internet.
   - Elimina a necessidade de gerenciar a infraestrutura subjacente.
   - Exemplos: Google App Engine, Heroku, Microsoft Azure App Service.

3. **SaaS (Software como Serviço):**
   - Disponibiliza aplicativos hospedados na nuvem, acessados pela internet.
   - Os usuários finais podem usar esses aplicativos sem se preocupar com manutenção ou gerenciamento.
   - Exemplos: Google Workspace (anteriormente G Suite), Microsoft 365, Salesforce.

4. **Serverless Computing (Computação sem Servidor):**
   - É um modelo de nuvem em que os provedores de nuvem gerenciam a infraestrutura.
   - Os desenvolvedores podem executar códigos em pequenas unidades chamadas de funções, sem se preocupar com o hardware subjacente.
   - Oferece escalabilidade automática, cobrando apenas pelos recursos consumidos.
   - Exemplos: AWS Lambda, Azure Functions, Google Cloud Functions.

Cada um desses modelos oferece um nível diferente de controle, gerenciamento e responsabilidades para os usuários, permitindo que escolham a opção mais adequada às suas necessidades. O Serverless Computing, por exemplo, é uma evolução na direção de minimizar a necessidade de gerenciamento de infraestrutura, permitindo que os desenvolvedores se concentrem apenas no código e na lógica de negócios.

## Cloud AWS

### Zonas de disponibilidade (AZs)

AZs, ou Zonas de Disponibilidade, são unidades distintas dentro de uma região de um provedor de serviços em nuvem que oferecem redundância física e independência de falhas. Cada zona é composta por um ou mais data centers que são separados fisicamente dos outros, mas estão interconectados através de redes de baixa latência e alta velocidade.

A ideia principal por trás das Zonas de Disponibilidade é fornecer uma infraestrutura que seja resistente a falhas. Se um data center em uma zona específica falhar devido a um desastre natural, falha de energia ou qualquer outro motivo, outras zonas ainda estarão operacionais, garantindo alta disponibilidade para os serviços hospedados na nuvem.

Por exemplo, na Amazon Web Services (AWS), cada região pode ter várias Zonas de Disponibilidade. Quando você implanta recursos na AWS, como servidores ou bancos de dados, pode distribuí-los entre essas Zonas de Disponibilidade para garantir redundância e alta disponibilidade dos serviços.

Essa abordagem de design em Zonas de Disponibilidade é uma prática comum em infraestruturas de nuvem para garantir que os serviços permaneçam disponíveis mesmo em caso de problemas em uma determinada área geográfica ou data center específico.

## Arquitetura para cloud

A arquitetura para a nuvem é fundamental para garantir que uma aplicação ou sistema seja robusto, escalável, seguro e eficiente quando implantado em um ambiente de computação em nuvem. Aqui estão alguns elementos-chave a considerar ao projetar uma arquitetura para a nuvem:

1. **Microservices:**
   - Desenvolvimento de aplicações divididas em serviços independentes que se comunicam por APIs. Isso permite escalabilidade e manutenção mais fácil.

2. **Elasticidade e Escalabilidade:**
   - Projete para lidar com variações de carga, permitindo que recursos sejam alocados ou desalocados automaticamente conforme a demanda, usando autoescala e recursos elásticos.

3. **Resiliência:**
   - Projete para lidar com falhas de maneira eficaz. Isso pode incluir redundância, replicação de dados e distribuição geográfica.

4. **Segurança:**
   - Implemente medidas de segurança em várias camadas, incluindo autenticação, autorização, criptografia de dados, monitoramento e gerenciamento de identidades.

5. **Arquitetura de Rede:**
   - Considere a conectividade entre diferentes componentes e serviços na nuvem. Utilize serviços de balanceamento de carga, content delivery networks (CDNs) e redes privadas virtuais (VPNs) quando necessário.

6. **Monitoramento e Logging:**
   - Implemente sistemas robustos de monitoramento e registro para acompanhar o desempenho, identificar problemas e fazer ajustes conforme necessário.

7. **Automação:**
   - Utilize ferramentas de automação para provisionamento de recursos, implantação e gerenciamento de infraestrutura.

8. **Compliance e Governança:**
   - Garanta que a arquitetura esteja alinhada com regulamentações, políticas internas e práticas de governança.

9. **Multi-cloud e Hybrid Cloud:**
   - Considere a possibilidade de utilizar diferentes provedores de nuvem ou uma combinação de nuvem pública e privada, dependendo dos requisitos de negócios.

10. **Arquitetura Serverless:**
   - Explore a utilização de serviços serverless para focar no código e permitir que o provedor de nuvem gerencie a infraestrutura.

Ao projetar uma arquitetura para a nuvem, é essencial avaliar os requisitos específicos da aplicação, suas necessidades de desempenho, segurança, escalabilidade e a capacidade de resposta às demandas variáveis do usuário.

### Well Architected Framework

O Well-Architected Framework (WAF) é um conjunto de melhores práticas e princípios para projetar e avaliar arquiteturas de sistemas na nuvem de maneira eficaz. Desenvolvido pela Amazon Web Services (AWS), o WAF ajuda organizações a entender, avaliar e implementar arquiteturas de nuvem de alto desempenho, seguras e eficientes.

Ele se baseia em cinco pilares principais:

1. **Operacional Excelente:**
   - Envolve a execução eficiente e eficaz dos sistemas, gerenciando e monitorando continuamente as operações para garantir a entrega contínua de valor aos clientes.

2. **Segurança:**
   - Garante a proteção dos dados, sistemas e ativos usando controles de segurança adequados, práticas de conformidade e gerenciamento de riscos.

3. **Confiança:**
   - Foca na confiabilidade dos sistemas, assegurando a resiliência para lidar com falhas e manter a disponibilidade, além de minimizar o impacto de eventos inesperados.

4. **Eficiência de Desempenho:**
   - Garante o uso eficiente dos recursos computacionais para atender às demandas dos sistemas, otimizando custos e maximizando o desempenho.

5. **Otimização de Custos:**
   - Envolve a maximização dos benefícios dos recursos investidos na nuvem, identificando oportunidades de economia e eliminando gastos desnecessários.

6. **Sustentabilidade**
    - Se concentra em minimizar os impactos ambientais da execução de workloads em nuvem. 

O WAF fornece uma estrutura para avaliação contínua, ajudando na identificação de áreas de melhoria, otimização e garantindo que as arquiteturas na nuvem estejam alinhadas com as metas de negócios, sejam resilientes e seguras.

Ele é uma ferramenta valiosa para arquitetos de soluções, desenvolvedores e equipes de operações que buscam criar e manter arquiteturas robustas na nuvem, seguindo as melhores práticas recomendadas pela AWS.

## Infraestrutura como código

A infraestrutura como código (IaC) é uma abordagem na qual a infraestrutura de TI, como servidores, redes, bancos de dados e recursos de armazenamento, é gerenciada e provisionada usando código e scripts ao invés de processos manuais.

Essa prática permite que os desenvolvedores e equipes de operações automatizem o provisionamento, configuração e gerenciamento de recursos de infraestrutura por meio de linguagens de programação ou declarações descritivas, como YAML ou JSON. Isso oferece vários benefícios:

1. **Automatização e Consistência:** Ao escrever código para provisionar recursos, é possível automatizar tarefas repetitivas e garantir que a configuração seja consistente em diferentes ambientes (desenvolvimento, teste, produção).

2. **Gerenciamento de Versão e Rastreamento de Mudanças:** O código de infraestrutura pode ser versionado, revisado e controlado por sistemas de controle de versão (como Git), facilitando o rastreamento de mudanças e a reversão a versões anteriores, se necessário.

3. **Agilidade e Escalabilidade:** A IaC permite a escalabilidade rápida e eficiente, permitindo que recursos sejam provisionados e modificados de maneira ágil e responsiva às necessidades do negócio.

4. **Padronização e Reprodutibilidade:** A padronização é facilitada, garantindo que a configuração seja reproduzível em diferentes ambientes ou regiões de nuvem.

5. **Facilidade de Colaboração:** Equipes multidisciplinares podem colaborar mais facilmente, compartilhando e revisando o código de infraestrutura como parte do ciclo de desenvolvimento.

Ferramentas como Terraform, AWS CloudFormation, Azure Resource Manager (ARM) e Ansible são exemplos comuns usados para implementar a IaC, permitindo que os desenvolvedores descrevam a infraestrutura desejada em um formato legível por máquina e implantem essa infraestrutura de maneira consistente e repetível.

A IaC é essencial na computação em nuvem, pois suporta a agilidade, automação e consistência necessárias para gerenciar infraestruturas modernas e escaláveis.

## Deployment em Cloud e esteiras de CI/CD

O deployment na nuvem se refere ao processo de distribuir, instalar e disponibilizar uma aplicação, serviço ou atualização de software em um ambiente de computação em nuvem. Isso pode ser feito de várias maneiras, dependendo da infraestrutura, das necessidades da aplicação e das práticas da equipe de desenvolvimento. Aqui estão alguns métodos comuns de deployment na nuvem:

1. **Continuous Deployment (Implantação Contínua):**
   - Automatização do processo de deployment, onde qualquer alteração no código-fonte que passe pelos testes automatizados é implantada automaticamente no ambiente de produção.

2. **Continuous Integration/Continuous Deployment (CI/CD):**
   - Combinação de Continuous Integration (Integração Contínua) e Continuous Deployment (Implantação Contínua) para automatizar todo o ciclo de vida do software, desde a integração de código até a entrega e implantação na produção.

3. **Deploy Manual:**
   - Implantação realizada manualmente por uma equipe, geralmente por meio de ferramentas de gerenciamento de configuração ou diretamente nas interfaces de gerenciamento de serviços em nuvem.

4. **Orquestração de Contêineres:**
   - Uso de ferramentas como Kubernetes para implantar e gerenciar contêineres em escala na nuvem, permitindo atualizações e implantações de maneira mais fácil e eficiente.

5. **Serverless Deployment:**
   - Implantação de código em um ambiente serverless, como AWS Lambda ou Azure Functions, onde o provedor de nuvem gerencia a infraestrutura e dimensiona automaticamente com base na demanda.

As plataformas de nuvem oferecem serviços e ferramentas específicas para facilitar esses processos de deployment, fornecendo APIs, consoles de gerenciamento, integração com ferramentas de automação (como Jenkins, GitLab CI/CD, CircleCI) e orquestração de contêineres para simplificar e agilizar o deployment de aplicações na nuvem.

A escolha do método de deployment depende das necessidades da aplicação, da estrutura da equipe e das preferências em termos de automação, controle e gerenciamento do ciclo de vida do software.

### Esteiras de CI/CD

As esteiras de CI/CD (Integração Contínua/Implantação Contínua) são conjuntos de processos automatizados que permitem aos desenvolvedores construir, testar e implantar software de maneira eficiente e consistente. Elas automatizam o ciclo de vida do desenvolvimento de software, desde a integração do código até a entrega e implantação em produção.

**Integração Contínua (CI):**
- **Desenvolvimento Colaborativo:** Os desenvolvedores frequentemente fazem commits de código em um repositório compartilhado.
- **Builds Automatizadas:** Esses commits acionam processos automáticos de build e testes para verificar se as alterações não quebram o código existente.
- **Feedback Rápido:** Identifica problemas mais cedo, reduzindo conflitos de integração e facilitando a resolução de bugs.

**Implantação Contínua (CD):**
- **Entrega Automatizada:** Após a etapa de CI, o código aprovado passa para a etapa de entrega.
- **Testes Adicionais:** Testes adicionais são realizados para garantir a qualidade do software.
- **Implantação Automatizada:** Uma vez aprovado, o código é implantado automaticamente nos ambientes de teste, pré-produção e produção, dependendo da configuração da esteira.

**Ferramentas de CI/CD:**
- **Jenkins:** Uma das ferramentas mais populares para automação de CI/CD, oferece flexibilidade e personalização.
- **GitLab CI/CD:** Integrado diretamente com repositórios GitLab, oferecendo um conjunto robusto de recursos de CI/CD.
- **CircleCI:** Plataforma hospedada para CI/CD, fornecendo integração contínua e entrega automatizada em um ambiente na nuvem.
- **GitHub Actions:** Ferramenta integrada ao GitHub para criar workflows de CI/CD diretamente de repositórios GitHub.
- **Travis CI:** Oferece integração contínua para projetos de código aberto e privados.

As esteiras de CI/CD são fundamentais para as equipes de desenvolvimento modernas, permitindo que entreguem software de maneira rápida, confiável e repetível. Automatizam tarefas, reduzem erros, aceleram o feedback e ajudam a manter a consistência ao longo do ciclo de vida do desenvolvimento de software.

## Segurança em Cloud 

A segurança na nuvem é uma consideração crítica e envolve uma série de práticas e medidas para proteger os dados, as aplicações e a infraestrutura hospedados em ambientes de computação em nuvem. Aqui estão alguns aspectos importantes da segurança em nuvem:

1. **Controle de Acesso:**
   - Utilização de sistemas de autenticação robustos, como autenticação de dois fatores (2FA) e gerenciamento de identidade para controlar quem tem acesso aos recursos na nuvem.

2. **Criptografia de Dados:**
   - Implementação de criptografia para proteger dados em repouso e em trânsito, garantindo que mesmo se os dados forem interceptados, não possam ser lidos sem a chave de descriptografia.

3. **Gerenciamento de Identidade e Acesso (IAM):**
   - Configuração de políticas de IAM para conceder permissões precisas aos usuários, limitando o acesso apenas ao necessário para realizar suas funções.

4. **Monitoramento e Detecção de Ameaças:**
   - Implementação de sistemas de monitoramento contínuo, análise de logs e detecção de ameaças para identificar atividades suspeitas ou anômalas na infraestrutura.

5. **Atualizações e Patches:**
   - Manutenção regular e aplicação de patches de segurança para sistemas operacionais, aplicativos e serviços em nuvem para proteger contra vulnerabilidades conhecidas.

6. **Backup e Recuperação de Desastres:**
   - Implementação de estratégias de backup regulares e planos de recuperação de desastres para garantir a continuidade dos negócios em caso de falha ou ataque.

7. **Segurança em Camadas:**
   - Utilização de abordagens de segurança em camadas, implementando firewalls, segmentação de rede e controles de acesso para criar uma defesa robusta.

8. **Conformidade e Governança:**
   - Adesão a regulamentações de segurança, políticas internas e práticas de governança para garantir que a infraestrutura na nuvem esteja em conformidade e siga as melhores práticas.

Provedores de nuvem como AWS, Azure e Google Cloud oferecem uma variedade de ferramentas e serviços para ajudar na implementação dessas práticas de segurança. No entanto, a responsabilidade pela segurança é compartilhada entre o provedor de nuvem e o usuário, e é importante que as organizações compreendam suas responsabilidades específicas para garantir uma postura de segurança robusta na nuvem.