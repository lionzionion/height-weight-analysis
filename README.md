# Meu Projeto

## Projeto de Cálculo de IMC

### 1. Alturas

#### i. Criando Arrays para Alturas

```python
import numpy as np

# Lista de alturas em centímetros
lista_de_centimetros = list(range(170, 190, 5))

# Criando um ndarray chamado altura_em_centimetros
altura_em_centimetros = np.array(lista_de_centimetros)

# Convertendo alturas para metros
altura_em_metros = altura_em_centimetros / 100.0
ii. Criando Arrays para Pesos e Calculando IMC
python
Copy code
# Lista de pesos em kg
lista_pesos = [70, 75, 80, 85]

# Criando um ndarray chamado pesos
pesos = np.array(lista_pesos)

# Calculando o IMC
imc = pesos / altura_em_metros ** 2
imc_arredondado = np.round(imc, 2)

# Exibindo resultados
print("Altura em centímetros:", altura_em_centimetros)
print("Altura em metros:", altura_em_metros)
print("Pesos em kg:", pesos)
print("IMC:", imc_arredondado)
2. Projeto de Gerenciamento Financeiro
i. Gerenciando Dados Financeiros
python
Copy code
# Lista de dados financeiros
dados_financeiros = [[3000, 2500, 1000, 10000], [1000, 2500, 3000, 5000], [6000, 5500, 7000, 16000]]

# Criando um ndarray para dados financeiros
dados_financeiros_ndarray = np.array(dados_financeiros)

# Calculando o endividamento total
endividamento_total = np.sum(dados_financeiros_ndarray)
print("Endividamento Total:", endividamento_total)
ii. Correção de Dados
python
Copy code
# Corrigindo um valor específico
dados_financeiros_ndarray[0, 1] = 3000

# Exibindo dados financeiros corrigidos
print("Dados Financeiros (após correção):")
print(dados_financeiros_ndarray)
Conclusão
Estes projetos demonstram a eficácia do NumPy no manuseio eficiente de dados numéricos. Seja calculando o IMC ou gerenciando dados financeiros, o NumPy simplifica operações complexas e melhora a legibilidade do código.
