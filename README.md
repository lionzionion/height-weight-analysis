# Projeto de Análise de Dados com NumPy
## 1) Alturas
### i. Transformação em Numpy Array
No trecho de código abaixo, criamos um NumPy array chamado altura_em_centimetros ao transformar a lista lista_de_alturas utilizando a função np.array().

```import numpy as np

# Lista de alturas em centímetros

lista_de_centimetros = list(range(170, 190, 5))

# Criar um ndarray chamado altura_em_centimetros

altura_em_centimetros = np.array(lista_de_centimetros)

### ii. Conversão para Metros

Em seguida, criamos um objeto altura_em_metros convertendo os valores de altura_em_centimetros para metros.

```# Criar um objeto altura_em_metros
altura_em_metros = altura_em_centimetros / 100.0

# Exibir resultados

```print("Altura em centímetros:", altura_em_centimetros)
print("Altura em metros:", altura_em_metros)

# 2) IMC

### i. Criação de Numpy Array para Pesos
Considerando pesos em Kg, criamos um Numpy array chamado pesos com a função np.array().

```# Lista de pesos em kg
lista_pesos = [70, 75, 80, 85]

# Criar um ndarray chamado pesos

pesos = np.array(lista_pesos)
ii. Cálculo do IMC
Utilizando os objetos que contêm alturas e pesos, calculamos o IMC desses indivíduos.

```# Calcular o IMC
imc = pesos / altura_em_metros ** 2

# Arredondar os resultados do IMC

imc_arredondado = np.round(imc, 2)

# Mostrar os resultados

print("Pesos em kg:", pesos)
print("IMC:", imc_arredondado)

3) Endividamento

i. Transformação de Dados em Numpy Array
Considere o seguinte conjunto de dados financeiros. Transformamos a lista de listas dados_financeiros em um Numpy array chamado dados_financeiros_ndarray.

```# Lista dados_financeiros
dados_financeiros = [[3000, 2500, 1000, 10000], [1000, 2500, 3000, 5000], [6000, 5500, 7000, 16000]]

# i) Transformar a lista dados_financeiros em um ndarray

dados_financeiros_ndarray = np.array(dados_financeiros)
ii. Transposição e Indexação
Utilizamos a transposição para garantir uma linha por indivíduo e uma coluna por informação. Imprimimos a segunda linha e a segunda coluna.

```# ii) Exibir o ndarray
print("Dados Financeiros:")
print(dados_financeiros_ndarray)

# Utilizando a indexação do numpy
print("Segunda linha do array:")
print(dados_financeiros_ndarray[1, :])

print("Segunda coluna do array:")
print(dados_financeiros_ndarray[:, 1])

iii. Cálculo do Endividamento Total
Calculamos o endividamento total e exibimos os resultados.

```# iii) Calcular o endividamento total
endividamento_total = np.sum(dados_financeiros_ndarray[:, :2] / dados_financeiros_ndarray[:, 2])

# Exibir resultados
print("Endividamento Total:", endividamento_total)
iv. Correção de Dados e Recálculo
Corrigimos um valor específico e refazemos os cálculos.

```# iv) Corrigir um valor específico
dados_financeiros_ndarray[2, 2] = 10000

# Exibir resultados após correção
print("Dados Financeiros (após correção):")
print(dados_financeiros_ndarray)
4) Tratamento de Valores Especiais
No trecho de código abaixo, geramos um ndarray com números pseudoaleatórios e desconsideramos valores iguais a zero.

```# np.random.seed(1234) garante a reprodutibilidade dos resultados
np.random.seed(1234)

# i) Criação do objeto bool_zero
poi = np.random.poisson(3, 100)
bool_zero = poi == 0

# ii) Contagem de valores zero
quantidade_zeros = np.sum(bool_zero)

# iii) Utilização da indexação booleana para criar poi_nao_zero
poi_nao_zero = poi[~bool_zero]  # ~ inverte os valores booleanos

# Exibição dos resultados
print("Objeto poi:", poi)
print("Objeto bool_zero:", bool_zero)
print("Quantidade de zeros:", quantidade_zeros)
print("Objeto poi_nao_zero:", poi_nao_zero)
Este projeto oferece práticas essenciais de manipulação de dados usando a biblioteca NumPy em Python.




