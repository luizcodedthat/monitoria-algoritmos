# Exercícios de Leitura e Construção de Código em Python

## Instruções Gerais
- **Objetivo**: Reconhecer e usar estruturas de forma independente, entendendo cada bloco de código como uma ferramenta.
- **Dicas**: Leia cada questão com calma. Se tiver dúvida sobre a execução ou a ordem, anote passo a passo o que acontece em cada linha.
- **Linguagem simples**: Foque no “o que o código faz?” e não no “por que está assim”.

---

## Parte 1: Leitura de Código

### Questão 1
```python
for i in range(3):
    print("Olá", i)

print("Fim")
```

**Pergunta**: O que este código imprime, linha a linha?

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Lembre-se de que `range(3)` gera os valores 0, 1 e 2. Primeiro, execute cada iteração do `for`, depois execute o `print("Fim")`.

</details>

---

### Questão 2

```python
x = 0
while x < 4:
    x += 2
    print("Valor de x:", x)

print("Loop encerrado")
```

**Pergunta**: Qual será a sequência de saída no console? Explique passo a passo.

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Observe que `x` começa em 0. A cada iteração, soma-se 2 antes de imprimir. Quando o `while` não for mais verdadeiro, ele sai e executa o `print` final.

</details>

---

### Questão 3

```python
soma = 0
for num in range(1, 4):
    if num % 2 == 0:
        soma += num

    else:
        soma += 1
    
print("Resultado final:", soma)
```

**Pergunta**: Qual o valor impresso em “Resultado final” e como foi calculado?

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Percorra cada elemento do intervalo. Se o número for par (`num % 2 == 0`), adicione esse número; senão, adicione 1.

</details>

---

### Questão 4
```python
contador = 5
while contador > 0:
    print(contador)
    contador -= 1

else:
    print("Laço encerrado pelo else")
```

**Pergunta**: O que o código imprime? Note que existe um bloco `else` associado ao `while`.

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Em Python, o `else` após o `while` só é executado se o laço terminar “normalmente” (não por `break`). Aqui, não há `break`.

</details>

---

### Questão 5
```python
arq = open("lista.txt", "w")
for i in range(1, 4):
    arq.write(f"Linha {i}\n")

arq.close()

print("Arquivo escrito")
```

**Pergunta**: Mesmo sem ver o conteúdo de “lista.txt”, explique:
- O que acontece com o arquivo aberto em modo "w".
- Quantas linhas são escritas e qual o texto de cada linha.
- O que é impresso no console.

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Modo `"w"` cria ou limpa o arquivo antes de escrever. O `for i in range(1, 4)` gera i = 1, 2 e 3.

</details>

## Parte 2: Construção de Código
### Questão 6

Escreva um programa que:
- Peça ao usuário um número inteiro “num”.
- Use um for para imprimir todos os valores de 1 até n (inclusive).
- Se o número for menor que 1, imprima “Entrada inválida”.

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Pense em dois blocos:
> - Primeiro, verifique com `if n < 1` e trate o erro.
> - Depois, use `for i in range(1, n+1)` para os valores válidos.

</details>

---

### Questão 7

Crie um programa que calcule a soma de todos os números pares de 2 a 10 (inclusivo), usando while. Imprima o resultado final.

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Inicialize uma variável soma em zero e outra variável `x = 2`. Enquanto `x <= 10`, adicione `x` à soma e incremente `x` de 2 em 2 (ou seja, `x += 2`).

</details>

---

### Questão 8

Você tem um arquivo “dados.txt” que contém números inteiros, um por linha. Escreva um programa que:
- Abra o arquivo em modo leitura.
- Leia cada linha, converta em inteiro e acumule em uma variável soma.
- Feche o arquivo.
- Imprima “Soma total: X” (onde X é o valor de soma).

<details>
  <summary> <strong> 💡 Dica: </strong> </summary>

> Use:
> ```python arq = open("dados.txt", "r")
> for linha in arq:
>     num = int(linha.strip())
>     soma += num
> arq.close()
> ```
> Certifique-se de iniciar `soma = 0` antes do loop.

</details>

---

### Questão 9
Escreva um trecho de código que:
- Receba três notas (float) do usuário: n1, n2 e n3;
- Calcule a média aritmética;
- Use if, elif, else para imprimir:
  - “Aprovado” se a média for ≥ 7;
  - “Recuperação” se a média for ≥ 5 e < 7;
  - “Reprovado” se a média for < 5.

<details>
  <summary> <strong>💡 Dica: </strong> </summary>

> Defina:
> ```python
> media = (n1 + n2 + n3) / 3
> if media >= 7:
>     print("Aprovado")
> 
> elif media >= 5:
>     print("Recuperação")
>
> else:
>     print("Reprovado")
> ```
> Observe a ordem das condições.

</details>

---

### Questão 10

Monte um programa que gere o seguinte padrão no console, usando apenas loops (for/while) e print:

```
*
**
***
****
*****
```

Ou seja, 5 linhas, onde a primeira tem 1 asterisco e a última tem 5.