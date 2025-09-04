# Revisão de Conceitos em Python

Este documento fornece uma análise detalhada de diversos conceitos fundamentais em Python, incluindo a manipulação de variáveis, tipagem, operadores, strings e interpolação. Abaixo estão exemplos de código com explicações.

## 1. Introdução ao Python

```python
print("Olá, mundo!")
```
Este é um exemplo simples que imprime a mensagem `"Olá, mundo!"` no console. Funciona como uma introdução ao uso de funções em Python.

## 2. Variáveis

As variáveis são usadas para armazenar dados. Você pode atribuir valores a elas utilizando o sinal de igual (`=`).

### Exemplo de Atribuição

```python
nome = "Maria"
nome2 = "Carlos"
```

Aqui, `nome` e `nome2` são variáveis que armazenam strings. 

### Comparação

```python
print(nome == nome2)  # False
```

O operador `==` é usado para comparar se os valores das variáveis são iguais. Nesse caso, a comparação resulta em `False` porque "Maria" não é igual a "Carlos".

## 3. Tipos de Dados

Os tipos de dados em Python são: 
- **String (str)**: Sequência de caracteres.
- **Inteiro (int)**: Números inteiros sem parte decimal.
- **Ponto Flutuante (float)**: Números com parte decimal.
- **Booleano (bool)**: Valores verdadeiros ou falsos.

### Exemplo de Tipagem Dinâmica

```python
numero = "10"  # string 
numero = 15    # inteiro
numero = 10.5  # ponto flutuante 
numero = True  # booleano 
```

Python é uma linguagem de tipagem dinâmica, o que significa que você pode mudar o tipo de uma variável ao longo do tempo.

## 4. Conversão de Tipos

Você pode converter entre tipos usando funções integradas:

```python
numero_float = int(10.5)  # Conversão de float para int
print(numero_float)  # Saída: 10

text_bool = bool(152487563255) 
print(text_bool)  # Saída: True

numero_bool = str(text_bool)
print(type(numero_bool))  # Saída: <class 'str'>, "True" como string
```

### Conversões Comuns

- `int()`: Converte para inteiro.
- `str()`: Converte para string.
- `float()`: Converte para ponto flutuante.
- `bool()`: Converte para booleano.

## 5. Operadores de Comparação

Os operadores de comparação permitem comparar valores. 

| Operador  | Descrição                     | Exemplo      |
|-----------|-------------------------------|--------------|
| `<`       | Menor que                     | `3 < 5`      |
| `>`       | Maior que                     | `5 > 3`      |
| `<=`      | Menor ou igual                | `3 <= 5`     |
| `>=`      | Maior ou igual                | `5 >= 5`     |
| `==`      | Igual a                       | `5 == 5`     |
| `!=`      | Diferente de                  | `5 != 3`     |

### Exemplos

```python
print(3 < 5)  # True
print(5 != 3)  # True
```

## 6. Operadores Aritméticos

Os operadores aritméticos permitem realizar cálculos matemáticos.

### Exemplo de Operações

```python
# Adição
resultado = 10 + 5
print("Resultado da adição:", resultado)  # Saída: 15

# Subtração
resultado = 10 - 5
print("Resultado da subtração:", resultado)  # Saída: 5

# Multiplicação
resultado = 10 * 5
print("Resultado da multiplicação:", resultado)  # Saída: 50

# Divisão
resultado = 10 / 5
print("Resultado da divisão:", resultado)  # Saída: 2.0

# Divisão Inteira
resultado = 125 // 4 
print("Resultado da divisão inteira:", resultado)  # Saída: 31

# Módulo
resultado = 13 % 5
print("Resultado do módulo:", resultado)  # Saída: 3

# Exponenciação
resultado = 2 ** 3
print("Resultado da exponenciação:", resultado)  # Saída: 8
```

## 7. Comparação de Identidade

O operador `is` compara se duas variáveis referenciam o mesmo objeto em memória. O operador `is not` verifica se não são o mesmo objeto.

### Exemplo

```python
numero = 10
numero2 = 5010

verificacao = numero is not numero2
print(verificacao)  # Saída: True
```

## 8. Manipulação de Strings

Strings são sequências de caracteres. Veja alguns exemplos de manipulação de strings:

### Exemplo de Criação de Strings

```python
nome = "Maria"
sobrenome = "Carmargo"
idade = 60
cpf = "148-9658-965-02"
```

### Concatenando Strings

Você pode concatenar strings usando o operador `+` ou usando f-strings para formatação:

```python
print(f"Nome completo: {nome} {sobrenome}, tem {idade} anos! E possui o CPF {cpf}")
```

### Repetindo Strings

```python
nome3x = nome * 5
print(nome3x)  # Saída: MariaMariaMariaMariaMaria
```

### Acessando Caracteres

```python
print(nome[0])  # Saída: M
```

### Tamanho de Strings

```python
print(len(nome))  # Retorna o comprimento da string
```

### Fatiamento de Strings

Você pode acessar partes de strings através de índices e fatiamento:

```python
print(nome[0:3])  # Saída: Mar
print(nome[:3])    # Saída: Mar (até o índice 2)
print(nome[1:])    # Saída: aria (do índice 1 em diante)
```

### Invertendo uma String

```python
print(nome[::-1])  # Saída: airam
```

### Exemplo com Inclusão e Conteúdo

```python
sorvete = "Pistache com chocolate"
print("tac" in sorvete[0:11])  # Verifica se 'tac' está no fatiamento
```

## 9. Métodos de String

Veja alguns métodos úteis para manipular strings:

```python
print("VidA".lower())  # Converte para minúscula
```

## 10. Interpolação de Strings

A interpolação de strings permite incluir variáveis no texto:

```python
nome = "Ford"
marca = "Mustang"
print("Os carros da %s são bonitos e os da %s são ainda mais bonitos!" % (nome, marca))
```

## 11. Conclusão

Este documento revisa diversos conceitos fundamentais do Python, incluindo variáveis, tipos de dados, operadores, condições e manipulação de strings. Compreender estes fundamentos é essencial para escrever programas em Python e facilita o aprendizado de conceitos mais avançados.
```

