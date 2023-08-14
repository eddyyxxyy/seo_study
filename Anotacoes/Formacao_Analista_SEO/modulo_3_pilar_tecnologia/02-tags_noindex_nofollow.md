# Tags _noindex_ e _nofollow_

Pense no seguinte cenário:

Imagine cada URL que um site como a americanas.com consegue criar a cada filtro, a cada categoria, a cada parte do site que vai se combinando e sendo indexada. A quantidade de URLs é muito grande, muito mesmo.

O que vamos aprender agora são as tags que nos auxiliam a controlar, gerir, esse tipo de situação. Fazer a gestão das páginas que queremos que sejam indexadas ou não é essencial, pois, mesmo que o Google já não indexe automaticamente páginas que necessitem de login para serem vistas, existem páginas como a de contato que não precisam e geralmente não devem estar indexadas, pois o foco das nossas aplicações web é atrair usuários pelo conteúdo, produtos e serviços que oferecemos.

Nós queremos converter cliques em vendas, em assinaturas, em consumo de conteúdo que possa a levar os usuários à clicar em nossos anúncios e produtos, esse é nosso foco.

## _noindex_

Comunica aos buscadores que não é para incluir na indexação determinada página, para não as incluir nas páginas de resultados dos mecanismos de buscas, para não as incluir nas SERPs.

Os motivos são variados para se utilizar a tag _noindex_, mas geralmente se trata de manter somente o que é realmente relevante para seu negócio, seu nicho, indexado nos mecanismos de buscas.

## _nofollow_

Comunica aos buscadores para não seguirem os links que estão na página em questão.

Por exemplo, se estamos linkando conteúdos nessa página que não são relevantes para seu negócio, adicionamos essa tag para dizer ao buscador para não acessar esses links.

## A estrutura disso

O que está acontecendo no código HTML abaixo?

```html
<meta name="robots" content="follow,index" />
```

A abertura da _meta_ tag em HTML sinaliza a criação de um metadado estruturado para páginas web, ela fica no _header_ do HTML das páginas. As _meta_ tags são trechos de texto que descrevem o conteúdo e propósito das páginas.

O campo _name_ especifica que **robots** deve seguir as diretivas dadas no campo _content_, pois "robots" referência à todos os bots de mecanismos de buscas.

O campo _content_ é literalmente o conteúdo da _meta_ tag e contém as diretivas, os "comandos" que os **robots** devem seguir.

As diretivas _"follow,index"_ são os comandos em si, as diretivas de indexação, os comandos que serão seguidos pelo GoogleBot ou outros bots de mecanismos de buscas (que no nosso caso, são contrárias às que citamos, pois diz ao bot que siga os links disponíveis na página e indexe a página em si).

Em suma, o que está ocorrendo aqui é:

**Todos os Crawlers (sendo referenciados por "_robots_"), sigam os links disponíveis na página e também indexem essa página.**

## Uma ferramenta para enxergar isso melhor

Podemos adicionar uma extensão no Google Chrome para nos auxiliar a ver isso na prática.

O Seerobots analisa as páginas acessadas (se o acesso ao robots por permitido pelo site) e nos diz quais _meta_ tags estão sendo utilizadas.

Enquanto que na categoria "Celulares e Smartphones" da americanas.com temos as tags _index e follow_, quando filtramos a busca dessa categoria com "Capas de Celulares", temos agora que o uso das _meta_ tags citadas mudou, agora está como _noindex e follow_, pois não interessa à Americanas indexar essa página, mesmo que o bot possa seguir por ela e a analisar e guardar pelos links disponíveis na página, pois o foco dessa categoria é indexar justamente a busca completa de "Celulares e Smartphones.

Se a Americanas indexasse as páginas geradas de cada um dos filtros em cada uma das suas categorias de produtos, teriamos a indexação de tantas páginas que o real interesse da empresa poderia se perder entre as SERPs geradas pelos mecanismos de buscas. O ideal é ser enxuto, na medida do possível, para ser coerente com a indexação que mais agregue valor e conversão ao seu negócio.
