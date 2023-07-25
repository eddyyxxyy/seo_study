# Instalação padrão em Sites de 3 formas diferentes

Iremos abordar três maneiras bem simples de se implementar os códigos/tags/diretivas necessárias para que a conexão do Fluxo de Dados do seu site possa ir de encontro à sua Propriedade do GA4, tudo isso utilizando do seu ID de Métrica.

Então, vamos a primeira delas...

## Via WordPress ou outras plataformas prontas

Provavelmente a forma mais simples e direta de se realizar a conexão entre seu site e o GA4. Porém, há formas de se fazer que também são mais técnicas, que envolvem mexer nos códigos da plataforma.

Por exemplo, você poderia ir em `Aparência > Editor de Temas` e injetar o código da Tag (que é o código que levará seus dados à sua Propriedade por meio do seu ID) dentro do `<head>` do arquivo `header.php` do seu tema. Contudo, por questões de segurança, pode não ser possível realizar essa alteração e de certa forma não é recomendado também, uma vez que atualizações do seu tema forem instaladas, todas as mudanças em código puro se perderão.

O que podemos fazer e é indicado seria utilizar um plugin, algum que possibilite a injeção de códigos HTML. Um exmeplo seria o plugin Custom CSS & JS para WordPress.

> O mais importante é que deixemos a Tag implementada em __todas__ as páginas que queremos acompanhar.

## Sites Próprios/Puros

Dentro da ferramenta do GA4, caso já tenha sido definido o Fluxo de Dados (a definição do Domínio/URL do seu site e as opcionais "Métricas Otimizadas"), você terá o seu ID de Métrica, este seria o seu identificado único dessa propriedade que está sendo acessada.

Pouco abaixo da onde podemos consultar nosso ID de Métrica temos as instruções para adicionar a Tag em seu site.

Por mais que a implementação seja técnica, conhecimentos básicos de HTML já fazem jus ao que se é pedido, é necessário somente copiar e colar o código apresentado dentro da seção do código que foi dita pelas próprias instruções.

## Google Tag Manager

O Tag Manager é uma ferramenta do Google que te ajuda a instalar Tags no seu site, tags estas que agregam eventos à serem disparados em determinadas páginas, botões, entre outros.

O único momento que precisamos de desenvolvedores, quanto ao uso do Tag Manager, é na hora de instalar/colocar os códigos da ferramenta em seu site.

Quando entramos no Tag Manager, após criarmos uma conta e um container (especificando, assim como no GA4, se é Web, iOS, Android, etc), teremos acesso ao código que devemos inserir no `<head>` e `<body>`.

Após isso, podemos "_Adicionar uma nova tag_" por meio da página inicial de nosso container. Dessa forma, colocaremos a vinculação do GTM com o GA4 utilizando nosso ID da Métrica e, somente então, adicionamos um __Acionador__ que executa os códigos da tag e envia os dados para o GA4. Porém, somente isso que fizemos não garante que está funcionando.

Para garantirmos que as coisas estão funcionando como queriamos/precisavamos, podemos clicar em "Visualizar" e teremos uma nova aba com o Tag Assistant, permitindo que testemos nossas tags em tempo real, assim validaremos o fluxo de dados que desejamos.

> O Tag Assistant é uma ferramenta independente do Tag Manager, ou seja, pode ser usada mesmo fora do Tag Manager.

Ainda mais, com o GTM podemos fazer um controle de versões dos nossos Containers, trazendo ainda mais robustez para o uso da ferramenta.
