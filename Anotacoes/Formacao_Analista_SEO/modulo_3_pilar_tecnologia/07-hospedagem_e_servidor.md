# Hospedagem e Servidor

Iremos abordar SEO técnico nessa anotação; esse arquivo tem como pretenção abordar os temas de Hospedagem e Servidor sob a perspectiva de um desenvolvedor e analista de SEO para a melhor e mais performática utilização das tecnologias abordadas.

## Links de referência:

- Monitoramento de UPTIME:
  - https://uptimerobot.com/
  - https://www.pingdom.com/
- CDN:
  - https://www.cloudflare.com/pt-br/
  - https://www.gocache.com.br/
- Indicação de server de confiança:
  - https://www.hostinger.com/ (Cloud ou VPS)
  - https://wpengine.com/ (Hospedagem WordPress)
  - https://aws.amazon.com/pt/ (Cloud + CDN)
  - https://www.digitalocean.com/ (Cloud VPN)

## Entendendo Servidores no Trabalho de SEO:

Quando pensamos em SEO técnico temos de ter olhares precisos sobre os requisitos de cada negócio, de cada projeto. O olhar crítico, porém sensível, quanto as nuances dos resultados gerados na produção de um conteúdo ou oferta de serviço e produtos é mais do que essencial.

Começando com os fundamentos iremos abordar **o que exatamente é um Servidor Web**.

### Servidor Web, do que se trata?

O Servidor Web é um sistema de computador que processa solicitações via HTTP (Hypertext Transfer Protocol), que é o protocolo base de rede usado para distribuir informações na World Wide Web, na WWW, que nada mais é do que a própria Internet.

Essas solicitações são _"pedidos"_ de acesso, para **visualização, modificação, atualização e/ou deleção** de dados presentes na Web, resgatados de um servidor que analisa essas solicitações HTTP e determina se as permissões das operações citadas (as que estão em negrito) estão de acordo com o usuário que as requisita, dando algum retorno de sucesso, falha ou de falta de permissões para acesso à esses dados.

A função básica de um servidor é analisar essas solicitações, como citado acima, e entregar ao usuário/cliente o documento HTML (Hypertext Markup Language) correspondente à requisição HTTP feita. Todo servidor **processa aplicações, presta serviços e armazena dados**.

Quando digitamos um endereço de um site em um navegador, o DNS (Domain Name System, Sistemas de Nomes de Domínios) e o IP (Internet Protocol, um endereçamento que leva à sua máquina) encaminham a solicitação para o servidor correto.

> O DNS é o sistema de nomes que leva aos IPs que direcionam sua solicitação ao servidor correto.

Os servidores ou as empresas de hospedagem Web tem suas próprias máquinas (que são os servidores, computadores mesmo) e alugam esses recursos computacionais para que possamos hospedar os arquivos de nosso site e torná-lo acessível à outras pessoas. Ou seja, o caminho do seu site (https://www.seusite.com) levará até essa máquina que processará a requisição e retornará os arquivos pertinentes contidos lá.

O custo de criar servidores do zero é alto, pois demanda uma estrutura e expertise dos profissionais que a constroem para criar um sistema funcional, escalável, de fácil manutenção e, _principalmente_, seguro e rápido, pois possui recursos computacionais suficientes para tal.

#### Funções de um Servidor Web:

Um passo a passo para ilustrar as funções de um Servidor Web seria:

1. Construir e publicar páginas Web, que são os sites;
2. Baixar o protocolo de transferência de arquivos ou solicitações de FTP:
   - Onde ficam os sistemas de persistência de dados de um servidor, um HD da máquina, por exemplo, serão recebidos os dados e arquivos do seu site.
3. Enviar e receber e-mails.

Hoje em dia, temos empresas como a Microsoft ou Google que oferecem um serviço de e-mail a parte que não é necessário se utilizar de um sistema proveniente de um Servidor Web. Inclusive, quando se trata de e-mail, é melhor contratar serviços de outras empresas para que seu serviço fique mais rápido e mais barato, vindo do seu próprio servidor.

Devemos adequar as necessidades e equilibrar os custos de nossas aplicações, e esse é um dos principais desafios em um projeto de SEO. Mas o que impacta o Servidor Web no SEO?

### O impacto do Servidor Web no SEO:

Quando falamos se um Servidor Web ajuda ou atrapalha nos resultados de SEO, a resposta é **sim** para ambas.

Muitos fatores afetam os resultados de SEO em nossos projetos, e dando destaque ao Servidor percebemos que esses problemas ou soluções estão relacionadas à _qualidade de serviço_ que você recebe do seu provedor de hospedagem; Esse fator pode prejudicar MUITO ou ajudar MUITO.

Não adianta um site com conteúdo rico, em abundância, que possua a Expertise dos que criam os conteúdos sem a Autoridade gerada pela qualidade do site e dos serviços prestados e sem a Confiança que é resultado dos dois outros fatores sendo construída por uma experiência realmente completa de consumo da sua aplicação.

Um site lento, com muita instabilidade, páginas com erros, quedas de serviços (como no banco de dados), erros mostrados ao usuário... Podemos entender logo que é mais do que importante que a hospedagem do seu site seja de qualidade, seja de confiança e que entregue performance, além da segurança e fácil manutenção (muitas vezes abstraída pelos provedores).

Ao considerar os custos, o _budget_, do seu projeto, inclua sempre um bom provedor de hospedagem, ou rearrange seu negócio para que tenha isso garantido.

Quando a qualidade do serviço de hospedagem não é boa, os impactos são MUITO negativos. Mas utilizando bons serviços de hospedagem temos um servidor estável que garante uma boa conexão dos usuários com os recursos e conteúdo ofertado pelo site para que a experiência de quem consome seja a melhor possível, sem erros ou lentidão. Tudo isso corrobora para a análise, processamento e ranqueamento que os crawlers (bots dos Mecanismos de Busca) fazem em seu site.

> A escolha do Host é um fator significativo para determinar o tipo de experiência que o usuário terá com seu site.
>
> Um ótimo Host reduzirá a taxa de rejeição (pessoas que saem do seu site depois de visualizar apenas uma página) e aumentará a duração média de uma visita. Você também verá menos erros no site relacionados ao servidor e tempo limite de página.
>
> Esses fatores e muitos outros, numa lista gigantesca, afetam como o seu site irá se classificar nas bases de dados de mecanismos de buscas e pode ser justamente o diferencial entre você e sua concorrência.

#### Mas, especificamente, quais impactos são esses?

Vamos listar estes impactos então:

1. Velocidade de carregamento:
   - Relacionados aos recursos que temos disponíveis no servidor (memória, espaço em disco, processadores, placas de rede, conexão, etc.);
   - Também relacionado à quantidade de usuários conectados e consumindo os serviços simultaneamente, entre outros fatores.
2. Tempo de latência/localização:
   - Se contratamos um servidor americano e o usuário está acessando os serviços na região Sul do Brasil, o tempo de latência (de atraso das respostas das requisições) muito maior do que se contratarmos um servidor no Brasil;
   - Esse fator é justamente o que chama de problemas com o tempo de resposta do servidor.
3. UPTIME/Disponibilidade:
   - É muito comum vermos no mercado hospedagens compartilhadas que o site cai a todo momento e isso só pode ser verificado de forma preventiva e com caráter de manutenção com precisão por meio de serviços como [pingdom](https://www.pingdom.com/) e [UptimeRobot](https://uptimerobot.com/).
4. Disponibilidade de recursos:
   - Se o servidor é rápido, tem uma latência boa com uma localidade boa para seu público, seu cliente, e tem uma boa disponibilidade, podemos então falar da disponibilidade de recursos, que seria a capacidade de manter os serviços funcionando conforme updates, downgrades e alterações;
   - É a flexibilidade da disponibilidade dos serviços gerada no servidor.

Em suma, **se preocupe com a infraestrutura**.

### Como escolher o melhor servidor?

Podemos começar por três pontos:

**Qual a linguagem do seu site? PHP, ASP, Node?**

**Qual Sistema Operacional mais se encaixa à arquitetura e recursos necessários do site? Windows? Unix?**

**Qual o _budget_ para investir na hospedagem?**

Vamos detalhar esses pontos!

#### Sobre a linguagem de programação do seu projeto:

Se sua linguagem for **PHP**, prefira hospedagens com sistemas operacionais Linux (OS que opera PHP de forma mais ágil) e MySQL, que tem suas operações mais performáticas com o PHP. Mas sempre atento às versões do PHP disponíveis no servidor, dando preferência à hosts que tenham as versões mais atuais da linguagem.

Um ponto importante, todo servidor Linux costuma ter custos menores pois o sistema Linux é Open-Source, ou seja, desenvolvido pela comunidade para a comunidade. Dessa forma, servidores com sistemas Windows ou com Linux proprietários geralmente são mais caros, pois requerem a licença do uso do sistema operacional.

Muitos provedores afirmam que sua infraestrutura é compatível com Ruby. A razão para isso é que existem cada vez mais empresas usando Ruby on Rails. Então se preocupe mais em contratar Hosts que suportem as versões mais recentes do framework.

O Node.js faz parte de muitos produtos digitais, incluindo Netflix e Trello. Sua popularidade crescente faz com que vários hosts se adequem a linguagem. Então avalie seu orçamento.

A configuração de VPS ou servidores dedicados é repleta de dificuldades (e costumam ser as melhores para Python). A melhor hospedagem vai oferecer uma extensa base de conhecimento e uma equipe de suporte dedicada para ajudar na solução de problemas. Leve isso sempre em consideração.

> Temos algumas linguagens que são usadas predominantemente em servidores Linux, porém, em linguagens como o C# e tecnologias como .NET e ASP.NET devem rodar exclusivamente em ambientes Windows, pois foram desenvolvidas para a Microsoft afim de criar aplicações Desktop para seu sistema operacional.

#### Sobre a escolha do Sistema Operacional e os recursos necessários:

1 - **Pense no tráfego esperado!**

Para escolher o servidor/host mais adequado precisamos nos atentar ao armazenamento e largura de banda como métricas fundamentais. Quanto maior o tráfego esperado, maiores os requisitos devem ser definidos. Servidores compartilhados de baixo custo podem ser bons o suficiente no estágio inicial, mas seus investimentos crescerão junto do aumento de suas demandas e pode ser possível uma migração, que é cara, demanda tempo e é geralmente bem difícil de se realizar.

Quando determinamos qual vai ser a hospedagem utilizada, o por quê disso e qual linguagem vai ser utilizada, não precisamos nos prender à ter um servidor único que contém tudo que a empresa oferece/tem. Podemos ter servidores mais simples, separados, como um blog em Wordpress para a parte institucional e um e-commerce para a venda dos serviços e solicitação de orçamentos. Conseguimos fazer um "apontamento" pelo DNS para que façamos com que as requisições para nosso site apontem para um sistema específico.

Uma boa solução para lidar com o tráfego variável é justamente o uso de um serviço Cloud como AWS, que abstrai as complexidades de implementação de uma infraestrutura própria e tem seus requisitos e poder de processamento escaláveis, onde em muitos dos serviços da AWS pagamos pelo consumo e pelo poder de processamento, não por uma reserva com valor previamente determinado (mas tudo isso depende de o que e como você quer implementar teu site, existem inumeras formas de o implementar num servidor Cloud dentro da própria AWS que fogem da explicação dada). Implementações feitas em ambientes Cloud trazem a escalabilidade de uma forma muito mais fácil, sempre considere os custos e veja se o que é mais viável.

2 - **Escolha do OS e Recursos**:

Iremos abordar nesse tópico um comparativo em diversos quesitos entre o Linux e Windows.

Existe um mito expalhado pela comunidade de que os sistemas operacionais Linux são inseguros, então iremos salientar que não é o caso, pois a estrutura de grupos de usuários, permissões de pastas e arquivos, etc, constituem uma estrutura mais segura do que de um SO Windows. Esse preconceito com o Linux muito se deve à ser uma tecnologia Open Source, um conceito que muitos não entendem. Para saber mais sobre aplicações Open Source vá para o artigo da Red Hat ["O que é Open Source?"](https://www.redhat.com/pt-br/topics/open-source/what-is-open-source).

Muitas ferramentas de Banco de Dados e outros Recursos são exclusivos de certas plataformas, como o Microsoft SQL e o serviço de gerenciamento de e-mail Exchange, que são exclusivos do Windows. Sempre avalie os requisitos do seu sistema/aplicação e veja se as tecnologias que serão utilizadas batem com os requisitos de SO (Sistema Operacional).

ASP.NET e C# são linguagens de programação que são de uso exclusivo na criação de aplicações Windows, que necessitam de um ambiente Windows para funcionar. Já outras tecnologias são multiplataforma, mas são nativas do Linux como: PHP, Python, Peal, Ruby on Rails, etc.

Mas e sobre custo? Os valores de serviços e aplicações que rodam em ambientes Linux costumam ser gratuitas, isso incluindo o próprio sistema operacional, e muitas das vezes os que são pagos tem valores menores em comparação com serviços proprietários, como a plataforma Azure da Microsoft.

Podemos notar que o Linux é mais versátil, que possui maior compatibilidade e integração configurável com a maioria dos serviços e tecnologias que podemos considerar usar, porém os serviços que forem requisitos em seu projeto precisam atender às especificações e a exclusividade de SO é algo que deve ser sequido, para que possa ao menos funcionar ou não causar erros inesperados.

2.1 - **Os Recursos**:

Temos de nos atentar à escolha de CPUs, ao poder de processamento do nosso servidor escolhido.

A CPU do servidor é como se fosse o "cérebro" do sistema e ele trata todas as solicitações e processos necessários para o funcionamento da aplicação. Uma CPU geralmente tem dois ou mais núcleos, que são as entidades de processamento unificado que realizam as multiplas tarefas causadas pelas requisições que precisam ser processadas. Cada núcleo adicional fornece um aumento de poder computacional para lidar com o processamento, então nos traz mais performance.

É mais provável que você veja sobre a questão das CPUs do que sobre VCPUs, que estão presentes em VPS (Virtual Private Servers), que não são compartilhados entre outros serviços/aplicações e tem sua função completamente dedicada ao funcionamento do seu sistema, do seu site. As VCPUs são processadores dedicados dentro de Servidores Dedicados Privados que trazem maior desempenho e maior custo em sua contratação e manutenção, logo agregam mais valor a performance do seu aplicativo, porém, também agregam nos custos para utiliza-las/contrata-las.

Já sobre o armazenamento, podemos destacar que o tamanho da alocação contrata é o que limita "o tamanho do seu site". Isso, pois, o espaço alocado pela sua aplicação dentro de um HD ou SSD no provedor ou VPS é da mesma forma que em um computador pessoal, afinal também são computadores. De modo geral, a capacidade máxima de armazenamento do seu plano contratato ou construído é listada em Gigabytes (GB).

Podemos destacar que a utilização de SSDs no lugar de HDs é mais cara, porém dezenas de vezes mais rápida para realizar as operação de leitura, escrita, atualização e deleção de dados.

Agora, tratando da memória principal do computador, a RAM. Essa memória é de curto prazo e é "randômica", ela é utilizada durante a execução dos processos do SO e das aplicações que estão rodando nele, para que as operações sejam feitas de maneira mais ágil e concisa. Ela é responsável por armazenar dados voláteis que são mais do que essenciais em qualquer aparelho computacional e a falta de espaço nessa memória pode resultar no erro de servidor interno no seu site, o erro 500, e também é listada nos planos de contratação por Gigabytes (GB).

Devemos também considerar a Largura de Banda (Bandwidth), que é a taxa de transferência de dados suportada pelo servidor. Em outras palavras, determina a rapidez com que seu site pode retornar o conteúdo de uma requisição ao usuário. Quanto maior, MELHOR! Existem hospedagens no mercado que oferecem Largura de Banda ilimitada, algo que devemos sempre desconfiar pois pode se tratar de somente uma estratégia de Marketing, assim como em UPTIME e VCPUs.

Outro ponto super importante para seu projeto é: se dentro do seu servidor há um IP dedicado e se te fornecem acesso direto do seu plano ao FTP (File Transfer Protocol) do servidor mesmo se a aplicação não estiver no ar ou apontando para outro provedor (o que é ótimo para testes).

E tome cuidado com IPs compartilhados, pois se houver algum problema quanto a Confiabilidade do seu site por parte dos buscadores causado por outros sites do mesmo grupo, você também será penalizado pelas métricas dos buscadores. Então vale a pena ter um IP dedicado e acesso ao FTP, não é um custo frívolo, muito pelo contrário.

A maioria dos servidores oferecem algum tipo de serviço de e-mail atrelado a hospedagem. Pode valer a pena para pequenos projetos que não querem usar serviços proprietário mais caros como o do Google ou Microsoft, que costumam ter valores muito mais altos em comparação. Sempre avalie a disponibilidade desse serviço se for utilizar essa tecnologia específica.

3 - **Hospedagem e Orçamento**:

Após avaliar as tecnologias que serão utilizadas, como a linguagem de programação e frameworks, os recursos necessários e a expectativa de crescimento do negócio que sera implementado, devemos avaliar:

- O Host que vou utilizar suporta as versões mais recentes e adequadas das tecnologias que vou utilizar na aplicação?
- Qual Host que analisei tem os recursos de Hardware e outras especificações de conectividade para possuir uma qualidade de construção e manutenção boa?

E para ter uma resposta mais concisa dessas questões podemos elencar os tipos de hospedagem mais comuns do mercado:

| Dedicada                                                                                 | VPS (Servidor Privado Virtual)                                                                                                                                              | Compartilhada                                                                                                                                   | WordPress Gerenciado                                                                                                                                                 | Cloud                                                                                                                       |
| ---------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Uma hospedagem dedicada significa que temos um servidor só para nós                      | Meio termo entre hospedagem dedicada e compartilhada. Cada site teu seu próprio espaço dentro do servidor.                                                                  | Seu site será armazenado junto de diversos outros, dividindo a hospedagem.                                                                      | Já vem os recursos para facilitarem a configuração e manutenção do seu site WordPress.                                                                               | Hospedagem baseada em rede na qual os recursos são distribuídos por vários servidores individuais.                          |
| **Vantagem:** Provê mais controle sobre o servidor e um serviço mais rápido e confiável. | **Vantagem:** É uma ótima opção para um serviço em crescimento, pois alia as condições de um servidor dedicado (mas com menos controle) com o menor custo em relação à ele. | **Vantagem:** É o mais barato do mercado.                                                                                                       | **Vantagem:** Já é pensada com a implementação de um CMS (Content Manegement System) para gerir o site.                                                              | **Vantagem:** É a solução mais versátil de todas e mais fácil de se escalonar mediante crescimento ou queda do uso do site. |
| **Desvantagem:** Costuma ser um serviço muito caro.                                      | **Desvantagem:** Necessita de mais conhecimento para configurar e manter, mas também possui algumas interfaces mais amigáveis.                                              | **Desvantagem:** Seu site será mais lento e inevitavelmente irá afetar a UX (User Experience) e também costumam ser mais vulneráveis à ataques. | **Desvantagem:** Para quem tem mais conhecimento e gosta de uma abordagem mais técnica, pode gerar a impressão de menor controle sobre a aplicação e sua manutenção. | **Desvantagem:** Necessita de mais conhecimento técnico, mas há opções com painéis mais amigáveis para trabalhar.           |

<br>

> Por meio dos recursos de Virtualização (isolamento de máquina, de sistema operacional e de recursos) disponíveis num VPS ou Cloud, podemos abstrair a complexidade de multiplos servidores em ambientes isolados entre si, para aplicações que rodem em Linux e outras que rodem no Windows de uma mesma empresa.

4 - **Salientando pontos importantes e citando outros mais**:

- Alta garantia de UPTIME\* (99.9%):
  - Use ferramentas como [pingdom](https://www.pingdom.com/) e [UptimeRobot](https://uptimerobot.com/) para analisar e garantir esse recurso.
- Localização do servidor:
  - Você precisará reduzir o tempo de resposta (a latência) do seu site para uma melhor experiência do usuário.
- Suporte bem avaliado:
  - Independente do tamanho ou nível de senioridade do time de SEO e TI, ter um bom suporte nos serviços de hospedagem é essencial na hora de resolver problemas.
- Ferramentas e recursos úteis:
  - SSL, backup diário, suporte 24h, CDN\* incluso ou integração fácil com algum provedor de CDN do mercado, upgrade ou downgrade de recursos de maneira automática e escalável... Muitos outros detalhes podem ser citados, mas os "principais", que fazem mais diferença, foram elencados.

> Um UPTIME de 99.9% equivale a apenas 1,44 minutos de inatividade (no máximo) a cada 24h.<br>
> CDN (Content Delivery Network, Rede de Distribuição de Conteúdo). É uma rede de servidores que redireciona os conteúdos solicitados por um usuário para o mesmo, porém, vindo de uma localidade mais próxima dele, fazendo com que a entrega seja mais rápida, melhorando a UX.

### CDN e suas vantagens

CDN é a abreviação de Content Delivery Network (ou Rede de Distribuição de Conteúdo). É uma rede de servidores (pontos de presença) que armazenam cópias do seu conteúdo em cache e entregam para seus usuários de acordo com a localização geográfica, isso para entregar os conteúdos do seu site por meio de um servidor intermediário mais próximo de quem está acessando o site, trazendo rápidez e por consequência melhorando a UX. CDNs reduzem a latência, entregam o conteúdo mais rápido.

Normalmente CDNs possuem proteções contra ataques de DDoS e outros tipos de ataques também. Esse detalhe é algo muitas vezes esquecido ou simplesmente ignorado, mas é essencial em qualquer aplicação.

Basicamente, o CDN distrui cópias do seu conteúdo entre diversos pontos com servidores e atendem às requisições de usuários mais próximos à eles do que do seu servidor para diminuir o tempo de resposta, diminuir a latência, além de oferecer mais um reforço de segurança.

#### O que levar em consideração ao contratar um serviço de CDN?

1 - **Qual é o servidor principal desse serviço?**
2 - **Quantos pontos de presença (locais com servidores) esse serviço provê?**
3 - **Temos servidores suficientes para onde meu público está?**

### Dicas essencias de caráter geral:

1 - **Mantenha seus projetos em servidores rápidos, com bom suporte, que atendam aos requisitos, que sejam escaláveis e confiáveis;**
2 - **Ofereça recursos de hospedagem que ajudem os clientes com SEO, sempre levando em conta o orçamento disponível (maior eficiência pelo menor custo possível);**
3 - **Inclua seu projeto em serviços escaláveis para atender às necessidades em constante mudança de negócios em crescimento (migrações são trabalhosas, demoradas e caras);**
4 - **Empregue uma rede de entrega de conteúdo (CDN) para garantir um ótimo desempenho do site para entregas de requisições dos usuários das localidades que contém nosso público (há um projeto brasileiro chamado [gocache](https://www.gocache.com.br/), que cobre grandes áreas do nosso território, e para projetos menores com menor orçamento é recomendado o uso do [Cloudflare](https://www.cloudflare.com/pt-br/));**
5 - **Hospede seu site com implementações de segurança que garantam a conformidade com leis e entrega dos serviços sem maiores problemas para os usuários e seu negócio (um bom exemplo é o backup diário e uma boa administração do sistema do servidor, pense sempre na segurança do seu projeto);**
6 - **Avalie os recursos humanos disponíveis no projeto na hora de escolher um servidor de hospedagem. Para saber o nível de suporte necessário e entendimento do tipo de servidor a ser escolhido.**
