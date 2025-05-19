# Lista de Exercícios

**Conteúdos:**  
- Operadores (aritméticos, relacionais, lógicos, atribuição)  
- Estruturas condicionais (`if`, `elif`, `else`)  
- Estruturas de repetição (`for`, `while`)  
- Manipulação básica de arquivos (`open()`, leitura/escrita)

---

## 1. Academia em Números

Uma academia está registrando dados dos seus clientes: nome, idade e tempo de treino (em meses).  
Você deve:

1. Ler esses dados para **10 clientes**.
2. Exibir:
   - Quantas pessoas têm **mais de 1 ano** de treino.
   - Quantas pessoas têm **menos de 18 anos**.
   - A **média de idade** geral.

---

## 2. Cálculo de Salário com Bônus

Uma empresa paga aos seus funcionários um bônus de fim de ano com base em critérios:

- Salário **até R$1500** → bônus de **20%**
- Salário **entre R$1501 e R$3000** → bônus de **10%**
- Salário **acima de R$3000** → bônus de **5%**

Peça ao usuário o salário de **5 funcionários** e exiba o valor do bônus de cada um, junto com o valor final (salário + bônus).

---

## 3. Jogo de Adivinhação (While + Condicionais)

Crie um programa onde:

- O computador escolhe um número secreto entre 1 e 20.
- O usuário tenta adivinhar esse número.
- O programa dá dicas: `"maior"` ou `"menor"`.
- O jogo termina quando o número for acertado, mostrando quantas tentativas foram necessárias.

*Dica:* use `random.randint()` para sortear o número.

---

## 4. Registro de Produtos com Arquivo

Escreva um programa que:

1. Peça ao usuário para digitar o nome de **5 produtos** (um por vez).
2. Armazene cada nome em uma linha do arquivo `produtos.txt`.
3. Depois da escrita, abra o arquivo para leitura e:
   - Mostre todos os produtos.

---

## 5. Temperaturas Extremas

Você deve receber a **temperatura máxima** de cada dia da semana (segunda a domingo).  
O programa deve exibir:

- A temperatura **mais alta** e o **dia correspondente**.
- A temperatura **mais baixa** e o **dia correspondente**.
- A **média semanal** das temperaturas.

---

## 6. Cadastro de Alunos (Condicional + Atribuição)

Você precisa registrar os dados de **6 alunos**, capturando:

- Nome
- Nota final

Depois, exiba:

- A quantidade de alunos **aprovados** (nota ≥ 7).
- A quantidade de alunos **reprovados**.
- A **nota mais alta** entre todos.
- A média geral da turma.

---

## 7. Controle de Estoque

Peça ao usuário a **quantidade inicial** de produtos em estoque.  
Depois, use um `while` para simular a venda de produtos:

- A cada iteração, pergunte quantos produtos foram vendidos.
- Atualize o estoque com `-=` (atribuição).
- Quando o estoque chegar a **zero**, exiba `"Estoque zerado!"` e pare.

*Evite permitir vendas maiores do que o estoque disponível.*

---

## 8. Verificação de CPF

Peça ao usuário para digitar **10 números de CPF** (sem formatação).  
Para cada CPF:

- Verifique se ele possui **11 dígitos**.
- Se não possuir, exiba: `"CPF inválido"`.
- Se for válido, escreva-o no arquivo `cpfs_validos.txt`.

*Dica:* use `len()` para contar os dígitos.

---

## 9. Desafio das Operações

Sem usar Python, diga o resultado (ou tipo de resultado) das seguintes expressões:

a) `7 + 4 * 2`  
b) `(7 + 4) * 2`  
c) `18 / 3 + 2`  
d) `18 // 4 * 2`  
e) `10 % 3 + 4`  
f) `3 ** 2 == 9 and 5 < 10`  
g) `not 7 > 3`  
