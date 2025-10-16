# Análisis de Sentimiento en el corpus de reseñas cinematográficas (IMDb)

En este trabajo se han aplicado métodos propios del **Procesamiento del Lenguaje Natural (PLN)**, mediante la combinación de recursos léxicos (*SentiWordNet*), modelos de lenguaje (*Transformers*, *RoBERTa*) y técnicas de *machine learning* aplicadas al **Análisis de Sentimiento**, con el objetivo de evaluar su eficacia en el corpus de reseñas cinematográficas IMDb.

En una primera etapa, se han configurado clasificadores lineales con ponderaciones léxicas derivadas de SentiWordNet, calculadas mediante la suma y el promedio, con y sin reglas heurísticas. Además, se han entrenado modelos lineales (*Logistic Regression* con L1 y L2, y *RidgeClassifier*) tanto con n-gramas con *embeddings* preentrenados, como con características adicionales léxicas de SentiWordNet, para evaluar el impacto de incorporar un lexicón al modelo clasificatorio.

Posteriormente, se han entrenado modelos basados en redes neuronales (RNN y LSTM) con distintas variantes, como mecanismos de atención y arquitecturas multientrada, combinadas, asimismo, con características léxicas.

Finalmente, se han evaluado modelos de aprendizaje transferido basados en Transformers, en concreto, se ha realizado *fine-tuning* sobre el modelo RoBERTa(*Robustly Optimized BERT Approach)* base, con distintas combinaciones de hiperparámetros como la tasa de aprendizaje, el número de épocas y la penalización por regularización. 

Parte del código base ha sido proporcionado por el profesor Nicolás José Fernández Martínez de la asignatura *Análisis de Sentimientos, afecto y connotación* perteneciente al Máster en Procesamiento del Lenguaje y aplicaciones de la IA a la Lingüística, de la Universidad de La Rioja

---

## Librerías principales:

- `nltk`
- `scikit-learn`
- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `lime`
- `tensorflow`
- `datasets`
- `transformers`

---
