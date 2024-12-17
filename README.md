**Alunos/Matricula:** [João V. Farias](https://github.com/beyondmagic) & [Renan V. Guedes](https://github.com/R-enanVieira) / 221022604 & 221031363

**Arquitetura Usada:** ResNet do zero

**Dataset Link:** [V1: Nonsegmented single plants (1.7GB)](https://vision.eng.au.dk/?download=/data/WeedData/Nonsegmented.zip)

# Rede Neural para determinar espécia de uma muda, dada sua imagem.

**Sobre o Dataset:** O dataset de mudas de plantas contém imagens de aproximadamente `960 plantas únicas` pertencentes a `12 espécies` em vários estágios de crescimento. Ele compreende imagens RGB anotadas com uma resolução física de aproximadamente `10 pixels por mm`.

Para o projeto, pensamos inicialmente em utilizar filtros, dos quais rapidamente abandonamos a ideia por ser complicado de mais criar uma função que removesse tantos fundos diferentes, alguns mais cinzas, outros mais claros; se pensassemos apenas em deixar o verde, havia uma boa chance de não pegar plantas mais "amareladas" ou perto do azul, então também não era uma escolha boa.

O projeto então foi construindo uma arquitetura do zero de ResNet, parecida com a mencionada por K. He em 2015 em seu primeiro artigo sobre o assunto.

<img src="/.github/confusion_matrix.png">
