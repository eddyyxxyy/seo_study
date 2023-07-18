# Como o Google Analytics 4 funciona?

É essencial que você tenha esse conhecimento antes de colocar a mão na massa, então veremos em detalhes.

## O básico

Ao acessar o GA4, temos por padrão a visualização da aba Página Inicial, acesse a aba de Relatórios e você se deparará com o "Resumo dos Relatórios".

Nessa página teremos respostas rápidas e esses dados vem de um site previamente configurado, isso se houve configuração. Dessa forma, podemos saber a quantidade de usuários que acessaram nosso site e quantos desses usuários são novos, podemos verificar também seu tempo de engajamento e como eles chegaram até nosso site, se foi por tráfego pago ou orgânico, por exemplo.

Também podemos ver até da onde o usuário está acessando, de qual país; podemos verificar as páginas mais acessadas de um site ou telas mais acessadas de um aplicativo mobile, entre muitos outros detalhes.

Já em "Tempo Real", a aba abaixo do "Resumo dos Relatórios", podemos verificar as pessoas que estão agora acessando nosso site ou app, mas somente as que estiveram nos ultimos 30 minutos. Sempre que uma pessoa acessa o site/app, um código é executado e os dados são enviados para o Analytics, esse código o usuário não vê, mas está presente no código fonte de nossos sites/aplicações.

Para atingir isso, esse envio dos dados por parte do código para o GA4, precisamos colocar a tag/comando respectivo em todas as páginas de nosso site. Como iremos colocar esse código no site/app depende da tecnologia que utilizamos e quais ferramentas escolhemos trabalhar, mas independente disso, o funcionamento e direção dada pelo curso é suficiente para que se saiba tomar as melhores decisões na hora de fazer sua implementação.

### Sobre os IDs de métricas

Independente do que aconteça, teremos um ID de Métrica. Esse ID é exclusivo e é graças à ele, aliado ao código que colocamos nas páginas de nosso site, que mandamos os dados para nossa Propriedade do GA4.

Com os dados enviados para o GA4, a ferramenta irá transformar os dados em informações úteis através de relatórios, como os citados brevemente na sessão anterior.

Tudo isso é feito através de Eventos e Parâmetros, por exemplo: quando alguém acessa a página do nosso site, automaticamente um evento chamado "page_view" é coletado pelo GA4 através do código colocado em nosso site e enviado para a Propriedade correta através do ID de Métrica. Ou, também, quando o usuário realiza o _scroll_ da tela (geralmente 90% da página), um evento chamado "scroll" é enviado para a Propriedade e, como podemos notar, temos diversos eventos que vão desde o scroll da tela, a visualização da página, clicks em links externos na página, entre outros.

Esses eventos são coletados de maneira automática, mas isso não nos impede de criar e personalizar nossos próprios eventos, por conseguinte, nós temos a possibilidade de atender a qualquer necessidade que tenhamos ao criar novos eventos.

### Mais sobre Eventos e Parâmetros

Junto aos Eventos são enviados os Parâmetros.

Os Parâmetros servem para detalhar o evento, ou seja, caso acessemos o evento "click", teremos uma visualização de diversas informações como: qual link foi acessado, qual o domínio do link acessado, em qual página aconteceu esse click, entre outros mais.

Esses dados obtidos através dos Eventos e detalhados pelos Parâmetros são transformados em relatórios pelo GA4, isso se contarmos com os relatórios padrões, feitos automaticamente pela própria ferramenta. Uma vez que entendemos esse funcionamento podemos utilizar o GA4 para criar relatórios próprios dentro da aba "Explorar", relatórios estes que serão mais avançados e personalizados por nós arrastando métricas e dimensões.

As dimensões são as perspectivas de análises e as métricas são aquilo que quero mensurar, como por exemplo: gerar um relatório de quantos usuários, novos e ativos, tem acessado nosso site à partir de algum dispositivo específico (Desktop, Mobile ou outros). E todos esses relatórios levam em conta um período, seja de dias, semanas, meses ou anos.

## Como o GA4 sabe o que é um usuário, quem é novo e outros detalhes?

Hoje, o GA4 trabalha com três formas de identificação, a mais usada e padrão é a chamada de "Identificação por Dispositivo", ou seja, a ferramenta nunca identifica uma pessoa, mas sim o dispositivo usado por ela (mesmo que seja um bot). Dessa forma, acessando o site desejado que está metrificado pelo GA4, é gerado um cookie (um dado temporário que pode se alterar com o tempo, pela troca de navegador ou o uso de alguma tecnologia externa) que identifica o usuário e "lembra" dele quando o site for acessado novamente por esse usuário específico, pois seu Client ID está gravado, logo o acesso não é de um usuário novo.

A segunda forma é chamada de "User ID", que é uma maneira que consegue manter a jornada do usuário entre dispositivos e navegadores, uma vez que esta atrelado à um sistema de login e senha, sempre que o usuário for utilizar um site de _ecommerce_ e se autenticar, ele terá o seu acesso "trackeado" (rastreado) e identificado pelo seu User ID.

A terceira forma é pelo Google Signals, personalização de anúncios e conta do Google. Então mesmo que não tenhamos a possibilidade de utilizar um User ID para manter os dados mais coesos, o GA4 nos trás mais essa maneira de trabalhar que é independe de cookies. Por exemplo, sua conta do Google que está logada no seu computador, smartphone e outros dispositivos, atrela seus dados à um único usuário e pode identificar melhor os usuários do seu site.

> Porém, sobre a terceira forma, o usuário deve ter ativado em suas Configurações de Conta, na aba de "Dados e personalização", a opção de "Personalização de Anúncios" e, também, o site precisa ter muitos acessos.

Em suma, o que temos de mais concreto para manter a jornada do usuário de forma geral é o User ID.

__Lembre-se: _TUDO_ no GA4 é feito por meio de _Eventos_ e _Parâmetros_.__
