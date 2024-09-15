# Otimização atraves de hiper-parametros
Estudo focado na utilização do hiperparâmetros da biblioteca Sklearn, utilizando o modelo de treino DecisionTreeClassifier.

Max_deph:
    A profundidade máxima da árvore. Se None, os nós serão expandidos até que todas as folhas sejam puras ou até que todas as folhas contenham menos de min_samples_split amostras.

min_samples_split:
    O número mínimo de amostras necessárias para dividir um nó interno:
        Se for int, considere min_samples_split como o número mínimo.
        Se for float, então min_samples_split é uma fração e ceil(min_samples_split * n_samples) é o número mínimo de amostras para cada divisão.

min_samples_leaf:
    O número mínimo de amostras necessárias para estar em um nó folha. Um ponto de divisão em qualquer profundidade só será considerado se deixar pelo menos              min_samples_leaf amostras de treinamento em cada um dos ramos esquerdo e direito. Isto pode ter o efeito de suavizar o modelo, especialmente na regressão.
    Se for int, considere min_samples_leaf como o número mínimo.
    Se for float, então min_samples_leaf é uma fração e ceil(min_samples_leaf * n_samples) é o número mínimo de amostras para cada nó.
