# resumo-do-lab
"Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO".
Conteudo estudado no modulo:
1-Conceitos e definição de Computação em Nuvem
2-O que é computação em nuvem
3-Modelos de Nuvem
4-Custo de Capital e Cisto operacional
5-Definição de nuvem puiblica, privada e hibrida
6-Identificação dos casos de uso para cada tipo de modelo de nuvem
7-Modelos de consumo 
8-Comparação de modelos de preços
9-
-------------------------------------------
Os beneficious da nuvem
-descrever os beneficious da alta disponibilidade e da escalabilidade da nuvem.
-descrever os beneficious da confiabilidade e da previsibilidade da nuvem.
-Descrever os beneficious de segurançae de governança a sim como a capacidade de gerenciamento na nuvem.
Alta disponibilidade: Se concentra em garantir a a disponibilidade maxima, independentemente de interrupções ou eventos que possam ocorre.
no Azure existe um ambient de nuvem altamente disponível com garantias chamadas de SLAs (contratos de nível de serviço)
Escalabilidade: E a capacidade de ajustar recursos para atender as demandas, significa que pode-se adicionar mais recursos para alinhar com o aumento da demanda. Um dos beneficious desse modelo é que se paga somente oque se usa podendo aumentar e diminuir conforme a necessidade da demanda. Esse recurso e conhecido como movimento vertical podendo aumentar a capacidade de processamento adicionando mais CPUs ou RAM.
Elasticidade: quando ha um salto repentino acentuado na demandas os recursos implantados poderiam ser expandidos, pode-se adicionar mais maquinas virtuais ou container por meio da expansão. da mesma forma pode-se diminuir quando a demanda diminuir também. esse recurso e conhecido como movimento horizontal.
Confiabilidade: com o modelo de design descentralizado, a nuvem suporta uma infra confiável e resiliente permitindo que se tenha recursos em varias regiões do mundo.
Previsibilidade: Permite o avanço confiante no desempenho ou custo, com uso do Microsoft Azure Well-Architected Framework.
Segurança: fornece uma grande variedade de recursos e ferramentas onde muitas delas implantas pelo cliente. dependendo do modele de segurança a ser adotado pela empresa pode se implantado infraestrutura como serviço onde os recursos são gerenciados pelo cliente recursos como sistema operacional app instalados, patches e manutenção. O modelo de plataforma como serviço toda a manutenção, atualização e aplicações de Patchs são realizadas pela novem assim como o modelo de software como serviço.
Governança: Processo de auditoria em nuvem, sinaliza qualquer recurso que esteja fora de conformidade como os padrões, ajuda a manter o ambiente protegido a atualizado e bem gerenciada.
Gerenciabilidade: sendo um dos principais beneficious da nuvem, o gerenciamento diz respite a maneira de gerenciar o ambiente em novem e seus recursos,  por meio de portal web, CLI, APIs ou PowerShell.
------------------------------------------------------------------------------------
Descrever os serviços de:
IaaS : Infraestrutura com serviço
PaaS : Plataforma como serviço
SaaS : Software como serviço
Classificar e identificar cada modelo de caso de uso para os serviço em nuvem
Modelos de responsabilidade compartilhada 

IaaS : IaaS oferece flexibilidade, controle e escalabilidade sem precedentes, sendo ideal para empresas que desejam modernizar sua infraestrutura mantendo autonomia e eficiência. Quando bem implementado com boas práticas e governança, IaaS reduz custos, melhora a agilidade operacional e fortalece a resiliência do negócio.
principais aplicações : Hospedagem de sistemas legados sem necessidade de reescrita de código.
Ambientes de teste e desenvolvimento dinâmicos e descartáveis.
Infraestrutura escalável para startups e empresas em crescimento, sem necessidade de capital inicial elevado.
Soluções de Disaster Recovery (DR) geograficamente distribuídas.
Execução de aplicações críticas, como ERPs, bancos de dados, VMs para aplicações internas e servidores web.

PaaS : O PaaS oferece grandes vantagens em velocidade, escalabilidade e eficiência. Implementá-lo corretamente exige planejamento e boas práticas para obter o máximo de benefícios sem comprometer segurança e custo.
Aplicabilidades : Desenvolvimento Web e Mobile: Criação e hospedagem de aplicativos.
Big Data e Analytics: Plataformas PaaS integram serviços para processamento de dados e inteligência artificial.
Internet das Coisas (IoT): Facilitam conexão e processamento de dados de dispositivos IoT na nuvem.
Automação e Integração Corporativa: Integração de aplicações e APIs para conectar fluxos de trabalho entre sistemas distintos.

SaaS : SaaS, ou Software como Serviço, representa um modelo de distribuição e licenciamento de software onde o acesso à aplicação é fornecido via internet, geralmente sob um regime de assinatura.
Aplicabilidades : Gestão de Relacionamento com o Cliente (CRM): Salesforce, HubSpot CRM.
Planejamento de Recursos Empresariais (ERP): NetSuite, SAP Business ByDesign.
Ferramentas de Colaboração e Produtividade: Google Workspace, Microsoft 365, Slack, Zoom.
Marketing e Vendas: Mailchimp, RD Station, Pipedrive.
Gerenciamento de Projetos: Asana, Trello, Jira.
--------------------------------------------------------------------------------------------------------------------------------

Modulo 2:
Arquitetura e Serviços do Azure
AZ-900 : Introdução aos Conceitos Básicos do Microsoft Azure

Computação e rede :
- Comparar os tipos de computação do tipo instancia de contêiner, maquinas virtuais e funções conjuntos de dimensionamento de máquinas virtuais, conjuntos de disponibilidade de máquinas virtuais e a Área 
de Trabalho Virtual do Azure.
- descrever os requisito exigidos para maquina virtual.
- Onde a computação do Azure é um serviço sob demanda que fornece recursos de computação como disco, processador, memoria, rede e sistema operacional.
- maquinas Virtuais são ofertas de IaaS que oferece personalização e controle total, onde o conjunto de dimensionamento oferece uma oportunidade de balanceamento de carga para dimensionamento de carga.
- A Área de Trabalho Virtual do Azure é uma virtualização de área de trabalho e aplicativo executada na nuvem.
- Possibilidade de um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway. 
Reduza o risco de que o recurso seja deixado para trás.
Implantações reais de várias sessões.
- Contêineres do Azure oferecem um ambiente virtual leve e sem a necessidade de gerenciar o sistema operacional.
- Instâncias de Contêiner do Azure são uma solução PaaS para executar contêineres ou grupos de contêineres.
- Aplicativos de Contêiner do Azure também são uma oferta PaaS, permitindo balanceamento de carga e escalabilidade.
- O Serviço de Kubernetes do Azure atua como um orquestrador para contêineres em arquiteturas distribuídas e com grande volume.
- Azure Functions é uma solução PaaS que suporta computação sem servidor, executando código baseado em eventos quando necessário, sem infraestrutura durante períodos de inatividade.
- O logon de vários clientes permite que vários usuários façam logon no mesmo computador na ao mesmo tempo.
- Os aplicativos e serviços são empacotados em um contêiner que fica na parte superior do sistema operacional do host. 
Rede Virtual do Azure (VNet) permite que os recursos do Azure se comuniquem uns com os outros, com a Internet e com as redes locais.Pontos de extremidade públicos, acessíveis de qualquer lugar na Internet.Pontos de extremidade privados, acessíveis somente de dentro da sua rede.
- As O Gateway de VPN é usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela Internet pública. 
- Segurança do DNS do Azure baseia-se no gerenciador de recursos do Azure, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log. 
- Redes virtuais personalizáveis permitem que você use nomes de domínio privados e totalmente personalizados em suas redes virtuais privadas. 
- Os registros de alias dão suporte a conjuntos de registros de alias para apontar diretamente para um recurso do Azure.

--------------------------------------------------------------------------------------------------------------------------------------------------
