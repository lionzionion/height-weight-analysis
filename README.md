# 1) Alturas

```python import numpy as np

## Lista de alturas em centímetros
lista_de_centimetros = list(range(170, 190, 5))

## i. Criar um ndarray chamado altura_em_centimetros
altura_em_centimetros = np.array(lista_de_centimetros)

## ii. Criar um objeto altura_em_metros
altura_em_metros = altura_em_centimetros / 100.0

## Mostrar os resultados
print("Altura em centímetros:", altura_em_centimetros)
print("Altura em metros:", altura_em_metros)
```


