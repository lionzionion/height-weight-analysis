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
***Explicação:
Neste trecho, você está criando um ndarray chamado altura_em_centimetros a partir da lista lista_de_centimetros e, em seguida, 
criando outro ndarray chamado altura_em_metros convertendo os valores de altura_em_centimetros para metros. Os resultados são impressos no final.***

# 2) IMC

```python ## Lista de pesos em kg
lista_pesos = [70, 75, 80, 85]

## Criar um ndarray chamado pesos
pesos = np.array(lista_pesos)

## Calcular o IMC
imc = pesos / altura_em_metros ** 2

## Arredondar os resultados do IMC
imc_arredondado = np.round(imc, 2)

## Mostrar os resultados
print("Altura em centímetros:", altura_em_centimetros)
print("Altura em metros:", altura_em_metros)
print("Pesos em kg:", pesos)
print("IMC:", imc_arredondado)
```

