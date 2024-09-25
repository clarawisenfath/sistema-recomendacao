# sistema-recomendacao

# propósito do projeto
O projeto tem como objetivo criar um sistema que recomenda filmes para os usuários de forma personalizada. Para isso, ele utiliza um método de agrupamento chamado K-means, que organiza os usuários em grupos com base nos filmes que já assistiram.

A ideia principal é ajudar os usuários a encontrar novos filmes que possam gostar, analisando os padrões de visualização de pessoas com gostos semelhantes. O sistema começa coletando dados sobre quais filmes cada usuário já viu. Em seguida, o K-means divide esses usuários em grupos, onde cada grupo contém pessoas que assistiram a filmes parecidos. Depois dessa classificação, o sistema informa a cada usuário a qual grupo pertence e quais filmes ele já assistiu, o que ajuda a entender como as recomendações são feitas.

Quando um usuário é colocado em um grupo, o sistema verifica quais filmes foram assistidos por outros usuários do mesmo grupo. Dessa forma, ele consegue sugerir filmes que essas pessoas gostaram, mas que o usuário ainda não viu.

O K-means oferece recomendações personalizadas, levando em conta os interesses de cada usuário e as preferências de pessoas semelhantes. Isso pode aumentar a satisfação dos usuários e mantê-los mais engajados na plataforma. Além disso, o sistema incentiva a descoberta de filmes que o usuário pode não conhecer, enriquecendo sua experiência de entretenimento.

# Algoritmo de Agrupamento utilizado 
O algoritmo de agrupamento usado para as recomendações é o K-means. Ele é muito comum em análise de dados e aprendizado de máquina e funciona de maneira simples.

Primeiro, o usuário escolhe quantos grupos quer criar, baseado na ideia de quantas categorias de gostos existem entre os usuários. Depois, o K-means seleciona aleatoriamente alguns pontos de dados para serem os "centros" dos grupos.

Em seguida, cada usuário é colocado no grupo cujo centro está mais perto, usando os filmes que assistiram como base. Isso é feito calculando a distância entre o usuário e os centros dos grupos. Após essa atribuição, o algoritmo recalcula a posição dos centros, levando em conta a média dos usuários de cada grupo.

Esse processo de atribuição e atualização dos centros continua até que as mudanças nas atribuições sejam pequenas ou até que um número máximo de tentativas seja alcançado. Assim, o K-means consegue identificar grupos de usuários com gostos parecidos, o que ajuda a recomendar filmes que esses usuários já viram e gostaram.