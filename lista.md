

```markdown
# Lista e  introdução às Estruturas de Dados em Python

Este documento explica várias estruturas de dados e operações comuns em listas utilizando Python. Ele cobre listas, loops, pilhas (LIFO) e filas (FIFO) com exemplos.

## Listas

As listas são uma coleção de elementos que podem conter diferentes tipos de dados, incluindo números, strings e outros objetos. Aqui estão algumas operações comuns:

### Criação de Listas

```python
lista_num = [10, 5, 3, 4, 6, 7, 8, 9, 1, 2]
lista_heterogenea = [10, "hola", 3.5, True, 6, "adios", 8.9, False, 1, 2]
```

- **`lista_num`**: Uma lista contendo apenas números.
- **`lista_heterogenea`**: Uma lista que contém diferentes tipos de dados, incluindo inteiro, string, float e booleano.

### Listas Vazias e Repetição de Elementos

```python
lista_vazia = []
lista_milti = [12] * 5
print(lista_milti)  # Saída: [12, 12, 12, 12, 12]
```

- **`lista_vazia`**: Uma lista sem elementos.
- **`lista_milti`**: Uma lista que contém cinco elementos com valor 12.

### Manipulação de Listas

```python
lista_nomes = ["Ana", "Maria", "João", "Pedro"]

# Acessando elementos
# Impressão do primeiro e segundo elemento
print(lista_nomes[0:2])  # Saída: ['Ana', 'Maria']
```

- **Slicing**: O exemplo mostra como acessar um subconjunto da lista.

### Iteração sobre a Lista

#### Usando `for`

```python
for nome in lista_nomes:
    print(f"Olá {nome}")
```

- Este loop imprime uma saudação para cada nome na lista.

#### Usando `while`

```python
indice = 0
while indice < len(lista_nomes):
    print(f"Olá {lista_nomes[indice]} - indice {indice}")
    indice += 1
```

- Este loop imprime os nomes junto com seus índices.

#### Usando `enumerate`

```python
for i, el in enumerate(lista_nomes):
    print(f"Olá {el} - indice {i}")
```

- `enumerate` permite iterar com o índice e o valor ao mesmo tempo.

## Concatenando Listas

```python
lista2 = ['Maçã', 'Banana']
lista3 = lista_nomes + lista2
print(lista3)  # Combinação das duas listas
```

- **Concatenação**: Combina `lista_nomes` e `lista2` em uma nova lista `lista3`.

## Convertendo String em Lista

```python
soletrar = list("Africa")
print(soletrar)  # Saída: ['A', 'f', 'r', 'i', 'c', 'a']
```

- A função `list` converte uma string em uma lista de caracteres.

## Checando Pertinência de Elementos

```python
print("6" not in lista2)  # Saída: True
```

- Verifica se um elemento não está presente na lista.

## Listas Vazia e Booleana

```python
lista_v = []
print(len(lista_v))  # Saída: 0
print(bool(lista_v))  # Saída: False (listas vazias são consideradas False)
```

- **`len`**: Retorna o número de elementos na lista.
- **`bool`**: Converte a lista em um valor booleano.

## Manipulação de Elementos em Listas

```python
# Adicionando elementos
lista_frutas = [1.5, 2.5, 3.0]
lista_frutas.append("banana")
print(lista_frutas)

# Removendo elementos
lista_frutas.remove(2.5)
print(lista_frutas)

# Removendo pelo índice
lista_frutas.pop(1)
print(lista_frutas)

# Inserindo um elemento em um índice específico
lista_frutas.insert(1, "morango")
print(lista_frutas)
```

- **`append`**: Adiciona um elemento ao final da lista.
- **`remove`**: Remove um elemento específico.
- **`pop`**: Remove e retorna um elemento do índice especificado.
- **`insert`**: Insere um elemento em um índice específico.

## Ordenação e Inversão de Listas

```python
lista_frutas = [10, 5, 0, 2, 50]
lista_frutas.sort()  # Ordena a lista em ordem crescente
print(lista_frutas)   # Saída: [0, 2, 5, 10, 50]

lista_frutas.reverse()  # Inverte a lista
print(lista_frutas)      # Saída: [50, 10, 5, 2, 0]
```

### Spreading (Expandindo Listas)

```python
lista_n = [1, 2, 3, 4, 5]
lista_x = [10, 9, 6, *lista_n, 20]
print(lista_x)  # Saída: [10, 9, 6, 1, 2, 3, 4, 5, 20]
```

- **`*` operator**: Expande os elementos da lista `lista_n` na nova lista `lista_x`.

## Estruturas de Dados: Pilhas e Filas

### Pilha (LIFO - Last In First Out)

Em uma pilha, o último elemento a ser adicionado é o primeiro a ser removido.

```python
pilha = []
pilha.append(1)
pilha.append(2)
pilha.append(3)
print(pilha)  # Saída: [1, 2, 3]
pilha.pop()   # Remove o último elemento (3)
print(pilha)  # Saída: [1, 2]
```

- **`append`**: Adiciona um elemento ao topo da pilha.
- **`pop`**: Remove o elemento do topo.

### Fila (FIFO - First In First Out)

Em uma fila, o primeiro elemento a ser adicionado é o primeiro a ser removido.

```python
fila = []
fila.append(1)
fila.append(2)
fila.append(3)
print(fila)   # Saída: [1, 2, 3]
fila.pop(0)   # Remove o primeiro elemento (1)
print(fila)   # Saída: [2, 3]
```

- **`append`**: Adiciona um elemento ao final da fila.
- **`pop(0)`**: Remove o primeiro elemento da fila.

## Conclusão

Este documento apresentou uma variedade de conceitos e operações que podem ser realizadas com listas em Python, além de estruturas para pilhas e filas. Entender essas estruturas de dados é fundamental para a programação e o desenvolvimento de algoritmos em Python.
```

### Como Usar

- **Copie e cole** o conteúdo acima em um arquivo de texto ou um editor de Markdown.
- **Visualização**: Você pode visualizar o Markdown usando um editor que suporte esta formatação ou em plataformas como GitHub, que renderizam automaticamente arquivos Markdown (com extensão `.md`).

Essas explicações e exemplos permitem que você entenda cada aspecto do código apresentado na aula. Se precisar de mais informações ou ajustes, fique à vontade para pedir!