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
