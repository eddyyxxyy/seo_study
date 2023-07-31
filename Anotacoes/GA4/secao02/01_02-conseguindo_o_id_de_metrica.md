# Conseguindo o ID de Métrica

O objetivo dessa aula é conseguir o ID da Métrica e depois fazer a instalação em nosso site.

## O que fazer

O primeiro passo é acessar [analytics.google.com](https://analytics.google.com/) e, quando acessarmos o site, teremos de nos autenticar com uma conta do Google.

Então, já podemos clicar no botão de início, provavelmente escrito como "Começar a usar".

A partir desse ponto entramos na Criação de Contas, Propriedades, Detalhes Comerciais, Objetos de Negócio e Coleta de Dados.

### Criação de Contas

Não confunda essa conta que está sendo criada com a que utilizamos para logar na ferramenta.

Dentro do Analytics podemos criar configurações para diversos sites e aplicativos, cada site/aplicação tem o que chamamos de ID de Métrica que, como dito anteriormente, é o ID exclusivo que é usado para direcionar os dados da sua aplicação para o GA4. Esses IDs de Métrica ficam dentro de uma Propriedade.

Temos de organizar tudo isso dentro de uma conta, isso é obrigatório.

Na aba de "Detalhes de Conta", nós temos o "Nome da Conta", que é onde colocamos o nome da conta que terá acesso às Propriedades (sites/aplicativos) dessa conta em específico, com os respectivos IDs de Métrica de cada aplicação do dono da conta, podendo ser, por exemplo, um site de portfólio de um desenvolvedor como uma propriedade e um ecommerce de peças eletrônicas que também pertence à esse mesmo desenvolvedor.

Tudo isso é compartilhado com o próprio Google de forma anônima, em nível macro no ambiente que estamos criando a conta, uma vez que cada Propriedade tem suas configurações próprias com especificidades únicas muitas da vezes.

### Criação de Propriedades

Para medir os dados da Web e de Apps, criamos uma Propriedade para esse produto no GA4, que no caso seria o site em si, o site gerido pela conta criada anteriormente.

A Propriedade é o agrupamento de dados e relatórios de um único produto.

Damos um nome, definimos um Fuso Horário e Moeda.

### Detalhes Comerciais

Aqui definimos o setor e tamanho de nossa empresa.

### Objetivos de Negócio

O que selecionamos nessa etapa afeta diretamente o menu de "Relatórios" no Analytics, mas é algo que podemos personalizar posteriormente da forma que acharmos melhor.

É recomendado que, caso não haja certeza quanto aos seus "Objetivo de Negócio", que você marque a ultima opção: "Gerar relatórios de valor de referência".

### Finalização da criação de Conta/Propriedade

Agora, nessa ultima etapa de configuração básica, iremos conectar nossa Propriedade do GA4 com a plataforma da nossa aplicação, seja Web, App Android ou App iOS.

Nos é mostrado a configuração do Fluxo de Dados específico para cada tipo de aplicação, dessa forma podemos preencher as informações necessárias para criar a conexão entre a ferramenta do GA4 e nossos produtos.

Algo a se notar na criação do Fluxo de Dados para aplicações Web, para sites, é que temos como habilitar a "Métrica Otimizada".

#### Métrica Otimizada

Por padrão é algo que já vem marcado como aceito e, como já sabemos, tudo no Google Analytics 4 é feito por meio de Eventos e Parâmetros e a "Métrica Otimizada" se trata justamente dos Eventos com os Parâmetros padrões que citamos anteriormente em outras anotações e, por conseguinte, é algo essencial para a implementação do nosso ID de Métrica, uma vez que não precisaremos configurar esses eventos que já vem por padrão em nossa Propriedade por meio de código ou pelo GTM (Google Tag Manager).

> Ainda podemos desativar alguns eventos ao personalizar e podemos fazer ainda mais, como definir parâmetros específicos de alguns eventos padrões para atender à nossas necessidades.

Ao terminar de configurar o que deseja, é só clicar em "Criar Fluxo" e teremos gerado o ID da Métrica da sua Propriedade e as instruções para que se instale a Tag (os códigos) no site.

Existem duas formas de fazer essa instalação:

- Manualmente: replicando o código em cada uma de suas páginas e;
- GTM: replicando o código do GTM em cada uma de suas páginas.

> Pelo GA4 ser uma ferramenta nova e uma aplicação Web, muitos recursos podem estar posicionados em outro lugar do que os apresentados aqui ou no curso de acompanhamento.
