# Core Web Vitals

Em 2021, surgiu um update no Google que gerou bastante tumulto, este update foi chamado de _Paid Experience Update_. Ele foi responsável pela introdução de 3 métricas que medem a experiência do usuário nas páginas dos sites e passaram a ser vitais quando falamos da indexabilidade dos sites, essas métricas são chamdas de _Core Web Vitals_.

Vamos entender cada uma delas.

## As métricas:

### LCP - Largest Contentful Paint (Loading)

Traduzindo o LCP para português temos algo como "Maior Renderização de Conteúdo". Essa métrica mede o desempenho do carregamento das páginas, ou seja, o tempo que demora para carregar o maior conteúdo que tem dentro de uma página.

O que devemos ressaltar é que não se trata do carregamento da página inteira, mas sim o tempo que o maior conteúdo dentro de uma página vai carregar.

Segundo o Google, um tempo bom para a LCP é de 2.5 segundos após o início do carregamento da página, sendo até 4 segundos uma nota considerada razoável e que precisa de melhoras, qualquer tempo de carregamento acima disso é considerado _negativo_.

### FID - First Input Delay (Interactivity)

FID, que significa "O Atraso da Primeira Entrada", mede a interatividade de um usuário com alguma página, ou seja, o tempo gasto entre o momento que o usuário enviou uma ação, um clique, uma interação com a página, e o momento que essa ação é iniciada. Essa métrica aborda um "acionamento" de milissegundos desde o momento que você clica até o site começar a processar seu clique, é basicamente isso.

O Google indica que as páginas devem ter um FID de 100 milisegundos ou menos para serem considerados bons. Acima disso, até antes de 300 milisegundos, é considerado razoável e precisa de melhoras e qualquer valor acima deste é considerado _negativo_, ruim, diminui o ranqueamento do site/página.

### CLS - Cumulative Layout Shift (Visual Stability)

CLS significa "Mudança Acumulativa de Layout", é basicamente a medida da estabilidade visual do seu site conforme sua página vai caregando. Isso acontece, normalmente, através daquelas reorganizações da página quando ela está terminando de carregar todos os seus elementos.

Se trata daquele carregamento dos elementos da página que ficam se rearranjando conforme os elementos vão se organizando dentro da estrutura do site, do HTML e dos estilos CSS. Isso ocorre principalmente nas páginas que estão sendo acessadas por dispositivos Mobile.

No CLS, a métrica é feita através de uma pontuação calculada olhando para o impacto dessas movimentações, na distâncias entre os elementos antes e depois da reorganização.

Para que a média de CLS seja boa ela deve estar em 0.1 ou menos, para ser considerada razoável e que necessita de melhoras teremos valores acima de 0.1 e abaixo de 0.25. Qualquer valor de 0.25 é considerado ruim e é punitivo com nosso site/página, é _negativo_ no impacto que causamos.

## Para encontrar essas estatísticas utilizamos...

O **PageSpeed Insights**, algo que veremos nas próximas anotações.
