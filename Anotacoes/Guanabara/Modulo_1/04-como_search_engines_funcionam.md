# Como funciona o Google e outros buscadores?

## O que vamos abordar hoje

Os resultados de nossas pesquisas é de fato impressionante, temos a facilidade de acessar um site como o Google, inserir poucas letras e ter como reposta uma lista complexa, porém objetiva e confortável para o usuário final, de todos os conteúdos realmente relevantes para minha consulta, para meu uso. Mas como isso funciona? Como esses resultados se adequam à minha necessidade?

O objetivo aqui é, além de conhecer esse tópico, realmente entender como esses buscadores nos trazem tanta facilidade, praticidade, realizando consultas complexas em bases de dados que retornam resultados adaptados para nossa realidade, que coincidem com a nossa necessidade naquela busca. Como um encanador sabe de forma técnica e intuitiva o que fazer ao analisar por um breve momento algum problema? Sabendo de onde, por que e como as coisas que tem essa finalidade operam, existem.

## Funcionamento dos Motores de Busca

Pensemos então:

De um lado temos a Internet e de outro os usuários, que são as pessoas que estão buscando sites. Como um mecanismo de busca apresenta sites a uma pessoa? Como, por exemplo, tendo construído um site, uma loja virtual, uma página, etc, como esse site vai parar no Google?

Existem diversas formas desses sites "irem parar" no Google, quando utilizamos WordPress e algum plugin como o Yoast ou Rank Math já temos um "aviso" para o Google gerado por esses plugins. Caso façamos um site em html e não tenham links em nenhum lugar do mundo que leve até esse site, o Google não irá saber indexar essa URL, o site, temos de ir até o Google e informar "onde" se encontra nosso site (ou seja, utilizando WordPress já temos isso, pois o Google tem de ser informado sobre o site, pois ele não sabe que existimos).

Tendo essa conciência, o Google possui uma inteligência bem sofisticada de pré-processar essas informações e as guardar numa base de dados. Quando pensamos no buscador, temos de ter em mente de que não se trata de somente um algoritmo, são conjuntos de algoritmos que tem suas funções bem definidas trabalhando em uníssono; um conjunto que faz toda essa coleta de dados, outro conjunto que nos dá os resultados na hora da busca, dentro de cada um deles temos diversas rotinas e interconexão entre elas, são sistemas completos para cada parte. O nome genérico à esses sistemas e algoritmos é GoogleBot, sistemas e algoritmos estes que fazem o **Rastreamento, Classificação e Armazenamento**. O rastreamento acontece a partir do momento que o Google sabe que seu site existe, para que ele possa ler todo o conteúdo do site (ou, ao menos aquilo que for legível ao algoritmo; iremos aprender à construir sites assim), então classifica esses dados e os armazena numa base de dados de forma eficiente, para que, quando ele precise voltar, ele compare os dados que ele tem com o site no momento atual. Até esse ponto o usuário não fez nenhuma busca.

Nesse momento temos um índice no banco de dados dos servidores do Google que contém esses dados sobre nossos sites junto de outros sites, já classificados e organizados. O sistema que procura nesse índice é o **Sistema de Busca**, é aquele que busca no banco de dados os dados pertinentes àquela busca e usa fatores de ranqueamento para exibir em ordem os melhores resultados. Quando entramos no Google e pesquisamos algo, é nesse sistema que estramos (Sistema de Busca), que não é o GoogleBot, e para isso poder rolar o teu site deveria já ter sido "capturado" pelo GoogleBot.

Esses fatores de ranqueamento definem muita coisa em nossas buscas, um dos fatores vigentes é o de Geolocalização. Por exemplo, dependendo de onde estamos realizando a busca, teremos um resultado diferente para cada região, um resultado que atenda mais às necessidades daquela localidade.

### Rastreamento e Classificação

#### Os buscadores coletam os dados previamente

Os buscadores utilizam de softwares para rastrear e classificar os sites na Internet. Citando alguns detalhes:

- Os sistemas usados são responsáveis por:
  - Encontrar as páginas na Internet;
  - Armazenar os conteúdos;
  - Identificar e separar esses conteúdos;
  - Registra tudo de forma organizada e classificada.
- O objetivo é otimizar o processo de busca e oferecer as respostas mais assetivas para os interesses do usuário.

Antigamente a quantidade de vezes que uma palavra aparecia era importante, dessa forma os _Web Masters_ enchiam comentários e keywords nos HTMLs repetindo essas palavras afim de otimizar o aparecimento da página nos mecanismos de buscas, isso é algo que hoje em dia pode prejudicar o alcance de nossos sites. O Google não está provendo serviços para melhorar o engajamento, acesso e converção do seu site, ele provê serviços para proporcionar a melhor busca para o usuário.

Nós, como desenvolvedores, devemos saber o que o Google vai valorizar e deixarmos nosso site pronto, preparado, para que quando o GoogleBot passar por ali ele ter uma visão de que o site está bem construído, está tudo dentro do padrão. No SEO, fazemos alterações que só ficam aparentes os resultados após semanas/meses ou até mais tempo.

#### O que acontece quando o usuário faz uma busca?

Vamos ver uma lista, sequencial, do que acontece:

1. Os algoritmos analisam com base nos fatores de ranqueamento os itens classificados;
   - O que são esses fatores?
   - São mais de 200, são centenas. Os "principais" iremos ver em anotações futuras, mas podemos citar o título do site, a URL, o título (h1) da página em si, entre outros.
2. Encontram e apresentam os melhores resultados para exibir ao usuário;
   - O algoritmo do Google está sempre evoluindo para dar o **melhor resultado para o usuário**, o que importa pra ele é que você (como usuário) obtenha facilmente aquilo que você procura.

Para citar mais diretamente alguns dos fatores analisados:

- Autoridade do site;
- Tempo de existência do domínio;
- Quantidade de palavras-chave pesquisadas no texto;
- Os algoritmos também avaliam a localização das palavras-chave dentro do texto:
  - No título;
  - No cabeçalho;
  - Na URL;
  - Cada posição contribui na determinação dos resultados;
  - Entre outros...

A combinação desses e outros fatores de ranqueamento servirão para exibir os melhores resultados para o usuário.

#### Inteligência nos resultados

Para entregar precisão nos resultados, o Google desenvolveu tecnologias capazes de detectar:

- O idioma;
- O local de pesquisa do usuário;
- Completar frases;
- Interpretar erros de digitação;
- Aplicar sinônimos.
