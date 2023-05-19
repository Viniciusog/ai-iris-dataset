#### Projeto de inteligência artificial - Predição de classes iris

#### Introdução
Existem diversas espécies de flores do gênero Iris. Nas amostras dos conjuntos de dados analisados, existem três espécies, que são: setosa, virginica e versicolor. Para classificá-las, é preciso analisar informações como o comprimento e largura das pétalas, o comprimento e largura das sépalas, dentre outros dados.

Assim, esse trabalho apresenta uma aplicação, que utiliza técnicas de aprendizado de máquina, cujo objetivo é classificar corretamente uma flor de íris, com a maior precisão possível. Para isso, foi realizada uma análise dos dados das bases utilizadas, além da utilização de quatro técnicas de classificação para identificar as flores. Por fim, será analisado o desempenho das técnicas utilizadas, com o objetivo de concluir qual delas foi a mais precisa.

#### Base de dados
Para a aplicação dos algoritmos de classificação de aprendizado de máquina, foram utilizadas três bases de dados. Todas essas 3 bases contém as seguintes informações::

-   ID: responsável por identificar a amostra;
    
-   SepalLenghtCm: comprimento da sépala em centímetros;
    
-   SepalWidthCm: largura da sépala em centímetros;
    
-   PetalLengthCm: comprimento da pétala em centímetros;
    
-   PetalWidthCm: largura da pétala em centímetros;
    
-   Species: espécie da qual a flor do gênero Iris pertence.
    

A primeira base de dados, que pode ser encontrada no [link](https://www.kaggle.com/datasets/uciml/iris), contém 150 dados, sendo 50 para a espécie Iris-setosa, 50 para Iris-versicolor e 50 para Iris-virginica. Esta base foi introduzida pelo biólogo e estatístico Ronald Fisher em um documento em 1936, sendo considerado um data set clássico.

Já a segunda base de dados, que pode ser encontrada no [link](https://www.kaggle.com/datasets/mathurinache/iris-augmented), contém cerca de 1.000.000 de dados gerados com CTGAN, uma técnica de aprendizado de máquina que utiliza de redes generativas adversárias (GANs) para sintetizar dados tabulares com características semelhantes aos dados originais. GANs são um tipo de rede neural que consiste em duas partes: um gerador que cria amostra de dados sintéticos e um discriminador que avalia a autenticidade das amostras geradas em comparação com os dados reais. O CTGAN é uma implementação específica de GANs para dados tabulares, onde a rede neural do gerador é projetada para produzir linhas de uma tabela, e a rede neural do discriminador avalia a autenticidade da tabela como um todo.

. Por fim, a terceira base de dados utilizada foi gerada artificialmente pelo grupo utilizando de uma API chamada Gretel. Esta API utiliza o algoritmo chamado “Gretel Synthetics”, que também é baseado em técnicas de rede generativa adversarial. A partir dos dados originais (DataSet 1), a plataforma treina um modelo GAN que gera dados sintéticos que se assemelham aos dados originais, mas não contêm informações identificáveis dos indivíduos ou entidades nos dados. Inicialmente, o modelo é treinado para gerar dados sintéticos que sejam estatisticamente semelhantes ao dados originais, para posteriormente, refinar esse modelo e produzir dados sintéticos que atendam a critérios específicos de privacidade, como a remoção de informações identificáveis e a preservação de padrões e relacionamentos importantes nos dados.