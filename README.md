# Book-analisys

# Apresentação do Projeto [book-analysis]

Recebemos uma proposta da Alta Books para implementação de uma solução capaz de analisar comentários realizados no site da Amazon.

o Analisar comentários e avaliações (estrelas) feitas no livro: Data Science para negócios o Avaliação das métricas históricas e criação de um dashboard com essas informações. o O sistema precisa ser atualizado com novos dados 1 vez por dia.

Como analisar emoções de texto? o Existem técnicas relacionadas a Processamento de Linguagem Natural que nos permitem determinar se dados (textos) são positivos, negativos ou neutros.

Por que Análise de Sentimentos são tão importantes para empresas? o Existe uma infinidade de aplicações, mas é comumente usado para analisar comentários de clientes, respostas de pesquisas e análises de produtos.

### Tarefas

- Como funciona a Análise de Sentimentos?
    
    Análise de sentimentos tem por função identificar, extrair, quantificar e estudar estados afetivos e informações subjetivas. Ela utiliza algoritmos de Natural Language Process(NLP) e Machine Learning para analisar e classificar textos com tons emocionais. A análise de sentimento funciona dividindo uma mensagem em blocos de tópicos e, em seguida, atribuindo uma pontuação de sentimento a cada tópico. Os modelos básicos concentram-se em especial nas classificações positivas, negativas ou neutras como graduação de sentimento (como estrelas,p.e.), mas podem-se levar em consideração também as emoções contidas em um texto (amo este produto, detestei o atendimento, p.e.), as características associadas a um produto ou serviço (produto mais barato que, melhor qualidade que, p.e.). O contexto de uma sentença também pode indicar a direção do sentimento. Há ainda que se considerar a dificuldade que a Inteligencia Artificial tem de compreender ou identificar sarcasmo e ironia em uma sentença. A análise de sentimento enfrenta algumas limitações e dificuldades de análise, como fatores culturais, nuances linguísticas, palavras homónimas, erros de escrita, abreviaturas, contexto das frases.
    
- Como Análise de Sentimentos se aplica ao meu problema?
    
    Com as múltiplas opiniões, avaliações, recomendações do livro a Alta Books, versão física ou digital (Kindle) tornou-se essencial gerenciar reputação e identificar novas oportunidades. Para tal é necessário transformar as avaliações e informações textuais em dados mensuráveis, perceber os apectos chave do produto que os clientes gostam ou não gostam e perceber as mensagens implícitas nestes textos.
    
- Quais as principais técnicas utilizadas para Análise de Sentimentos?
    
    Existem ferramentas SaaS prontas no mercado para análise de sentimentos (software de Inteligencia Artificial), que analisam automaticamente os dados de texto ou permitem treinar modelos, cada uma com suas características, algunas requerem um maior conhecimento de ciencia de dados. Em alternativa é possível construir uma solução mais ajustada a solicitação do cliente com soluções de código aberto em Python ou Java. Para este projeto vamos optar pelo Python pois existem muitas bibliotecas de código aberto. Precisamos basicamente extrair os dados, dividir o texto em sentencas, identificar os sentimentos associados, classificação e quantificão, atribuído valores as polaridades (ex: -1,0,+1) e finalmente estudá-los.
    

### Que recursos podemos utilizar:

- Scikit-learn é a biblioteca para Machine Learning e possui ferramentas úteis para vetorização de texto.

[scikit-learn](https://scikit-learn.org/stable/)

- A regressão linear é um algoritmo estatístico usado para prever um valor Y , dados os recursos X.

[Regressão Linear?](https://medium.com/@lauradamaceno/regress%C3%A3o-linear-6a7f247c3e29)

- Support Vector Machines (SVM) é outro modelo de aprendizado de máquina supervisionado, semelhante à regressão linear, mas mais avançado.

[Support Vector Machines (SVM) Algorithm Explained](https://monkeylearn.com/blog/introduction-to-support-vector-machines-svm/)

- [NLTK]tem sido a biblioteca NLP tradicional para Python.

[NLTK](https://www.nltk.org/)

- [SpaCy] é uma biblioteca fornece um conjunto robusto de funções de baixo nível para NLP e suporte para classificadores de texto de treinamento.

[spaCy · Industrial-strength Natural Language Processing in Python](https://spacy.io/)

- [TensorFlow] desenvolvido pelo Google, fornece um conjunto de ferramentas de baixo nível para construir e treinar redes neurais. Há também suporte para vetorização de texto, tanto na frequência tradicional de palavras quanto em incorporações de palavras mais avançadas.

[TensorFlow](https://www.tensorflow.org/)

- [Keras] fornece abstrações úteis para trabalhar com vários tipos de redes neurais, como redes neurais recorrentes (RNNs) e redes neurais convolucionais (CNNs ) e empilhar facilmente camadas de neurônios.

[Keras: the Python deep learning API](https://keras.io/)

- [PyTorch] é uma estrutura recente de aprendizado profundo apoiada por algumas organizações de prestígio como Facebook, Twitter, Nvidia, Salesforce, Universidade de Stanford, Universidade de Oxford e Uber. Desenvolveu rapidamente uma comunidade forte.

[PyTorch](https://pytorch.org/)

## Quais são as principais métricas de interação?

Considerando as informações passíveis de serem extraídas com comentários, poderemos gerar as seguintes métricas:

- % de avaliações por compra
- % de opiniões por compra
- Tipo de sentimento por característica do produto
- Taxa de frequência de ocorrência da característica
- Mudanças no sentimento ao longo do tempo
- Mudanças no sentimento por característica ao longo do tempo
- Perfil consumidor: sexo, idade (é possível???)

Referências: -Sentiment Analysis Guide -Sentiment Analysis | Comprehensive Beginners Guide | Thematic | Thematic Tudo sobre NLP: o que é, como opera, usos e desafios na IA
