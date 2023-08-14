# Tag `canonical`

Você já pensou em situações onde precisamos ter conteúdos duplicados em nosso site? Nessas situações, devemos e precisamos informar isso ao Google.

Pois, como já citado e discutido em anotações anteriores, conteúdos duplicados são uma má prática e geram penalização. Então imagine, num e-commerce de sapatos, onde cada tamanho de um único sapato tem sua própria URL, o que se pode fazer quanto a isso?

É nesse ponto que a tag `canonical` entra em ação.

## Explicando melhor

No nosso exemplo imaginativo temos que o conteúdo teóricamente duplicado corresponde à tamanhos diferentes de um mesmo sapato, ou seja, são reconhecidas as URLs de cada tamanho do sapato como uma página duplicada, que repete os conteúdos.

Por isso, existe a tag `canonical`.

Mas do que ela se trata?

**A tag `canonical` é usada para indicarmos, no código fonte da página (no HTML), que esse é um conteúdo original. É utilizada para páginas que têm conteúdos parecidos ou iguais em diferentes URLs.**

Usando ela, dizemos ao Google que ao termos essa página duplicada por algum motivo, sabemos que seus conteúdos são replicados em outras URLs e é dela
que vem originalmente esse conteúdo.

Basicamente temos algumas páginas que são cópias que tem seu conteúdo sendo direcionado à uma página canonica, a original, a principal do conteúdo.

Vamos ver isso na prática agora.

## Exemplificando

Primariamente, entremos nesse link:<br>https://www.americanas.com.br/produto/3518043671?epar=bp_pl_px_go_pmax_edom_3p_linha_1_pa_2&voltagem=220V&condition=NEW

Podemos notar que, ao visualizar o código fonte da página, que a tag `canonical` aponta para o seguinte endereço:<br>https://www.americanas.com.br/produto/3518043671/geladeira-refrigerador-top-freezer-cor-inox-382l-electrolux-tf42s

Sem a query de voltagem na URL.

Isso ocorre pois os conteúdos das URLs com a voltagem geram URLs próprias e que replicam o conteúdo do produto, da sua página. Dessa forma, é necessário apontar por meio da `canonical` onde podemos encontrar o conteúdo original.

Podemos então, seguindo essa boa prática nesse casos de duplicação necessária dos conteúdos, direcionar e especificar para o Google o por quê dessa duplicação e onde encontrar a fonte original daquele conteúdo, evitando a penalização.

### Referência

Para podermos estudar de maneira mais aprofundada e implementar essa tag de forma correta, podemos ler o seguinte artigo do próprio Google:<br>https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls?hl=pt-br.
