# Liberías útiles 

## Python 

### [arcade](https://api.arcade.academy/en/latest/)
Se trata de una librería para crear videojuegos en 2D
Sirve para diseñar el tablero del Sokoban en el TP1 de Métodos de Búsqueda. Es fácil de aprender y de usar 
```python
sudo pip3 install arcade
```
```python
import arcade
```

### [sklearn](https://scikit-learn.org/stable/index.html) 
Se trata de una libería para anáisis de datos. 
En particular, usamos para el TP4 de Aprendizaje No Supervido el modulo de [decomposition](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) para Principal component analysis (PCA) y el de [preprocessing](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html) para estandarizar features.
[Ver instalación](https://scikit-learn.org/0.16/install.html)

```python
from sklearn.decomposition import PCA
from sklearn.preprocessing import StandardScaler
```

### [scipy](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html) 
Se trata de una librería de optimización. Ofrece varios métodos como Powell, BFGS, Newton, entre otros. 
En particular, usamos el de [Powell](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fmin_powell.html) para el TP5 sobre Deep Learning. [Ver Instalación](https://www.scipy.org/install.html)

## Java