# Indexabilidade do site: como funciona?

Entrando agora no Pilar de Tecnologia que citamos no módulo anterior, vamos poder entender como funciona cada uma das características e especificidades apontadas anteriormente.

Você já parou para pensar o que acontece desde o momento que o GoogleBot encontra seu site até seu site de fato aparecer nos buscadores?

## O que acontece até o aparecimento nas buscas?

O primeiro passo é a Interpretação, o GoogleBot entra no seu site e tenta entender o que está acontecendo, do que se trata seu conteúdo, arquitetura e aquela página acessada em específico. O GoogleBot tenta entender do que se está falando, quais as palavras-chave relevantes que estão sendo usadas, qual seu nicho.

A partir dessa "varredura" ele vai para a etapa de indexação, que é guardar o seu conteúdo junto dos outros conteúdos que ele já tem dentro da base de dados gigantesca que o Google possui afim de fazer um "mix" de outros sites de um mesmo nicho que o seu, de um mesmo setor, e então define um ranking entre essas páginas baseadas na Autoridade, Expertise e Confiança do seu site, artigo e página.

## Mais especificamente, o que ele faz?

No primeiro passo, ele, o GoogleBot, navega pelo seu site através de _linkagem interna_. O Crawler entra no site com o objetivo de passear, conhecer e encontrar mais páginas e mais conteúdos, navegando pelas páginas que são linkadas na própria página que está sendo lida. É como se ele "_scaneasse_" seu site.

Depois disso, vamos para a indexação, a catalogação da busca e análise feita. Entendendo do que se trata seu site, o GoogleBot guarda nas bases de dados as URLs separadas por nichos e essas páginas já ranqueadas ao lado de outros sites de um mesmo seguimento.

Dessa forma, ao realizar uma busca que contenha as palavras-chave e contexto relevante que possa nos levar à uma página como a nossa, a busca nos retorna uma SERP (Search Engine Result Page) que estrutura os resultados da busca baseados nos fatores já citados, as mostrando ordenadamente pelo ranking estabelecido no presente momento da busca.

## "Hacks" maneiros para encontrar conteúdos no Google

O primeiro seria utilizar `site:` antes de colocar uma URL de algum site. Isso nos mostrará as URLs dentro desse site que foram indexadas e que são mostradas em SERPs. E podemos separar a busca pelo domínio principal ou contar também com os resultados de seus subdomínios, exemplificando:

- `site:petlove.com.br`: nos retorna a SERP com todos as URLs indexadas do site, contando seus subdomínios;
- `site:https://www.petlove.com.br`: nos retorna a SERP com todas as URLs indexadas do site, sem contar subdomínios.

Também podemos pesquisar por `URL`:

- `site:petlove.com.br inurl:racao`: nos retorna as páginas da _petlove_ que tem na **URL** a palavra racao (que se refere à ração).

Isso é útil pois podemos descobrir se já há conteúdos em nossos sites que já abordam esse tópico, ou, por exemplo, ver como a concorrência aborda esses tópicos específicos.

Ou, se não conseguirmos buscar pela URL, podemos buscar pelo `title`:

- `site:petlove.com.br intitle:cachorro`: em vez de buscar pela URL, que muitas vezes está focada somente na palavra-chave, buscamos pelo título da página que possua _cachorro_, nos retornando tudo relacionado à páginas que possuam _cachorro_ no `title`.

De toda forma, mesmo sem usar ferramentas como Search Console ou SEMrush, podemos verificar se nossa página está indexada.
