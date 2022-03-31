# book-analysis

Apresentação do Projeto [book-analysis]

Recebemos uma proposta da Alta Books para implementação de uma solução capaz de analisar comentários realizados no site da Amazon.

o Analisar comentários e avaliações (estrelas) feitas no livro: Data Science para negócios
o Avaliação das métricas históricas e criação de um dashboard com essas informações.
o O sistema precisa ser atualizado com novos dados 1 vez por dia.

Como analisar emoções de texto?
o Existem técnicas relacionadas a Processamento de Linguagem Natural que nos permitem determinar se dados (textos) são positivos, negativos ou neutros.

Por que Análise de Sentimentos são tão importantes para empresas?
o Existe uma infinidade de aplicações, mas é comumente usado para analisar comentários de clientes, respostas de pesquisas e análises de produtos.

• Tarefas
[ ] Como funciona a Análise de Sentimentos?
Análise de sentimentos tem por função identificar, extrair, quantificar e estudar estados afetivos e informações subjetivas. Ela utiliza algoritmos de Natural Language Process(NLP) e Machine Learning para analisar e classificar textos com tons emocionais.
A análise de sentimento funciona dividindo uma mensagem em blocos de tópicos e, em seguida, atribuindo uma pontuação de sentimento a cada tópico.
Os modelos básicos concentram-se em especial nas classificações positivas, negativas ou neutras como graduação de sentimento (como estrelas,p.e.), mas podem-se levar em consideração também as emoções contidas em um texto (amo este produto, detestei o atendimento, p.e.), as características associadas a um produto ou serviço (produto mais barato que, melhor qualidade que, p.e.). O contexto de uma sentença também pode indicar a direção do sentimento. Há ainda que se considerar a dificuldade que a Inteligencia Artificial tem de compreender ou identificar sarcasmo e ironia em uma sentença.
A análise de sentimento enfrenta algumas limitações e dificuldades de análise, como fatores culturais, nuances linguísticas, palavras homónimas, erros de escrita, abreviaturas, contexto das frases.

[ ] Como Análise de Sentimentos se aplica ao meu problema?
Com as múltiplas opiniões, avaliações, recomendações do livro a Alta Books, versão física ou digital (Kindle) tornou-se essencial gerenciar reputação e identificar novas oportunidades.
Para tal é necessário transformar as avaliações e informações textuais em dados mensuráveis, perceber os apectos chave do produto que os clientes gostam ou não gostam e perceber as mensagens implícitas nestes textos.

[ ] Quais as principais técnicas utilizadas para Análise de Sentimentos?
Existem ferramentas SaaS prontas no mercado para análise de sentimentos (software de Inteligencia Artificial), que analisam automaticamente os dados de texto ou permitem treinar modelos, cada uma com suas características, algunas requerem um maior conhecimento de ciencia de dados.
Em alternativa é possível construir uma solução mais ajustada a solicitação do cliente com soluções de código aberto em Python ou Java. Para este projeto vamos optar pelo Python pois existem muitas bibliotecas de código aberto.
Precisamos basicamente extrair os dados, dividir o texto em sentencas, identificar os sentimentos associados, classificação e quantificão, atribuído valores as polaridades (ex: -1,0,+1) e finalmente estudá-los.

Como recursos podemos utilizar:

 - Scikit-learn é a biblioteca para Machine Learning e possui ferramentas úteis para vetorização de texto. O Scikit-learn possui implementações para Support Vector Machines, Naïve Bayes e Logistic Regression, entre outros.
Naive Bayes é um grupo bastante simples de algoritmos probabilísticos que, para classificação de análise de sentimento, atribui uma probabilidade de que uma determinada palavra ou frase seja considerada positiva ou negativa. Basicamente, Naive Bayes calcula palavras umas contra as outras. Assim, com modelos de aprendizado de máquina treinados para polaridade de palavras, podemos calcular a probabilidade de uma palavra, frase ou texto ser positivo ou negativo. Quando técnicas como lematização, remoção de palavras irrelevantes e frequência das palavras (TF-IDF )são implementadas, o Naive Bayes se torna cada vez mais preciso.

 - A regressão linear é um algoritmo estatístico usado para prever um valor Y , dados os recursos X. Usando machine learnig, os conjuntos de dados são examinados para m mostrar um relacionamento. As relações são então colocadas ao longo do eixo X/Y , com uma linha reta passando por elas para prever outras relações. A regressão linear calcula como a entrada X (palavras e frases) se relaciona com a saída Y (polaridade). Isso determinará onde as palavras e frases caem em uma escala de polaridade de “realmente positivo” para “realmente negativo” e em todos os lugares intermediários.

 - Support Vector Machines (SVM) é outro modelo de aprendizado de máquina supervisionado, semelhante à regressão linear, mas mais avançado. O SVM usa algoritmos para treinar e classificar texto dentro de nosso modelo de polaridade de sentimento, dando um passo além da previsão X/Y .O SVM então atribui um hiperplano que melhor separa as tags. Em duas dimensões isso é simplesmente uma linha (como na regressão linear). Para maximizar o aprendizado de máquina, o melhor hiperplano é aquele com a maior distância entre cada tag:Simplificando , o SVM permite um aprendizado de máquina mais preciso porque é multidimensional.

[NLTK]tem sido a biblioteca NLP tradicional para Python. Possui uma comunidade ativa e oferece a possibilidade de treinar classificadores de machine learning.
[SpaCy] é uma biblioteca de NLP com uma comunidade crescente. Assim como o NLTK, ele fornece um conjunto robusto de funções de baixo nível para NLP e suporte para classificadores de texto de treinamento.
[O TensorFlow] desenvolvido pelo Google, fornece um conjunto de ferramentas de baixo nível para construir e treinar redes neurais. Há também suporte para vetorização de texto, tanto na frequência tradicional de palavras quanto em incorporações de palavras mais avançadas.
[Keras] fornece abstrações úteis para trabalhar com vários tipos de redes neurais, como redes neurais recorrentes (RNNs) e redes neurais convolucionais (CNNs ) e empilhar facilmente camadas de neurônios. Keras pode ser executado em cima do Tensorflow ou Theano. Ele também fornece ferramentas úteis para classificação de texto.
[O PyTorch] é uma estrutura recente de aprendizado profundo apoiada por algumas organizações de prestígio como Facebook, Twitter, Nvidia, Salesforce, Universidade de Stanford, Universidade de Oxford e Uber. Desenvolveu rapidamente uma comunidade forte.
[ ] Quais são as principais métricas de interação?

Considerando as informações passíveis de serem extraídas com comentários, poderemos gerar as seguintes métricas:

% de avaliações por compra
% de opiniões por compra
Tipo de sentimento por característica do produto
Taxa de frequência de ocorrência da característica
Mudanças no sentimento ao longo do tempo
Mudanças no sentimento por característica ao longo do tempo
Perfil consumidor: sexo, idade (é possível???)
[ ] Criar um Repositório no GitHub com o nome [book-analysi]

[ ] Inserir um Readme.md com a documentação das tarefas acima

[ ] Onde conseguir os dados necessários para o projeto?
https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt

Referências:
Sentiment Analysis Guide
Sentiment Analysis | Comprehensive Beginners Guide | Thematic | Thematic
Tudo sobre NLP: o que é, como opera, usos e desafios na IA
