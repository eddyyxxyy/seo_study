# Métrica Otimizada e Dimensão Personalizada

Na prática, com configurações e análises, iremos ver uma situação hipotética de um site fictício tendo seus dados coletados pelo GA4.

Mas, antes de começar, iremos verificar mais sobre a documentação oficial do GA4 que fala sobre Métricas Otmizadas.

## Métrica Otimizada

Todo o funcionamento das Métricas Otimizadas estão disponíveis online pelo link da [documentação oficial](https://support.google.com/analytics/answer/9216061?hl=pt-BR&sjid=14515463612533949003-SA) e para que possamos testar e validar as configurações adotadas em nossas Métricas, utilizaremos o Tag Assistant.

À partir do momento que configuramos um Fluxo de Dados no GA4 (podendo verificar isso na aba "_Administrador_ -> _Propriedade_ -> _Fluxo de Dados_"), temos a possibilidade de escolher as Métricas Otimizadas que queremos trabalhar, por padrão estão todas sempre ativas e recomenda-se que não se altere isso.

São diversas as Métricas Otimizadas que temos disponíveis por padrão, entre elas:

- Page View | Visualizações de Página;
- Page Scroll | Rolagem de Tela (90% da página);
- Link Click | Cliques em links para sites externos;
- View Search Results | Quando uma página de pesquisa é acessada por um usuário;
- File Download | Quando um arquivo é baixado do site por um usuário;
- Video Engagement | Quando um usuário assiste à um vídeo;
- entre outros...

Na visualização da aba de Tempo Real do GA4 podemos acompanhar, assim como no Tag Assistant, a ocorrência desses eventos que por padrão e sem requerer maiores configurações além de uma ativação são providos e organizados pra nós.

Todos esses eventos, além de indicar que ocorreram, ainda trazem informações detalhadas por meio de parâmetros, por exemplo: um evento de **file_download** quando é disparado teremos como alguns seus parâmetros:

- A extensão do arquivo;
- O nome do arquivo;
- O texto do link que leva ao arquivo;
- A localização da página que possui o arquivo para download;
- entre outros...

E todos esses detalhes estão disponíveis na já citada documentação. Sabendo dessas informações é mais do que simples abrir seu GA4, pelo DebugView ou aba Tempo Real, ou Tag Assistant para que possa ver isso ocorrendo de forma simultânea com suas interações.

## Dimensão: Padrão x Personalizada

<!-- Continuar aula 13 da seção 3 -->
