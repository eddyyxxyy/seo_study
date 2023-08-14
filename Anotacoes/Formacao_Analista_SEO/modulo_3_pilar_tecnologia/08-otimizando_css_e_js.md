# Otimizando CSS e JavaScript

## Fundamentos

**O que é CSS?**

Cascading Style Sheets (CSS) é um mecanismo para adicionar estilos a um documento Web (ao HTML, a uma página).

**O que é JavaScript?**

JavaScript (JS) é uma linguagem de programação de alto nível, que permite a criação de itens complexos e dinâmicos em páginas web. Essa tecnologia faz com que as páginas deixem de ser estáticas e permitem maior interação do usuário.

> O CSS, assim como o HTML, não é considerado uma linguagem de programação, mas sim, respectivamente, um mecanimos de estilização de páginas e uma linguagem de marcação.

### Processamento Client-Side

Contextualizando a terminologia utilizada, o client-side se trata do lado do cliente, de quem acessa o site, seria o processamento feito no navegador e na máquina do usuário que requisita, acessa e navega pelo site. O server-side seria o processamento que se dá no servidor, em quem provê o site que foi requisitado pelo usuário, todo o processamento crítico da aplicação, por motivos de segurança e muitos outros aspectos, é feito na máquina provedora do site/serviço.

Para visualizarmos esse processamento client-side de forma sequêncial, atente-se:

1 - Usuário faz uma requisição que leva ao nosso site (www.seusite.com.br);
2 - O servidor recebe e valida essa requisição, somente então envia os arquivos HTML, CSS e JS;
3 - O navegador que está sendo usado para acessar o site baixa os arquivos HTML, CSS e JS, normalmente nesta ordem;
4 - O navegador executa a biblioteca ou framework usado (se estiver presente na implementação do site);
5 - O navegador de fato carrega o site.

### Código Semântico

Um Código Semântico é aquele que reflete em seus elementos, variáveis e expressões a conformidade com seu prévio significado. Mas o quê isso significa? Se trata de utilizar nomes que tenham real significado, que reflitam do que se trata o elemento manipulado na linguagem de programação/marcação (JS e HTML).

O Código Semântico é claro, objetivo, porém cheio de significado dentro do possível naquele contexto. Por exemplo, quando colocamos um código de `header` sabemos que se trata do cabeçalho da página, quando colocamos `footer`, sabemos que é o rodapé da página, quando colocamos `h1`, `h2`, `h3`, `h4`, sabemos que são cabeçalhos e o nível de hierarquia entre eles dentro do conteúdo.

Existem alguns códigos como `div`, `span`, que são genéricos, que não dizem nada especialmente, mas que podem sim expressar algum significado pelo seu conteúdo ou classe utilizada.

O World Wide Web Consortium é a principal organização de **padronização da World Wide Web**. Consiste em um consórcio internacional com 450 membros, agregando empresas, orgãos governamentais e organizações independentes com a finalidade de estabelecer padrões para a criação e a interpretação de conteúdo para a Web.

> Validador de HTML e CSS da W3C: https://validator.w3.org/ <br>Cursos Gratuitos Online da W3C: https://www.w3schools.com/

Vale ressaltar que as DevTools de navegadores são o melhor lugar para começar a validar seus códigos CSS e JS: inicie pelo menu do seu navegador ou aperte `F12` (na maioria dos navedores abre as DevTools).

> Referência sobre as DevTools e SEO na prática: https://searchengineland.com/chromes-devtools-seo-10-ways-use-seo-audits-266433 <br>Muitas vezes, as DevTools te trazem de forma melhor como otimizar o HTML, JS e CSS do que ferramentas de análise de performance.

## Otimização a entrega dos arquivos

Uma das formas de otimizarmos a entrega dos arquivos requisitados pelos navegadores de usuário é utilizando o HTTP/2, que é uma versão nova do protocolo HTTP/1.1, sendo esteS protocolos os utilizados amplamente pela internet para servidores e sites. Ou seja, utlizar por padrão cabeçalhos HTTP/2 permite a conversa padrozinada entre cliente, geralmente navegadores, e servidor, que é onde ficam armazenados os conteúdos enviados quando um site é acessado.

> Site para aprender a implementar HTTP/2: https://www.practicalecommerce.com/enable-http2-happier-customers-better-seo

A versão 2 do protocolo HTTP tem o processamento assíncrono por padrão, que carrega as coisas aos poucos, já a versão 1.1 carrega os arquivos por meio de filas.

**Vantagens do HTTP/2**:

- Melhor desempenho;
- Latência reduzida;
- Permite solicitações paralelas com carregamento rápido;
- Melhor sobrecarga sem precisar fazer grandes alterações no seu site;
- Navegue até as ferramentas de desenvolvedores do seu navegador (DevTools) e observe a aba "Network" ("Redes") e verifique se o protocolo utilizado nas requisições são da versão desejada. Tente mudar tudo para ao menos a versão 2, visto que a versão 3 pode ainda não ser suportada por alguns navegadores.
- Ferramenta online para teste de protocolo: https://tools.keycdn.com/http2-test.

O impacto é **grande** em relação à performance, então considere utilizar os protocolos mais utualizados, pois processar as requisições neles, além de trazer maior desempenho, nos traz maior segurança e confiabilidade, aos olhos dos usuários (que terão melhor experiência) e aos "olhos" das Search Engines que verão a diferença de performance no seu site com as mudanças feitas, além de trazer o quesito de confiança maior devido a maior segurança.

**CDN (Content Delivery Network)**

CDN é a abreviação em inglês de Rede de Distribuição de Conteúdo, que é uma rede de servidores (pontos de presença) que armazenam cópias do seu conteúdo no cache e depois os entrega aos usuários de acordo com a localização geográfica, entregando os conteúdos à partir de um ponto de presença mais próximo ao usuário, reduzindo a latência (tempo de resposta) na transferência de dados para atender à requisição do usuário.

## Combinar x Minificar

Os dois termos dessa seção se referem à tecnicas para lidar com a qualidade/quantidade de código em uma aplicação, em um site, e o ideal é que se use um ou outro, não deve-se, por exemplo, ativar ambas as opções em um CMS WordPress com os plugins de performance que são utilizados, pois a chance de gerar erros ou resultado nenhum é grande.

Existem situações que podemos ter uso melhor da combinação de arquivos, juntá-los, e situações que é melhor simplesmente minificar os arquivos. É recomendado que seja evitado ao máximo e somente se o HTTP não seja da versão 2 (seja por qualquer motivo que se esteja utilizando o HTTP/1.1), se utilize da combinação de arquivos. Isso é algo a se considerar pois o HTTP/1.1 trata das requisições por filas, um a um, mas um site de HTTP/2 tem a assincronia como sua principal aliada e a combinação **desperdiça** o poder dessa tecnologia.

Exemplificando:

**Combinar**:

- Carregamento lento e desperdício dos recursos do HTTP/2;
- Potencial crítico de quebrar o site ao juntar conteúdos em um único arquivo;
- Carregamento de elementos desnecessário.

_Sendo utilizado somente se:_

- Seu site utiliza HTTP/1.1;
- Você tem um site simples sem muitos scripts e estilos.

**Minificar**:

- A maioria das ferramentas de criação e manutenção de sites permitem que você otimize seu CSS e JS removendo espaços em branco, comentários, indentações e caracteres desnecessários;
- Em temos de impacto, a minificação pode não trazer benefícios consideráveis se você tem o GZIP ativado no servidor. Porém, não há nenhuma desvantagem (diferentemente da técnica de combinar arquivos).

> Dica de ferramente para minificação de documentos CSS ou JS: https://www.minifier.org/.

## Defer x Async

Há duas formas de declarar as tags `script` em nosso código HTML, que se tratam dos atributos `defer` e `async`.

> Link de referência sobre os atributos: https://javascript.info/script-async-defer.

**`defer`**:

O atributo `defer` diz ao navegador para não esperar pelo script enquanto carrega a página. Em vez de esperar pelo carregamento do script para continuar lendo os conteúdos abaixo dele, o navegador continuará processando o HTML, construindo a DOM.

O script carrega "em segundo plano" e, em seguida, é executado quando a DOM é totalmente contruída.

Você DEVE usar `defer` quando seu script exigir que o carregamento do HTML já tenha ocorrido.

```html
<script defer src="script.js"></script>
```

**`async`**:

O atributo `async` significa que um script é completamente independente.

Com esse atributo, o arquivo é baixado de forma assíncrona e executado assim que é baixado (não espera todo o conteúdo carregar antes como o `defer`).

Use o `async` sempre que possível, ele costuma ser melhor e evita o bloqueio de renderização da página.

```html
<script async src="script.js"></script>
```

## CSS: otimizando e algumas dicas

**Quando puder substituir imagens por CSS, FAÇA ISSO!**

- Bordas;
- Sombras;
- Gradientes;
- Formas geométricas.

É melhor ter detalhes como esses em CSS do que em imagens dentro da página.

**Quando usar animações e efeitos na página, USE CSS!**

As transições e animações CSS nativas sempre serão mais rápidas do que os efeitos baseados em JavaScript.

> As animações CSS não funcionarão em navegadores mais antigos, como o IE9 e anteriores.

**Não anime algumas propriedades críticas!**

Animar as dimenções ou a posição de um elemento pode fazer com que toda a página seja reformulada em cada quadro (prejudicando o seu site com CLS).

Quando quiser um efeito parecido, use as propriedades CSS `opacity` e `transform`.

**Simplifique os seletores!**

Menos é mais. Trabalhe o estilo do seu site com seletores simples e práticos.

Facilite o processamento e renderização dos estilos e animações dos elementos para o navegador e bots das Search Engines.

```css
/* Tente evitar isso, use seletores de forma mais simples, se for possível. */
body > main.xpto > section.first
h3:nth-of-type(odd) + p::before >
a[href$=".xml"]
```

**Evite o uso de propriedades que causem o recálculo no carregamento da página!**

Propriedades como:

- `border-radius`;
- `box-shadow`;
- `opacity`;
- `transform`;
- `filter`;
- `position:fixed`;
- entre outras...

Intereferem bastante no carregamento da página, podendo causar CLS se usados em abundância. De uma forma geral, evite utilizar essas propriedades no CSS, o branding é super importante e criar uma identidade para suas páginas é essencial, mas nunca é demais o uso parcimonioso de propriedades que podem afetar diretamente nosso ranqueamento à custo de uma suposta estética idealizada.

**Utilize a propriedade `will-change`!**

A propriedade `will-change` permite que você indique que um elemento será animado (e com este sinal o navegador faz otimizações para melhorar o desempenho com antecedência). Por exemplo, para declarar um elemento que será transformado.

```css
will-change: auto;
will-change: scroll-position;
will-change: contents;
will-change: transform;
will-change: opacity;
will-change: left, top;
```

> Link de referência sobre a propriedade: https://developer.mozilla.org/en-US/docs/Web/CSS/will-change.

**Considere colocar CSS crítico "in-line"!**

Mais uma vez podemos salientar a importância das DevTools dos navegadores, pois por ela também podemos verificar os arquivos CSS críticos que estão presentes na página. O CSS crítico se trata das estilizações mais importantes do seu site e por isso é sempre bom ter essa atenção na implementação desses detalhes. Sempre faça:

- Extração dos estilos usados para renderizar elementos acima da dobra;
- Adicione-os a um elemento `<style>` no `<head>` do HTML;
- Carregue o arquivo CSS principal de forma assíncrona.

```html
<html>
  <head>
    <title>Exemplo de CSS in-line</title>
    <style>
      p {
        color: afff;
        text-decoration: underline;
      }
    </style>
  </head>
  <body>
    <p>Olá!</p>
  </body>
</html>
```

> Artigo sobre manutenção de CSS crítico em WordPress: https://10web.io/blog/inline-critical-css-defer-unused-css-wordpress/.

**Style Guide: ter clareza do design!**

Ter clareza do design do seu site e marca ajudam a evitar "sujeiras" no seu código CSS, o que contribui para um código mais limpo, coerente, performático e de melhor manutenção. Com um style guide (ou design system) definido, conseguimos padrozinar:

- Cores e tipografia;
- Estilo de botões;
- Regras de padding, grids e breakpoints;
- Etc...

> Exemplo de design system: https://boltdesignsystem.com.<br>Ferramenta que ajuda a montar design systems: https://patternlab.io/.

**Separe seus estilos, ganhe eficiência e "faxine" seus arquivos CSS!**

Ao separar os arquivos CSS (_Code Spliting_), identificar seus componentes e manter os que ainda estão em uso fica fácil, deixando-nos com maior abertura para descartar o restante (os componentes não mais utilizados ou de alguma forma irrelevantes).

Além disso, permite carregar o CSS necessário para cada página e geralmente de forma assíncrona.

```html
<link rel="stylesheet" href="principal.css" />
<link rel="stylesheet" href="checkout.css" />
<link rel="stylesheet" href="carousel.css" />
```

Geralmente os estilos de uma `navbar`, `footer` e outros elementos que aparecem em praticamente todas as páginas, são colocados em um arquivo CSS, enquanto os outros mais específicos são divididos e colocados em arquivos diferentes, que façam mais sentido pertencer.

**Evite o uso da declaração `!important`!**

A declaração `!important` é antipadrão (apesar de estar disponível para uso). Normalmente é usada quando algo não está funcionando como deveria, para forçar o estilo no elemento.

O problema é que ele é usado de forma excessiva na maioria das vezes e a causa real do design ruim não é de fato resolvida.

Essa declaração deixa o código sujo, uma colcha de retalhos e com a possibilidade de gerar ainda mais bugs no futuro.

```css
h4 {
  font-style: bold;
  color: #fff;
}

.bloco2 h4 {
  font-style: italic !important;
  color: #b5cf54 !important;
}
```

O ideal é que construamos o CSS de forma consciente e que funcione em todo nosso site sem o uso de "gambiarras" para seu funcionamento, sem usar o `!important`, ele é a ultima instância, em casos específicos.

## JS: otimizando e algumas dicas

**Usando Web Woker.**

Arquivos JS custam mais no carregamento que imagens e fontes com o mesmo "peso". Além de consumirmos mais CPU e memória do seu servidor e cliente.

Web Workers permitem que você execute os arquivos JavaScript mais críticos em uma thread em segundo plano, para que sua thread principal permaneça desbloqueada e carregue bem mais rápido e melhor para o usuário.

> Referências: https://web.dev/workers-overview/ e https://research.mozilla.org/2014/07/22/webgl-in-web-workers-today-and-faster-than-expected/.

O que mais impacta no desempenho de arquivos JS é o uso de CDN, os atributos `defer` e `async` e combinação ou minificação dos arquivos, mas é muito específico do JS o uso do Web Worker.

Enquanto a página carrega os elementos dela, pegariamos os scripts JS e carregariamos em segundo plano, permitindo que tudo carregue sem impedir o processamento em nenhuma das partes, o Web Worker isola o processamento dos scripts do processamento da página e estilos, sem impactar na performance da página.

Para termos uma ideia, o serviço de CDN da Cloudflare tem provê Web Workers, mas precisamos pagar para que esse processamento do JavaScript seja feito e temos outros serviços de CDN que tem Workers integrados. Devemos nos atentar se podemos contratar ou simplesmente integrar o uso de Web Workers em nossa aplicação para que o desempenho de scripts seja mais coerente e uniforme.

**Otimize a entrega de scripts de terceiros!**

Os scripts de terceiros, que são códigos incorporados no seu site, competem com seu próprio código pelo uso do poder de processamento da thread principal do navegador, o que atrasa a renderização dos conteúdos.

Além do `defer` e `async` podemos utilizar a solução de código aberto Partytown, que é um builder, uma API, que faz essa função de Web Worker com os scripts de terceiros, que não seus. Para scripts críticos, prefira utilizar scripts próprios que possam ser processados pelo servidor através de um CDN para evitar bugs e problemas.

Também podemos colocar um `delay` no carregamento dos scripts de terceiros, sempre lembrando do `defer` e `async`.

**Separe seus scripts e ganhe eficiência e "cleanness" no seus códigos JS!**

Mais uma vez nos referindo ao Code Spliting que, ao separar os arquivos JS (assim como nos CSS), nos ajudam a identificar seus componentes e melhora a manutenção das suas implementações, também trazendo maior qualidade para seu site em termos de performance.

Além disso, permite carregar somente o script que vai ser usado em cada página.

Antigamente, existia um mito que dizia que devemos diminuir o número de requisições a todo custo e, por isso, quando os desenvolvedores veem diversos arquivos com funções diferentes em abundância, já ficam incomodados e pensam ser uma prática errada, mas quando vemos que os dados de performance podemos notar que o número de requisições não é o que realmente faz diferença, o que faz diferença é carregar o que realmente importa para a página.

Otimizar a performance não tem a ver com diminuir o número de requisições, mas sim com constriur páginas com somente o necessário, com as chamadas corretas para criar a visualização e funcionalidade exata que precisamos.

**Opção de renderização otimizadas para JS e/ou site SPA (Single Page Application) como React e Angular!**

Server Side Rendering (SSR) pega todos os arquivos JS que normalmente são carregados no browser (client-side) e renderiza de forma estática no lado do servidor.

A renderização dinâmica requer que seu servidor detecte rastreadores (User Agents). Quando a solicitação for de rastreador são encaminhadas para um renderizador e solicitação de usuários são veiculadas normalmente.

Ou seja, separamos a renderização baseada no tipo de requisidor. Quando a requisição for de um usuário, manteremos o processamento dinâmico para entregar a melhor experiência para o usuário, quando forem feitas por rastreadores (como bots do Google), encaminharemos a requisição para o processamento estático SSR, no servidor.

> Referências: <br>[JavaScript: SEO Mythbusting com Martin Splitt e Jamie Alberico](https://www.youtube.com/watch?v=jwgnwtQcSWQ&list=PLKoqnv2vTMUN6lFDz6qMBsz7-Jm8YRV9H)<br>[Google I/O '18 com Tom Greenway](https://www.youtube.com/watch?v=PFwUbgvpdaQ)

## Ferramentas de Performance

Iremos enumerar agora diversas ferramentas para medição e análise de performance:

- [Merkle](https://technicalseo.com/tools/):
  - Destacando as ferramentas de Render e Pre-Render.
- [Smartlook](https://www.smartlook.com/);
  - Ferramenta para análise de comportamento de usuários dentro do site.
- [SEO Pro Extension](https://chrome.google.com/webstore/detail/seo-pro-extension/lajfdngpocmchpihjecojjllfjeehgnl):
  - É a extensão do Chrome que é completinha, que traz o `title`, `cannonical`, e outras métricas do Core Web Vitals.
- [Bing webmaster](https://www.bing.com/webmasters/about);
- [Semrush](https://pt.semrush.com/);
- [WebPageTest](https://www.webpagetest.org/);
- [Google PageSpeed](https://pagespeed.web.dev/);
- [Dareboost](https://www.dareboost.com/en);
  - Essa ferramenta foi comprada e provavelmente sairá do mercado;
  - Foi considerada por muitos a melhor ferramenta para otimizar arquivos JS e CSS "no detalhe".
- [GTmetrix](https://gtmetrix.com/).

> Artigo com diversas soluções gratuitas para otimização de CSS e JS: https://wp-rocket.me/blog/best-free-css-and-javascript-minification-tools/.
