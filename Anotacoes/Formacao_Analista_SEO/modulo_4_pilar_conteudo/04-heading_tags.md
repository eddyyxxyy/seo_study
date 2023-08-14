# Heading Tags

Agora que já falamos sobre as tags `title` e `meta description`, iremos falar sobre outras tags super relevantes quando falamos de SEO, que são as `heading tags`.

## Header: tag de cabeçalho

Header vem de cabeçalho, é o cabeçalho do seu conteúdo, que separa as sessões como em um texto mesmo, com títulos e tópicos.

Para entender isso um pouco melhor e irmos direto ao ponto, aqui está a representação em HTML das `heading tags`:

```html
<h1>Terra</h1>

<h2>Europa</h2>
<h3>Espanha</h3>
<h3>França</h3>

<h2>América</h2>
<h3>América do Sul</h3>
<h4>Brasil</h4>
<h5>São Paulo</h5>
<h6>Campos do Jordão</h6>
<h4>Bolívia</h4>
<h4>Argentina</h4>
<h3>América do Norte</h3>

<h2>Ásia</h2>
```

Nesse exemplo hipotético, é como se o nosso mundo fosse estruturado dentro de `heading tags`, onde o tema principal é a Terra, o `h1`, o "título" (o elemento mais importante do seu conteúdo), e os continentes são os `h2` ou "tópicos" (o segundo mais importante do seu conteúdo), e prosseguimos até um nível máximo de `h6`, que seria a menor `heading tag` que temos.

Quanto mais quebramos os elementos, mais fundo descemos na hierarquia de importância e especificade do conteúdo abordado, independente de qual seja o assunto. Dessa forma, podemos concluir que para inserirmos a Oceania precisariamos colocá-la em um `h2` e o país Austrália abaixo do `h2` da Oceania entre as tags `h3`.

Essa estrutura, como dito anteriormente, caracteriza que tópicos estão dentro de outros e que todos eles estão encapsulados dentro de um assunto que os contém, que os envolve num mesmo tema.

Em suma, as `heading tags` são usadas para disponibilizar de maneira estruturada o seu conteúdo, onde pode-se entender o título/assunto, tópicos e subtópicos abordados e onde cada um deles se encaixa, existe a noção de pertencimento para cada elemento.

### Você pode estar se perguntando, qual a diferença entre a title tag e o h1?

Apesar de muito parecidos, o `h1` e a `title tag` são tags que desempenham papéis diferentes.

O `h1` é um título de um post ou página do seu site que está aparecendo no próprio site, na própria página. Já a `title tag` aparece como título da página para o navegador, na aba do navegador, e para os buscadores, os mecanismos de buscas.

Na `title tag` é ideal que sempre tenhamos o nome da marca ou site, fazendo o usuário identificar mais facilmente o site que está acessando. Vamos a um exemplo para que fique mais claro, utilizando uma página hipotética que fala sobre SEO:

```html
<title>Saiba tudo sobre SEO, dias e mais - Nome da Marca</title>
<h1>O que é SEO? Tudo sobre otimização para mecanismos de busca</h1>
```

### Dica de ouro!

Instale a extensão do Chrome chamada [MozBar](https://chrome.google.com/webstore/detail/mozbar/eakacpaijcpapndcfffdgphdiccmpknp?hl=en). Essa extensão permite que você veja o `title` e a `description` de qualquer página, assim como as `heading tags` e outras coisas mais.
