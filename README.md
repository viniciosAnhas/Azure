<div align="center">

<img height = "150" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/azure/azure-original-wordmark.svg" />

</div>

### <p style="text-align: justify;"> O objetivo do presente README é apresentar o estudo do Microsoft Azure, para afim de conhecer a ferramenta, ter noções de serviços de nuvem e de certificações. </p>
___

## Sumário 📘

* [Introdução ao Azure](#introducao-ao-azure)
    * [Computação na Nuvem](#computacao-na-nuvem)
        * [Quais os beneficios da computação na nuvem ?](#quais-os-benefecios-da-computacao-na-nuvem)
    * [Modelos de Infraestrutura na Nuvem](#modelos-de-infraestrutura-na-nuvem)
___

## Introdução ao Azure <a name = "introducao-ao-azure"></a>

<p style="text-align: justify;">
    Iremos conhecer de modo geral sobre Computação na Nuvem, Benefícios, Modelos de Infraestrutura, Produtos do Azure, além de como criar a nossa conta no Azure, explorar o Azure através do Portal, Resource Groups, Controle de Acesso, Locks e politicas do Azure. 
</p>

##  Computação na Nuvem <a name = "computacao-na-nuvem"></a>

<p style="text-align: justify;"> 
    Segundo a <a href="https://pt.wikipedia.org/wiki/Instituto_Nacional_de_Padr%C3%B5es_e_Tecnologia" target="_blank">NIST</a>, Computação em nuvem é um modelo para permitir acesso ubíquo, conveniente e sob demanda via rede a um agrupamento compartilhado e configurável de recursos computacionais como redes, servidores, equipamentos de armazenamento, aplicações, serviços e etc. São serviços que podem ser rapidamente fornecidos e liberados com esforço mínimo de gerenciamento ou interação com o provedor de serviço.
</p>

<p style="text-align: justify;"> 
    São enumeradas 5 caracteristicas essenciais do modelo de cloud computing são eles: <b><i>auto serviço sob demanda</i></b>, <b><i>acesso amplo via rede</i></b>, <b><i>agrupamento de recursos</i></b>, <b><i>elasticidade rápida</i></b> e <b><i>serviços mensurados</i></b>. Iremos ver cada uma das cinco caracteristicas a seguir
</p>

* <b>Autoatendimento Sob Demanda (On-Demand Self-Service)</b><p style="text-align: justify;"> 
Refere-se ao serviço prestado pelos fornecedores de computação em nuvem que permite o fornecimento de recursos de nuvem sob demanda sempre que necessario. O usuário acessa os serviços de nuvem por meio de um painel de controle on-line, no nosso caso, é o portal do Azure. 
</p>

* <b>Amplo Acesso Via Rede (Broad Network Access)</b><p style="text-align: justify;"> 
Os recursos estão disponíveis na rede e são acessados por meio de mecanismos padrão que promovem o uso por plataformas heterogêneas. Por exemplo, você deve conseguir utilizar os recursos através do seu celular ou computador.
</p>

* <b>Agrupamentos de Recursos (Resource Pooling)</b><p style="text-align: justify;">
Os provedores devem atender vários clientes com serviços provisórios e escalonáveis. Esses serviços podem ser ajustados para atender ás necessidades de cada cliente, sem que nenhuma alteração seja aparente para o cliente ou usuário final. 
</p>

* <b>Escalabilidade Rapida (Rapid Elasticity)</b><p style="text-align: justify;"> 
Os recursos podem ser provisionados e liberados elasticamente, em alguns casos automaticamente, para escalar rapidamente para fora e para dentro de acordo com a demanda. Para o consumidor, os recursos disponíveis para provisionamento geralmente parecem ilimitados e podem ser apropriados em qualquer quantidade e a qualquer momento.
</p>

* <b>Serviços Mensurados (Measured Service)</b><p style="text-align: justify;">
Os sistemas em nuvem controlam e otimizam automaticamente o uso de recursos aproveitando um recurso de medição em algum nível de abstração apropriado ao tipo de serviço., por exemplo armazenamento, processamento, largura de banda e contas de usuários ativos. 
</p>

### Quais os benefícios da Computação na Nuvem ? <a name = "quais-os-benefecios-da-computacao-na-nuvem"></a>

<p style="text-align: justify;"> 
Vamos pensar em como era a computação nas empresas antes de utilizar os serviços de Cloud Computing. O espaço físico em alguns casos é sufuciente, quando maiores as necessidades da sua organização maiores e mais sofisticados os locais em que são montados. Normalmente os equipamentos de um datacenter são montados em armários metálicos ou racks e além de abrigar servidores, switches e storages, o ambiente precisa ser projetado para permitir o acesso de técnicos, ter a climatização adequada, o fornecimento de energia e a organização do cabeamento e na maioria são montados em cima de piso suspenso. 
</p>

<p style="text-align: justify;"> 
Precisamos levar em conta a disponibilidade de energia e até mesmo a possibilidade de desastres naturais. Quanto mais a sua empresa cresce nesse modelo, maior será o seu datacenter, ou seja irá gastar sempre mais. Em relação ao consumo de energia, um datacenter o consumo é elevado e é essencial para manter as operações. Portanto é preciso garantir a disponibilidade em casos de imprevistos como falhas técnicas ou quedas no fornecimento. Mesmo que a empresa for pequena e adotem um datacenter totalmente local, terá que manter todos os servidores e climatização e isso gera um custo elevado.
</p>

<p style="text-align: justify;"> 
Para manter um datacenter local e totalmente separado da nuvem você precisará de pessoas capazes de operarem eles e sempre terá alguma manutenção, além disso esses colaboradores terão que trabalhar em regime de plantão caso algum problema ocorra na madrugada por exemplo.
</p>

<p style="text-align: justify;"> 
Os servidores são equipamentos responsáveis por fornecer serviços e recursos aos demais componentes da rede, em muitos casos há dezenas ou centenas deles, entre eles podem ter servidores de banco de dados, WEB, arquivos, dependendo da sua aplicação e eles podem ser virtualizados. Isso também é um custo e bem elevado ja que são necessarios hardwares potentes e especificos para esses equipamentos.
</p>

<p style="text-align: justify;"> 
Já no quisito segurança, podemos falar em dois tipos, física e digital, no campo físico, a proteção inclui a estrutura do prédio ou sala que abriga o datacenter, o local precisa ter um controle de segurança para apenas pessoas autorizadas possam acessar o local do datacenter, geralmente utilizam portas com biometria ou cartão ou outros meios de segurança e sempre monitorado com câmeras e sensores. Ján no campo digital a proteção contra invasões externas ou vazamento fica a cargo do Firewall, enquanto outras soluções cuidam da monitoração de tudo o que acontece no ambiente, como registro de ações de usuários, falhas e definições de políticas.
</p>

<p style="text-align: justify;"> 
Precisamos disso nos dias de hoje ? 
</p>

<p style="text-align: justify;"> 
Não, por isso vamos fazer o contraponto com a computação na nuvem, principalmente para pequenas e médias empresas. Isso tudo que foi citado acima gera muito custo e boa parte disso podemos eliminas ou pelo menos reduzir indo para a nuvem. Vamos levantas cinco vantagens para realizar a migração para a nuvem
</p>

<p style="text-align: justify;"> 
A primeira dela seria a velocidade e agilidade, temos na nuvem a agilidade para acrescentar um servidor ao nosso Server Farms por exemplo, clicando em alguns botões, e não precisamos comprá los.
</p>

<p style="text-align: justify;"> 
O segundo item seria evitar ociosidade de equipamentos, em um exemplo simples você acaba de lançar um site que espera ter milhares de acessos por minuto, mas infelizmente, as coisas não andaram como você planejava e os pageviews não foram tão bons assim, no modelo sem computação na nuvem você já teria comprado um novo servidor e aumentar o seu link de internet, e esse custo não tem como devolver, já na nuvem com apenas um clik você destrói esse servidor e assim evita a ociosidade em equipamentos.
</p>

<p style="text-align: justify;"> 
Um outro item muito importante é pague pelo que você consome conhecido como <b>Pay-Per Use</b>, se você não esta mais usando o servidor na nuvem você apenas exlui ele, parando de usar parou de gastar.
</p>

<p style="text-align: justify;"> 
A diminuição de gastos com manutenção é um ponto que pesa bastante quando temos um datacenter local, se você tem todos os seus storages no seu datacenter local, por exemplo, quando tiver que substituir ou acrescentar armazenamento na sua empresa terá que chamar uma empresa especialista, já na nuvem, apenas com um clique você pode aumentar o seu poder de armazenamento.
</p>

<p style="text-align: justify;"> 
Outro item que é visível a todos, talvez essa seja o principal ponto, se sua empresa trabalha com produtos online com a computação na nuvem você pode implantar facilmente seu aplicativo em várias regiões do mundo com apenas um clique, com isso temos baixa latência e uma experiência melhor para seus clientes de forma simples com baixo custo.
</p>

<p style="text-align: justify;">
E por último mas nao menos importante a segurança, no modelo datacenter você terá toda a segurança fisica, já na nuvem isso é eliminado 100% pois sua segurança e o login de acesso ao portal. Já na parte de aplicação, o Azure tem inúmeras soluções para isso.
</p>

## Modelos de Infraestrutura na Nuvem <a name = "modelos-de-infraestrutura-na-nuvem"></a>

<p style="text-align: justify;">
Existem três tipos de modelos de infraestrutura na nuvem, <b><i>púlica</i></b>,
<b><i>híbrida</i></b> e <b><i>privada</i></b>, iremo ver um pouco sobre cada uma delas.
</p>

* <b>Pública</b><p style="text-align: justify;"> 
São aplicativos e serviços que existem apenas na internet, e são características em serem multi-tenant, na qual uma única instância de serviço é executado em um servidor e atende a vários clientes ou requisições. O Azure por exemplo é uma referência de um sistema de nuvem pública.
</p>

* <b>Privado</b><p style="text-align: justify;">
Uma nuvem privada oferece a você todas as características de uma nuvem, resiliência, escala, auto atendimento e todas as definições que conhecemos, porem todos os serviços existem de forma local e esse modelo requer um ivestimento muito grande pois mesmo trabalhando de forma local precisamos ter reseliência em escala e para isso teremos que ter um  enorme parque datacenter local.
</p>

* <b>Híbrida</b><p style="text-align: justify;">
E como o nome já diz, temos uma infra local e remota fazendo o híbrido entre o público e o privado e o Azure é uma ótiuma opção para trabalhar de forma híbrida tendo soluções para isso. A ideia é estender o seu ambiente local para a nuvem onde você torna se capaz de gerenciar um one-premise e na nuvem juntos como em um grupo.
</p>