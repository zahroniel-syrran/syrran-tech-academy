# Interpretação lógica dos exercícios para criação de programas em C++

## Exercícios de lógica e repetição em C++

- Modalidade: em Dupla (Dividam os exercícios)
- Entrega: GitHub

Este material reorganiza os exercícios e explica **como pensar logicamente** na construção do programa em **C++**, sem apresentar a solução pronta.  
A ideia é ajudar o aluno a identificar **entradas**, **processamento**, **saídas**, estruturas de repetição, testes condicionais e variáveis de controle.

---

## Exercício 1

### Enunciado
Ler um número inteiro. Verificar e exibir se o número é primo.

### Como interpretar logicamente
Um número primo é aquele que possui **apenas dois divisores exatos**: 1 e ele mesmo.  
A lógica do exercício é testar se existem outros divisores além desses.

### O que o programa precisa fazer
- Ler um número inteiro.
- Verificar quantas divisões exatas ele possui.
- Informar se é primo ou não.

### Entradas
- Um número inteiro.

### Processamento
- Testar divisões possíveis.
- Verificar se existe divisor além de 1 e do próprio número.

### Saídas
- Mensagem informando se o número é primo ou não.

### Raciocínio para montar o programa
1. Ler o número.
2. Pensar em como testar divisores.
3. Criar uma variável de apoio para controlar se encontrou divisor.
4. Repetir os testes com laço.
5. Exibir o resultado final.

### Exemplo para pensar
Se o número for **7**, ele só divide exatamente por **1** e **7**.  
Se o número for **8**, ele também divide por **2** e **4**, então não é primo.

### Atenção lógica
- Números menores que 2 precisam de atenção especial.
- Não basta testar apenas uma divisão; é necessário analisar os possíveis divisores.

---

## Exercício 2

### Enunciado
Ler um número inteiro, calcular e exibir separadamente as potências de 2^0 até 2^(esse número).

### Como interpretar logicamente
O exercício pede uma sequência de potências de base 2, começando em **2^0** e terminando em **2 elevado ao número lido**.

### O que o programa precisa fazer
- Ler um número inteiro.
- Gerar todas as potências de 2 nesse intervalo.
- Exibir cada resultado separadamente.

### Entradas
- Um número inteiro.

### Processamento
- Repetir de 0 até o valor informado.
- Calcular a potência correspondente a cada passo.

### Saídas
- Lista das potências de 2.

### Raciocínio para montar o programa
1. Ler o número.
2. Criar um laço de repetição começando em 0.
3. Em cada repetição, calcular a potência atual.
4. Mostrar o expoente e o valor encontrado.

### Exemplo para pensar
Se o número lido for **4**, a saída deverá exibir os resultados de:
- 2^0
- 2^1
- 2^2
- 2^3
- 2^4

### Atenção lógica
- O programa deve mostrar cada potência separadamente.
- Pense se vai calcular diretamente ou aproveitar o resultado anterior.

---

## Exercício 3

### Enunciado
Ler vários números até que seja digitado um número negativo. Calcular e exibir a soma desses números.

### Como interpretar logicamente
Esse exercício usa **repetição com condição de parada**.  
O programa deve continuar lendo valores até aparecer um número negativo, que encerra a entrada.

### O que o programa precisa fazer
- Ler números sucessivamente.
- Somar os números válidos.
- Parar quando um número negativo for digitado.
- Exibir a soma final.

### Entradas
- Vários números inteiros ou reais, um de cada vez.

### Processamento
- Acumular a soma dos números digitados.
- Interromper a repetição quando encontrar valor negativo.

### Saídas
- Soma dos números lidos antes do número negativo.

### Raciocínio para montar o programa
1. Criar uma variável acumuladora para a soma.
2. Ler um número.
3. Verificar se ele é negativo.
4. Se não for, somar ao acumulador.
5. Repetir até a condição de parada.

### Exemplo para pensar
Entradas:
- 5
- 8
- 2
- -1

Nesse caso, o **-1** serve para parar e não entra na soma.

### Atenção lógica
- O valor negativo normalmente é apenas o sinal de parada.
- Pense bem na ordem: ler, testar, somar ou parar.

---

## Exercício 4

### Enunciado
Ler 10 números. Verificar e exibir o menor e maior número dessa sequência.

### Como interpretar logicamente
O objetivo é comparar os valores digitados e descobrir qual é o menor e qual é o maior da sequência.

### O que o programa precisa fazer
- Ler 10 números.
- Comparar os valores ao longo da leitura.
- Guardar o menor e o maior encontrados.
- Exibir os dois resultados.

### Entradas
- 10 números.

### Processamento
- Comparar cada novo número com o menor atual e com o maior atual.

### Saídas
- Menor número da sequência.
- Maior número da sequência.

### Raciocínio para montar o programa
1. Ler o primeiro número e usá-lo como referência inicial.
2. Guardar esse valor como menor e maior temporariamente.
3. Ler os demais números.
4. Atualizar menor e maior quando necessário.
5. Exibir o resultado ao final.

### Exemplo para pensar
Se a sequência for:
12, 5, 18, 3, 9, 21, 7, 10, 4, 15

O programa deve identificar:
- menor = 3
- maior = 21

### Atenção lógica
- É comum errar a inicialização das variáveis menor e maior.
- Usar o primeiro valor lido como base costuma facilitar.

---

## Exercício 5

### Enunciado
Ler um número para a parada final e outro número que representa um múltiplo. Exibir os múltiplos do número lido de 1 até o número final lido.

### Como interpretar logicamente
O programa deve mostrar os múltiplos de um número dentro de um intervalo que vai de 1 até um valor final informado.

### O que o programa precisa fazer
- Ler o valor final.
- Ler o número base dos múltiplos.
- Encontrar quais valores, até o limite, são múltiplos desse número.
- Exibir esses valores.

### Entradas
- Um número final.
- Um número que será usado como base dos múltiplos.

### Processamento
- Percorrer os números do intervalo.
- Verificar quais são múltiplos do número base.

### Saídas
- Lista dos múltiplos encontrados.

### Raciocínio para montar o programa
1. Ler o limite final.
2. Ler o número base.
3. Criar um laço de 1 até o limite.
4. Testar se cada valor atende à condição de múltiplo.
5. Exibir apenas os que servem.

### Exemplo para pensar
Se o valor final for **20** e o múltiplo for **4**, devem aparecer:
4, 8, 12, 16 e 20.

### Atenção lógica
- Verifique se o número final será incluído.
- Pense em como identificar que um número é múltiplo de outro.

---

## Exercício 6

### Enunciado
Ler vários números até que a soma desses números seja maior que 100. Exibir a multiplicação dos números lidos.

### Como interpretar logicamente
Esse exercício trabalha com duas ideias ao mesmo tempo:
- parar quando a soma passar de 100;
- multiplicar todos os números lidos até esse ponto.

### O que o programa precisa fazer
- Ler números sucessivamente.
- Somar os valores lidos.
- Multiplicar os valores lidos.
- Parar quando a soma ultrapassar 100.
- Exibir o produto final.

### Entradas
- Vários números.

### Processamento
- Acumular a soma.
- Acumular a multiplicação.
- Encerrar quando a soma for maior que 100.

### Saídas
- Resultado da multiplicação dos números lidos.

### Raciocínio para montar o programa
1. Criar uma variável para a soma.
2. Criar uma variável para a multiplicação.
3. Ler um número por vez.
4. Atualizar soma e multiplicação.
5. Verificar a condição de parada.
6. Exibir o resultado final.

### Exemplo para pensar
Se forem digitados:
20, 30, 25, 40

A soma passa de 100 no último valor, então o programa para após esse ponto.

### Atenção lógica
- A variável da multiplicação não deve começar com zero.
- Pense se o último número lido entra ou não no cálculo. O enunciado sugere que sim.

---

## Exercício 7

### Enunciado
Ler a quantidade de pessoas e ler a altura dessas pessoas. Calcular e exibir a altura média de todas as pessoas.

### Como interpretar logicamente
O exercício pede a média das alturas.  
Para isso, é necessário:
1. somar todas as alturas;
2. dividir pela quantidade de pessoas.

### O que o programa precisa fazer
- Ler a quantidade de pessoas.
- Ler a altura de cada pessoa.
- Somar todas as alturas.
- Calcular a média.
- Exibir o resultado.

### Entradas
- Quantidade de pessoas.
- Altura de cada pessoa.

### Processamento
- Somar as alturas.
- Dividir a soma pela quantidade de pessoas.

### Saídas
- Altura média do grupo.

### Raciocínio para montar o programa
1. Ler a quantidade de pessoas.
2. Criar uma variável acumuladora para as alturas.
3. Repetir a leitura das alturas conforme a quantidade informada.
4. Calcular a média ao final.
5. Mostrar o resultado.

### Exemplo para pensar
Se forem 3 pessoas com alturas:
1.70, 1.80 e 1.60

A média será a soma dessas alturas dividida por 3.

### Atenção lógica
- Altura normalmente exige variável do tipo real.
- Evite divisão inteira quando o resultado deve ter casas decimais.

---

## Exercício 8

### Enunciado
Ler um número. Exiba a soma de todos os números pares e ímpares de zero até o número lido.

### Como interpretar logicamente
O programa deve percorrer os números de 0 até o valor informado e separar a soma em dois grupos:
- soma dos pares;
- soma dos ímpares.

### O que o programa precisa fazer
- Ler um número.
- Percorrer todos os valores de 0 até esse número.
- Verificar quais são pares e quais são ímpares.
- Somar separadamente.
- Exibir os dois resultados.

### Entradas
- Um número inteiro.

### Processamento
- Repetir de 0 até o número lido.
- Testar se cada valor é par ou ímpar.
- Atualizar o acumulador correspondente.

### Saídas
- Soma dos números pares.
- Soma dos números ímpares.

### Raciocínio para montar o programa
1. Ler o número final.
2. Criar duas variáveis acumuladoras.
3. Fazer um laço no intervalo solicitado.
4. Testar cada valor.
5. Somar no grupo correto.
6. Exibir os totais separados.

### Exemplo para pensar
Se o número for **6**, os valores analisados serão:
0, 1, 2, 3, 4, 5, 6

O programa deve separar a soma dos pares da soma dos ímpares.

### Atenção lógica
- Zero é número par.
- O exercício pede duas somas diferentes, não uma única soma total.

---

## Exercício 9

### Enunciado
Ler um número entre 50 e 100. Exibir a sequência de Fibonacci até esse número.

### Como interpretar logicamente
A sequência de Fibonacci é formada a partir da soma dos dois termos anteriores.  
O exercício pede que a sequência seja gerada até atingir o limite informado.

### O que o programa precisa fazer
- Ler um número entre 50 e 100.
- Gerar a sequência de Fibonacci.
- Exibir os termos até o valor limite.

### Entradas
- Um número entre 50 e 100.

### Processamento
- Controlar os termos da sequência.
- Gerar o próximo valor com base nos dois anteriores.
- Parar quando ultrapassar o limite.

### Saídas
- Sequência de Fibonacci até o número informado.

### Raciocínio para montar o programa
1. Ler o número limite.
2. Validar se ele está no intervalo pedido.
3. Criar variáveis para os termos da sequência.
4. Exibir os primeiros termos.
5. Gerar os próximos até o limite.
6. Parar no momento correto.

### Exemplo para pensar
A sequência começa assim:
0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55...

Se o limite for **50**, o programa deve decidir até qual termo mostrar sem ultrapassar a regra proposta.

### Atenção lógica
- O exercício pede um intervalo específico para a entrada.
- É importante controlar corretamente os dois termos anteriores.

---

## Exercício 10

### Enunciado
Simule um jogo de adivinhação. O programa deve gerar um número aleatório e o jogador precisa acertar o número. Cada vez que o jogador informar o número, deve exibir se o palpite é muito alto, muito baixo ou correto. Quando for correto, exibir a quantidade de palpites.

### Como interpretar logicamente
Esse exercício mistura:
- geração de número aleatório;
- repetição;
- comparação;
- contagem de tentativas.

### O que o programa precisa fazer
- Gerar um número aleatório.
- Ler palpites do jogador.
- Comparar o palpite com o número sorteado.
- Informar se o palpite é maior, menor ou correto.
- Contar quantas tentativas foram feitas.
- Encerrar quando acertar.

### Entradas
- Palpites do jogador.

### Processamento
- Gerar o número secreto.
- Comparar cada palpite.
- Atualizar o contador de tentativas.

### Saídas
- Mensagens de orientação:
  - muito alto
  - muito baixo
  - correto
- Quantidade de palpites ao final.

### Raciocínio para montar o programa
1. Gerar o número aleatório.
2. Criar uma variável para contar tentativas.
3. Ler um palpite.
4. Comparar com o número secreto.
5. Exibir a dica correspondente.
6. Repetir até acertar.
7. Mostrar a quantidade total de palpites.

### Exemplo para pensar
Se o número secreto for **37**:
- palpite 50 → muito alto
- palpite 20 → muito baixo
- palpite 37 → correto

### Atenção lógica
- O programa deve continuar até o acerto.
- É importante contar todas as tentativas.
- Em C++, esse exercício normalmente exige biblioteca para números aleatórios.

---

# Modelo mental para resolver qualquer exercício em C++

Antes de programar, tente sempre responder estas 3 perguntas:

## 1. O que entra no programa?
São os dados que o usuário vai digitar.  
Esses dados virarão variáveis de entrada.

## 2. O que o programa faz com esses dados?
É a parte do processamento.  
Pode envolver:
- comparações
- contadores
- acumuladores
- laços de repetição
- testes condicionais
- cálculos matemáticos

## 3. O que sai do programa?
São os resultados que precisam ser mostrados na tela.

---

# Estrutura lógica básica em C++

Quase todos esses exercícios seguem esta ideia:

1. Declarar variáveis.
2. Ler os dados com `cin`.
3. Processar com `if`, `for`, `while` ou `do while`.
4. Exibir os resultados com `cout`.

---

# Dicas gerais para estes exercícios

## 1. Identifique o tipo de repetição
Pergunte:
- sei exatamente quantas vezes repete?
- repete até acontecer alguma condição?
- precisa ler pelo menos uma vez?

Isso ajuda a escolher entre:
- `for`
- `while`
- `do while`

## 2. Use variáveis de apoio
Muitos exercícios vão precisar de:
- acumulador de soma
- acumulador de multiplicação
- contador
- menor valor
- maior valor
- variável de controle lógico

## 3. Leia o enunciado em partes
Marque mentalmente:
- **Ler** → entrada
- **Calcular / verificar / testar** → processamento
- **Exibir** → saída

## 4. Faça testes com valores pequenos
Antes de programar, simule no papel:
- quais valores entram?
- o que muda a cada repetição?
- quando o laço deve parar?

---

**Metadata & Attribution**

* **Date:** April 2026

* **Author:** Ronildo A. Ferreira

* **Formato de apoio:** material de interpretação lógica para resolução em C++

