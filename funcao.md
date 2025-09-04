# Revisão do Uso de Funções em Python

As funções em Python são um dos principais blocos de construção da programação. Elas permitem que você escreva código reutilizável, organizado e modular. Este documento fornece uma visão abrangente sobre como definir, chamar e usar funções em Python.

## O Que é uma Função?

Uma função é um bloco de código que executa uma tarefa específica. Uma função pode receber dados como entrada (argumentos) e pode retornar um valor como saída.

### Definindo uma Função

Para definir uma função, usamos a palavra-chave `def`, seguida pelo nome da função e parênteses. Dentro dos parênteses, você pode especificar os parâmetros da função.

```python
def nome_da_funcao(parametro1, parametro2):
    # Código da função
    return resultado
```

#### Exemplo:

```python
def soma(a, b):
    resultado = a + b
    return resultado
```

### Chamando uma Função

Para chamar uma função, basta usar o nome da função seguido por parênteses, passando os argumentos que a função espera.

```python
resultado = soma(3, 5)
print(resultado)  # Saída: 8
```

## Funções com Parâmetros Padrão

Você pode definir valores padrão para os parâmetros. Se um argumento não for fornecido ao chamar a função, o valor padrão será usado.

```python
def saudacao(nome="Mundo"):
    return f"Olá, {nome}!"

print(saudacao())        # Saída: Olá, Mundo!
print(saudacao("Ana"))   # Saída: Olá, Ana!
```

## Funções com Número Variável de Argumentos

Use `*args` para passar um número variável de argumentos não nomeados e `**kwargs` para passar um número variável de argumentos nomeados.

### Exemplos:

```python
def soma_varios(*args):
    return sum(args)

print(soma_varios(1, 2, 3, 4))  # Saída: 10

def mostrar_informacoes(**kwargs):
    for chave, valor in kwargs.items():
        print(f"{chave}: {valor}")

mostrar_informacoes(nome="Ana", idade=30)  # Saída: nome: Ana, idade: 30
```

## Funções Lambda

Funções lambda são funções anônimas que podem ter múltiplos argumentos, mas apenas uma expressão. Elas são frequentemente usadas para tornar o código mais conciso, especialmente em operações gráficas como `map`, `filter` e `sorted`.

### Sintaxe

```python
lambda argumentos: expressão
```

### Exemplos:

```python
# Função lambda para somar dois números
soma = lambda a, b: a + b
print(soma(3, 4))  # Saída: 7

# Função lambda para elevar um número ao quadrado
quadrado = lambda x: x ** 2
print(quadrado(5))  # Saída: 25

# Usando com map
numeros = [1, 2, 3]
quadrados = list(map(lambda x: x**2, numeros))
print(quadrados)  # Saída: [1, 4, 9]
```

## Escopo de Variáveis

As funções têm seu próprio escopo, o que significa que as variáveis definidas dentro de uma função não são visíveis fora dela.

### Exemplo:

```python
def funcao_exemplo():
    x = 5  # x é local para esta função
    return x

print(funcao_exemplo())  # Saída: 5
# print(x)  # Isso causaria um erro, pois x não está definido aqui.
```

## Funções Recursivas

Funções recursivas são aquelas que se chamam a si mesmas. Elas são úteis para resolver problemas que podem ser divididos em subproblemas menores.

### Exemplo:

```python
def fatorial(n):
    if n <= 1:
        return 1
    else:
        return n * fatorial(n - 1)

print(fatorial(5))  # Saída: 120
```

## Práticas Recomendadas

- **Nomes Descritivos**: Use nomes de funções descritivos para que o propósito da função seja claro.
- **Documentação**: Utilize docstrings para descrever a função, seus parâmetros e o que ela retorna.
  
```python
def soma(a, b):
    """Retorna a soma de a e b."""
    return a + b
```

- **Evitar Efeitos Colaterais**: Minimize o uso de variáveis globais dentro das funções para evitar efeitos colaterais indesejados.

As funções são fundamentais na organização e reutilização de código em Python. Dominar o uso de funções é essencial para qualquer programador Python, pois elas tornam o código mais legível e fácil de manter.
```
