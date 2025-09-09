# LH_CD_2025

## Instalação 

Python versão 3.11

Bibliotecas utilizadas: Pandas, sklearn, numpy, matplotlib, seaborn, scipy (presentes no arquivo requirements.txt)

Modelo presente junto ao EDA no jupyter notebook!

Para rodar o modelo:

import joblib

load_model = joblib.load("random_forest.pkl")
pred = load_model.predict(novo_filme_dataframe)

**Nota-se que ao adicionar uma nova entrada as colunas devem estar na mesma ordem como o novo dicionario na aba "Adicionando a entrada" (usar como base e preencher as categorias presente no filme com 1 nas variáveis dummy, também não esquecer de seguir o passo de transformação em log para gross e votos, que podem inicializar no dicionario como 0.0) no passo 4. Prevendo nota IMDB.**  

Modelo não foi feito como uma pipeline (decisão ruim), então se deve garantir que os novos dados entrem com o mesmo formato de colunas e unidades que foi feito para treinar o modelo.
