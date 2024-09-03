### QUESTAO 1
```python
def fibonacci_sequence(limit):

    # 2 primeiros numeros da sequencia
    sequence = [0, 1]

    # sequence[-1] é o ultimo numero da lista
    while sequence[-1] < limit:
        # soma dos ultimos dois valores da lista
        next_value = sequence[-1] + sequence[-2]
        sequence.append(next_value)
    return sequence


def is_in_fibonacci(number):
    if number < 0:
        return False

    sequence = fibonacci_sequence(number)
    return number in sequence


number_to_check = int(input(
    "Informe um número para verificar se ele pertence à sequência de Fibonacci: "))

if is_in_fibonacci(number_to_check):
    print(f"O número {number_to_check} pertence à sequência de Fibonacci.")
else:
    print(f"O número {number_to_check} NÃO pertence à sequência de Fibonacci.")
```

### QUESTAO 2
```python
def verificar_letra_a(texto):

    quantidade = texto.lower().count('a')

    if quantidade > 0:
        print(f"A letra 'a' (maiúscula ou minúscula) aparece {quantidade} vez(es) na string.")
    else:
        print("A letra 'a' (maiúscula ou minúscula) não aparece na string.")


string_usuario = input("Informe uma string: ")
verificar_letra_a(string_usuario)
```

### QUESTAO 3
Resposta: 77

### QUESTAO 4
a)9   b)128  c)49   d)100   e)13   f)20


### QUESTAO 5
Primeiro, você liga o interruptor 1 por 5 minutos e depois desliga. Em seguida, liga o interruptor 2 e vai direto para as salas.

Se a lâmpada estiver acesa, ela é do interruptor 2.
Se estiver apagada, mas quente, é do interruptor 1.
Se estiver apagada e fria, é do interruptor 3.
Depois, como você já sabe a qual lâmpada pertence um interruptor, só precisa ligar um dos outros dois e ir para a próxima sala.

Assim, você descobre a qual interruptor pertencem as outras duas lâmpadas.