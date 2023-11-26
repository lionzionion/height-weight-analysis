# Análise de Altura e Peso

# 1) Alturas

## Copiar código

```python import numpy as np

# Lista de alturas em centímetros
lista_de_centimetros = list(range(170, 190, 5))

# i. Criar um ndarray chamado altura_em_centimetros
altura_em_centimetros = np.array(lista_de_centimetros)

# ii. Criar um objeto altura_em_metros
altura_em_metros = altura_em_centimetros / 100.0

# Mostrar os resultados
print("Altura em centímetros:", altura_em_centimetros)
print("Altura em metros:", altura_em_metros)
```
***Explicação:
Neste trecho, você está criando um ndarray chamado altura_em_centimetros a partir da lista lista_de_centimetros e, em seguida, 
criando outro ndarray chamado altura_em_metros convertendo os valores de altura_em_centimetros para metros. Os resultados são impressos no final.***

# 2) IMC

## Copiar código

```python ## Lista de pesos em kg
lista_pesos = [70, 75, 80, 85]

# Criar um ndarray chamado pesos
pesos = np.array(lista_pesos)

# Calcular o IMC
imc = pesos / altura_em_metros ** 2

# Arredondar os resultados do IMC
imc_arredondado = np.round(imc, 2)

# Mostrar os resultados
print("Altura em centímetros:", altura_em_centimetros)
print("Altura em metros:", altura_em_metros)
print("Pesos em kg:", pesos)
print("IMC:", imc_arredondado)
```
**Explicação:
Aqui, você está criando um ndarray chamado pesos a partir da lista lista_pesos. Em seguida, 
você calcula o IMC utilizando a fórmula e arredonda os resultados para duas casas decimais. Os resultados finais são impressos.**

# 3) Endividamento

## Copiar código

```python # Lista dados_financeiros
dados_financeiros = [[3000, 2500, 1000, 10000], [1000, 2500, 3000, 5000], [6000, 5500, 7000, 16000]]

# i) Transformar a lista dados_financeiros em um ndarray
dados_financeiros_ndarray = np.array(dados_financeiros)

# ii) Exibir o ndarray
print("Dados Financeiros:")
print(dados_financeiros_ndarray)

# iii) Calcular o endividamento total
endividamento_total = np.sum(dados_financeiros_ndarray, axis=1)
print("Endividamento Total:", endividamento_total)

# iv) Corrigir um valor específico (por exemplo, substituir o valor 2500 por 3000)
dados_financeiros_ndarray[0, 1] = 3000
print("Dados Financeiros (após correção):")
print(dados_financeiros_ndarray)
```
**Explicação:
Neste trecho, você transforma a lista dados_financeiros em um ndarray chamado dados_financeiros_ndarray. Em seguida, você exibe o ndarray, 
calcula o endividamento total para cada indivíduo e corrige um valor específico (2500 por 3000). Os resultados finais são impressos.**

# 4) Identificação de Valores Zero

## Copiar código

```python # np.random.seed(1234) garante a reprodutibilidade dos resultados
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
```
**Explicação:
Aqui, você gera um ndarray chamado poi com números pseudoaleatórios seguindo uma distribuição de Poisson. Em seguida, você cria um objeto booleano bool_zero indicando quais valores de poi são zero. 
Você conta a quantidade de zeros, e finalmente, você cria um novo ndarray poi_nao_zero excluindo os valores zero usando a indexação booleana. Os resultados são impressos no final.**
