# UNIFOR
**Nome**:Cauã de Norões Milfont Queiroz 
**Disciplina**: Raciocínio lógico algorítm

## Exercício exemplo
Represente, em fluxograma e pseudocódigo, um algoritmo para calcular o adicional de salário de funcionário por cargo de uma empresa fictícia. Sabe-se que os funcionários de cargo técnico receberão reajuste de 50%, cargo de gerência, um reajuste de 30% e demais, um reajuste de 10%. 

#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite o salário e profissão}}
B --> C[\sal, prof\]
C --> D{prof == 'Tecnico'}
D --FALSE--> E{prof == 'Gerente'}
D --TRUE--> F[sal_reaj = 1.5 * sal]
E --FALSE--> H[sal_reaj = 1.1 * sal]
E --TRUE--> G[sal_reaj = 1.3 * sal]
 
H --> J{{'Salário Reajustado = ', sal_reaj}}
G --> J
F --> J
J --> I([FIM])
```

#### Pseudocódigo
```
1  ALGORITMO calReajuste
2  DECLARE  sal, sal_reaj: real, prof: caractere
3  INICIO
4 ESCREVA "Digite o sálario e profissão"
5 LEIA sal, prof
6   SE prof == “Técnico”	 ENTÃO
7     sal_reaj ← 1.5 * sal
8 SENÃO
9  SE prof = “Gerente”	ENTÃO	
9     sal_reaj ← 1.3 * sal
10  SENÃO
11    sal_reaj ← 1.1 * sal
12 FIM_SE
13 ESCREVA “Salário Reajustado = “, sal_reaj
14 FIM_ALGORITMO
```

#### Teste
| sal | prof | prof == “Técnico” | prof = “Gerente” | sal_reaj | Saída |
| -- | -- | -- | -- | -- | -- |
| 1000 | Técnico | V | F | 1500 | “Salário Reajustado = 1500“ |
| 2000 | Gerente | F | V | 2600 | “Salário Reajustado = 2600“ |
| 9000 | Diretor | F | F | 9900 | “Salário Reajustado = 9900“ |

## Lista de exercícios 02

### Exercício 01 (2.5 pontos)
Calcule a média de quatro números inteiros dados.

#### Fluxograma (1.0 ponto)

```mermaid
flowchart TD
A([INICIO]) --> B{{Digite 4 números}}
B --> C[/N1, N2, N3, N4/]
C --> D{N1, N2, N3, N4 => 0  }
D --FALSE--> E{{O número tem que ser positivo!}}
D --TRUE--> F[media = N1 + N2 + N3 + N4 /4]
E --> H([FIM])
F --> G{{"A média é: ", media}}
G --> H
```

#### Pseudocódigo (1.0 ponto)

```
1 Algoritmo Media
2 DECLARE N1, N2, N3, N4, media: INTEIRO
3 INICIO
4 ESCREVA "Digite 4 números: "
5 LEIA N1, N2, N3, N4
6 SE N1, N2, N3, N4 => 0 ENTÂO
7 media = (N1 + N2 + N3 + N4)/4
8 ESCREVA "A média é: ",media
9 SENÃO
10 ESCREVA "O número tem que ser positivo!"
11 FIM_SE
12 FIM_ALGORITMO
```

#### Teste de mesa (0.5 ponto)

| N1           | N2           | N3           | N4           | >= 0         | Saída    |
|      --      |      --      |      --      |      --      |      --      | 
| 20           | 34           | -2           |  7           | F            |"Escreva um número positivo"
| 30           | 12           | 06           | 30           | V            |"Sua média é: " media
| 45           | 25           |45            |              | F            |"Digite 4 números 

### Exercício 02 (2.5 pontos)
Leia uma temperatura dada em Celsius (C) e imprima o equivalente em Fahrenheit (F). (Fórmula de conversão: F = (9/5) * C + 32)

#### Fluxograma (1.0 ponto)

```mermaid
flowchart TD
A([INICIO]) --> B([FIM])
```

#### Pseudocódigo (1.0 ponto)

```
Algoritmo ConverteCelsiusFarenheit
FIM_ALGORITMO
```

#### Teste de mesa (0.5 ponto)

| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |

### Exercício 03 (2.5 pontos)
Receba dois números reais e um operador e efetue a operação correspondente com os valores recebidos (operandos). 
O algoritmo deve retornar o resultado da operação selecionada simulando todas as operações de uma calculadora simples.

#### Fluxograma (1.0 ponto)

```mermaid
flowchart TD
A([INICIO]) --> B([FIM])
```

#### Pseudocódigo (1.0 ponto)

```
Algoritmo Calculadora
FIM_ALGORITMO
```

#### Teste de mesa (0.5 ponto)

| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |

### Exercício 04 (2.5 pontos)
Elaborar um algoritmo que, dada a idade, classifique nas categorias: infantil A (5 - 7 anos), infantil B (8 -10 anos), juvenil A (11 - 13 anos), juvenil B (14 -17 anos) e adulto (maiores que 18 anos).

#### Fluxograma (1.0 ponto)

```mermaid
flowchart TD
A([INICIO]) --> B([FIM])
```

#### Pseudocódigo (1.0 ponto)

```
Algoritmo ClassificaCategoria
FIM_ALGORITMO
```

#### Teste de mesa (0.5 ponto)

| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |
