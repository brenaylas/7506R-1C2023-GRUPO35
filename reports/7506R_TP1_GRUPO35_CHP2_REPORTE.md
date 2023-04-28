# **Trabajo Práctico 1: Reservas de Hotel**

## Checkpoint 2

**Grupo 35**

### Integrantes:

- Aylas, Brenda
- Cori, William
- Nazario, Ingrith

A partir del dataset procesado en el checkpoint uno se fue probando distintos metodos de encoding para entrenar un árbol de decisiones.

Para las variables numéricas se probo utilizar el _MinMaxScaler_ en distintos valores y el _StandardScaler_ de sklearn sin variaciones en el f1 score.

Para las variables categoricas se utilizó _one hot encoding_ y _binary enconding_ segun la cantidad de categorias en cada variable.

Ademas para testear todos estos cambios se combino con GridSearchCV con distintos hiperparametros para ver si se mejora o no el f1 score en cross validation.

Para que las transformaciones sean las mismas en ambos conjuntos (train y test) se utilizo un pipeline de sklearn.

Y para guardar los modelos se utilizo la libreria _dill_ que es muy similar a pickle pero permite persistir funciones que eran necesarias para nuestro modelo.
