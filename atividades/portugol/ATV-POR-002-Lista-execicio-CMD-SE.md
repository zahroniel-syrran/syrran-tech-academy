# Interpretação lógica dos exercícios para criação de programas em Portugol


## Exercícios da página 21/22 da apostila de Portugol Studio

Este material reescreve cada exercício e explica **como pensar logicamente** na construção do programa em Portugol, sem apresentar a solução completa pronta.  
A ideia é treinar a identificação de **entradas**, **processamento** e **saídas**.

---

## Instruções para os alunos

O objetivo é discutir os conceitos apresentados, pesquisar informações adicionais e produzir respostas claras e bem explicadas.

### Organização das respostas

As respostas devem:

- ser claras e bem organizadas
- demonstrar compreensão dos conceitos estudados
- apresentar explicações próprias
- evitar apenas copiar definições da internet

#### Uso do GitHub

- cada aluno deve realizar **seus próprios commits**
- o histórico de commits deve demonstrar colaboração
- evitar realizar apenas um único commit final

#### Uso de fontes externas

Caso sejam utilizadas fontes externas:

- incluir as referências utilizadas
- citar corretamente as fontes consultadas
- evitar cópia direta sem explicação própria

---

## Critérios de avaliação

Serão considerados os seguintes critérios:

- clareza e organização das respostas
- qualidade da pesquisa realizada
- aplicação correta dos conceitos estudados
- capacidade de explicação e argumentação
- organização do documento entregue
- participação dos integrantes no repositório GitHub

---

## Referências

Materiais recomendados para estudo:

- Documentação do Portugol Studio  
  https://portugol.dev

- Python para Zumbis (material introdutório de programação)  
  https://pythondozero.com.br

- Livro: **Algoritmos – Lógica para Desenvolvimento de Programação**  
  Autor: Edécio Fernando Iepsen

- Livro: **Introdução à Programação com Python**  
  Autor: Nilo Ney Coutinho Menezes

- Curso em Vídeo — Lógica de Programação  
  https://www.cursoemvideo.com

---


# 📘 Conhecimentos necessários para resolução dos exercícios

## 1. Declaração de Variáveis

Em **Portugol**, as variáveis são utilizadas para **armazenar dados** lidos pelo programa e também os **resultados de cálculos**.

👉 Elas são fundamentais para que o programa consiga **processar informações**.

---

### 🔹 Tipos mais utilizados

| Tipo       | Uso comum                                         |
| ---------- | ------------------------------------------------- |
| `inteiro`  | Idades, anos, quantidades, classificações         |
| `real`     | Valores com casas decimais (preços, médias, etc.) |
| `caracter` | Leitura de um único símbolo (letra ou caractere)  |

---

### 💡 Exemplo prático

Guardar um ano, um preço e uma letra:

```
inteiro ano
real preco
caracter letra
```

✔️ `ano` → armazena valores inteiros

✔️ `preco` → armazena valores com decimais

✔️ `letra` → armazena um único caractere


---

### 🔎 Dica

Escolher o tipo correto de variável é importante para:

* Evitar erros no programa
* Garantir cálculos corretos
* Organizar melhor a lógica

---

### ✅ Resumo

✔️ Variáveis guardam dados durante a execução

✔️ Cada tipo atende a uma necessidade específica

✔️ Sempre declare antes de usar

👉 Esse conceito é a base de qualquer programa.

---

## 2. Entrada de Dados com `leia`

O comando `leia` é utilizado para **receber valores digitados pelo usuário** e armazená-los em variáveis.

👉 Ele permite que o programa interaja com o usuário, capturando dados para processamento.

---

### 🔹 Como funciona

```
leia(variavel)
```

✔️ O valor digitado será armazenado na variável informada

✔️ A variável deve estar **declarada previamente**

---

### 💡 Exemplo 1: Ler a idade de uma pessoa

**Objetivo:** armazenar a idade informada pelo usuário

```
inteiro idade
leia(idade)
```

✔️ O valor digitado será guardado na variável `idade`

---

### 💡 Exemplo 2: Ler diferentes tipos de dados

**Objetivo:** armazenar um ano, um preço e uma letra

```
inteiro ano
real preco
caractere letra

leia(ano)
leia(preco)
leia(letra)
```

✔️ Cada variável recebe um valor correspondente ao seu tipo

✔️ A ordem da leitura deve seguir a lógica do programa

---

### 🔎 Dica

* Sempre declare as variáveis antes de usar `leia`
* Certifique-se de que o tipo da variável é compatível com o valor digitado
* A leitura acontece **na ordem em que os comandos aparecem**

---

### ✅ Resumo

✔️ `leia` captura dados do usuário

✔️ Armazena valores em variáveis

✔️ É essencial para entrada de dados em programas

👉 Esse comando é fundamental para criar programas interativos.

---

## 🖥️ 3. Saída de Dados (`escreva` e `escreval`)

Os comandos de saída são utilizados para **exibir informações na tela**.

---

### 🔹 Diferença entre os comandos

| Comando    | Comportamento                         |
| ---------- | ------------------------------------- |
| `escreva`  | Exibe o conteúdo **na mesma linha**   |
| `escreval` | Exibe o conteúdo e **quebra a linha** |

---

### 💡 Exemplo

Exibir um resultado calculado:

```
inteiro resultado

resultado = 10 + 5

escreva("Resultado: ")
escreval(resultado)
```

✔️ `escreva` mantém o texto na mesma linha

✔️ `escreval` exibe o valor e pula para a próxima linha

---

### 🔎 Outro exemplo

```
escreval("Olá, mundo!")
escreval("Bem-vindo ao Portugol")
```

✔️ Cada mensagem será exibida em uma nova linha

---

### 🔎 Dica

* Use `escreva` quando quiser **continuar na mesma linha**
* Use `escreval` para **organizar a saída com quebras de linha**

---

### ✅ Resumo

✔️ Comandos responsáveis pela **saída de dados**

✔️ `escreva` → mesma linha

✔️ `escreval` → nova linha

👉 Essenciais para mostrar resultados ao usuário.

---

## 4. Atribuição de Valores

A **atribuição** é o processo de **armazenar em uma variável** o resultado de uma expressão.

👉 É assim que os programas guardam resultados de cálculos para uso posterior.

---

### 📌 Exemplo: Calcular um desconto

#### 🧾 Comando

```
valor_final = valor_compra - desconto
```

---

### 🧠 Explicação

* **`valor_compra`** → valor original da compra
* **`desconto`** → valor que será subtraído
* **`valor_final`** → resultado após aplicar o desconto

---

### 💡 Como funciona

A variável **`valor_final`** recebe o resultado da expressão:

```
valor_compra - desconto
```

✔️ Primeiro, o sistema realiza o cálculo

✔️ Depois, armazena o resultado na variável

---

### 🔎 Outro exemplo

```
soma = 10 + 5
media = soma / 2
```

✔️ `soma` recebe 15

✔️ `media` recebe 7.5

---

### 🔎 Dica

* O símbolo `=` não significa “igual” como na matemática
* Ele significa **"recebe"**

👉 Exemplo:

```
x = 5
```

✔️ Leia como: **x recebe 5**

---

### ✅ Resumo

✔️ Atribuição guarda resultados em variáveis

✔️ Sempre ocorre após um cálculo ou valor direto

✔️ É essencial para construir a lógica do programa

👉 Sem atribuição, não há como manipular dados em um programa.

---

## 5. Operadores Aritméticos

Os **operadores aritméticos** são utilizados para realizar **cálculos numéricos** em programação.

---

### 🔢 Principais operadores

| Operador | Descrição        |
| -------- | ---------------- |
| `+`      | Soma             |
| `-`      | Subtração        |
| `*`      | Multiplicação    |
| `/`      | Divisão          |
| `%`      | Resto da divisão |

---

### 💡 Exemplo de uso

Calcular o **preço total** e verificar o **resto da divisão**:

```
preco_unitario = 10
quantidade = 3

total = preco_unitario * quantidade
resto = total % 2
```

---

### 📌 Explicação

* `total` → calcula o valor final da compra
* `resto` → retorna o valor que sobra na divisão por 2

---

### ⚙️ Exemplos de comandos

```
total = quantidade * preco
resto = numero % 4
```

✔️ Multiplicação para cálculo de valores

✔️ Operador `%` para verificar divisibilidade

---

### 🔎 Dica

* Use `%` quando precisar saber se um número é **par, múltiplo ou divisível**
* Combine operadores para resolver problemas mais complexos

---

### ✅ Resumo

✔️ Operadores aritméticos realizam cálculos

✔️ São base para qualquer lógica numérica

✔️ Podem ser combinados em expressões

👉 Essenciais para trabalhar com números em programação.

---

## 6. Operadores Relacionais

Os **operadores relacionais** são utilizados para **comparar valores** e retornar um resultado lógico (*verdadeiro* ou *falso*).

---

### 🔹 Principais operadores

| Operador | Descrição        |
| -------- | ---------------- |
| `==`     | Igual            |
| `!=`     | Diferente        |
| `>`      | Maior que        |
| `<`      | Menor que        |
| `>=`     | Maior ou igual a |
| `<=`     | Menor ou igual a |

---

### 💡 Exemplo prático

Verificar se uma **idade** está dentro de uma faixa específica (entre 3 e 12 anos):

```
idade >= 3
idade <= 12
```

✔️ A idade precisa atender **as duas condições**

✔️ Normalmente, usamos isso junto com operadores lógicos (`e`)

---

### 🔎 Dica

* Operadores relacionais são usados dentro de estruturas como `se`
* Sempre resultam em **verdadeiro ou falso**

---

### ✅ Resumo

✔️ Servem para comparar valores

✔️ Retornam resultados lógicos

✔️ São base para decisões em programas

👉 Essenciais para controle de fluxo (condições).

---

## 7. Operadores Lógicos

Os **operadores lógicos** permitem **combinar múltiplas condições**, retornando um resultado lógico (*verdadeiro* ou *falso*).

---

### 🔹 Principais operadores

| Operador | Descrição                                                     |
| -------- | ------------------------------------------------------------- |
| `e`      | Verdadeiro apenas se **todas** as condições forem verdadeiras |
| `ou`     | Verdadeiro se **pelo menos uma** das condições for verdadeira |
| `nao`    | **Inverte** o valor lógico da condição (verdadeiro ↔ falso)   |

---

### 💡 Exemplo prático

Verificar se um valor está dentro de um intervalo (entre 100 e 500):

```
valor >= 100 e valor <= 500
```

✔️ O valor deve satisfazer **as duas condições simultaneamente**

✔️ Caso uma delas seja falsa, o resultado será falso

---

### 🔎 Dica

* Use `e` quando **todas** as condições precisam ser verdadeiras
* Use `ou` quando **apenas uma** já é suficiente
* Use `nao` para inverter resultados

---

### ✅ Resumo

✔️ Operadores lógicos combinam condições

✔️ Retornam verdadeiro ou falso

✔️ São essenciais para decisões mais complexas

👉 Muito usados junto com estruturas `se`.

---

## 8. Estrutura Condicional: `se`, `senao se`, `senao`

A **estrutura condicional** é utilizada quando o programa precisa **tomar decisões com base em condições**.

Ela permite executar diferentes blocos de código dependendo do resultado de uma ou mais condições.

---

### 🔹 Estrutura básica

```
se (condicao) {
   // executa se a condição for verdadeira
}
senao se (outra_condicao) {
   // executa se a condição anterior for falsa
   // e esta for verdadeira
}
senao {
   // executa se nenhuma das condições anteriores for verdadeira
}
```

---

### 💡 Exemplo prático

Classificar uma pessoa de acordo com a idade:

```
se (idade <= 2) {
   escreval("Gratuita")
}
senao se (idade <= 12) {
   escreval("Meia tarifa")
}
senao {
   escreval("Tarifa completa")
}
```

✔️ O programa avalia as condições **de cima para baixo**.

✔️ Assim que encontra uma condição verdadeira, executa o bloco correspondente e **ignora os demais**.

---

## 9. Condições Aninhadas

As **condições aninhadas** ocorrem quando uma estrutura condicional está **dentro de outra**.

👉 São utilizadas quando um problema exige **múltiplas verificações encadeadas** dentro da lógica de decisão.

---

### 🔹 Quando usar?

Use condições aninhadas quando:

* Uma verificação depende do resultado de outra
* É necessário validar uma condição antes de avaliar a próxima
* O problema possui **níveis de decisão**

---

### 💡 Exemplo prático

Verificar primeiro se os valores formam um triângulo e, em seguida, identificar o tipo:

```
se (a < b + c e b < a + c e c < a + b) {
   se (a == b e b == c) {
      escreval("Equilátero")
   }
}
```

✔️ Primeiro, verifica se os lados formam um triângulo

✔️ Só depois executa a próxima verificação

✔️ Neste caso, identifica se é **equilátero**

---

### 🔎 Observação

Esse exemplo mostra apenas um dos tipos de triângulo.
Outras condições podem ser adicionadas para identificar:

* **Isósceles** → dois lados iguais
* **Escaleno** → todos os lados diferentes

---

### 🔎 Dica

* Evite muitos níveis de aninhamento para não dificultar a leitura
* Sempre valide primeiro a condição mais importante

---

### ✅ Resumo

✔️ Condições dentro de condições

✔️ Usadas para decisões em etapas

✔️ Melhoram a organização da lógica

👉 Muito comuns em problemas com validações sequenciais.

---

## 10. Teste de Divisibilidade com Operador `%`

O operador `%` (módulo) retorna o **resto da divisão inteira** entre dois números.

👉 Quando o resto é **igual a zero**, significa que um número é **divisível** por outro.

---

### 🔹 Como funciona?

| Expressão | Resultado | Explicação           |
| --------- | --------- | -------------------- |
| `10 % 2`  | `0`       | 10 é divisível por 2 |
| `10 % 3`  | `1`       | sobra 1 na divisão   |
| `15 % 5`  | `0`       | 15 é divisível por 5 |

---

### 💡 Exemplo prático

Verificar se um ano é divisível por 4:

```
ano % 4 == 0
```

✔️ Se a condição for verdadeira → **é divisível**

✔️ Se for falsa → **não é divisível**

---

### 🔎 Dica

Esse tipo de verificação é muito usado para:

* Identificar números pares → `numero % 2 == 0`
* Verificar anos bissextos
* Testar múltiplos de um número

---

### ✅ Resumo

✔️ `%` retorna o resto da divisão

✔️ Resto zero indica divisibilidade

✔️ Muito útil em validações numéricas

👉 Essencial para vários tipos de problemas lógicos.

---

## 11. Cálculo de Porcentagem

A **porcentagem** representa uma **parte de um valor total**.

👉 O cálculo é feito multiplicando o valor base pela taxa percentual e dividindo por 100.

---

### 🔹 Fórmula geral

```
porcentagem = valor * taxa / 100
```

---

### 💡 Exemplo prático

Calcular **10% de desconto** sobre um valor:

```
desconto = valor * 10 / 100
```

✔️ O resultado corresponde ao valor do desconto

Para obter o valor final com desconto:

```
valor_final = valor - desconto
```

✔️ Subtraímos o desconto do valor original

---

### 🔎 Dica

Esse tipo de cálculo é muito comum em:

* Descontos em compras
* Juros e taxas
* Comissões
* Cálculo de impostos

---

### ✅ Resumo

✔️ Porcentagem = parte de um todo

✔️ Sempre dividir por 100

✔️ Muito usada em cálculos financeiros

👉 Essencial para resolver diversos problemas do dia a dia.

---


## 12. Comparação entre Valores

Alguns exercícios exigem identificar o **maior valor**, o **menor valor** ou simplesmente **comparar quantidades** para tomar uma decisão.

👉 Esse tipo de lógica é muito comum em programação.

---

### 🔹 Objetivo

* Comparar dois ou mais valores
* Definir um resultado com base na comparação
* Armazenar ou exibir o valor desejado

---

### 💡 Exemplo prático

Verificar qual número é maior:

```
se (a > b) {
   maior = a
}
senao {
   maior = b
}
```

✔️ Se `a` for maior que `b`, então `maior` recebe `a`

✔️ Caso contrário, `maior` recebe `b`

---

### 🔎 Explicação

* O operador `>` compara os valores
* A estrutura `se` decide qual valor será escolhido
* O resultado é armazenado na variável `maior`

---

### 🔎 Dica

* Para comparar mais valores, repita o processo ou use variáveis auxiliares
* Essa lógica pode ser expandida para encontrar:

  * Maior entre vários números
  * Menor valor
  * Valores iguais

---

### ✅ Resumo

✔️ Comparações ajudam na tomada de decisão

✔️ Usam operadores relacionais (`>`, `<`, `==`, etc.)

✔️ Muito usadas com estruturas condicionais

👉 Fundamental para resolver problemas com múltiplos valores.

---

## 13. Faixas de Valores

Quando um problema envolve **intervalos**, a lógica deve considerar um **limite inferior** e um **limite superior**.

👉 Isso permite verificar se um valor está **dentro de uma faixa específica**.

---

### 🔹 Estrutura geral

```
valor >= limite_inferior e valor <= limite_superior
```

✔️ O valor precisa atender **as duas condições ao mesmo tempo**

---

### 💡 Exemplo prático

Verificar se o valor de uma compra está entre **R$100 e R$500**:

```
valor >= 100 e valor <= 500
```

✔️ Verdadeiro → está dentro da faixa

✔️ Falso → está fora do intervalo

---

### 🔎 Dica

Esse tipo de verificação é muito comum em:

* Faixas de preço
* Classificação por idade
* Validação de dados
* Regras com limites mínimos e máximos

---

### ✅ Resumo

✔️ Trabalha com limites inferior e superior

✔️ Usa operadores relacionais + lógicos

✔️ Muito usado em validações

👉 Essencial para problemas com intervalos.

---

## 14. Uso da Raiz Quadrada

A **raiz quadrada** é utilizada, por exemplo, para verificar se um número é um **quadrado perfeito**.

👉 Um número é considerado quadrado perfeito quando sua raiz quadrada é um **número inteiro**.

No **Portugol Studio**, esse cálculo é feito utilizando a **biblioteca matemática**.

---

### 🔹 Como utilizar

Antes de usar a função de raiz, é necessário incluir a biblioteca:

```
inclua biblioteca Matematica
```

---

### 🔹 Cálculo da raiz quadrada

```
raiz = Matematica.raiz(numero, 2)
```

✔️ `numero` → valor que será calculado

✔️ `2` → indica raiz quadrada

---

### 💡 Exemplo prático

Calcular a raiz quadrada de um número:

```
inclua biblioteca Matematica

raiz = Matematica.raiz(numero, 2)
```

---

### 🔎 Dica

Para verificar se um número é **quadrado perfeito**, você pode:

1. Calcular a raiz quadrada
2. Verificar se o resultado é inteiro

```
se (raiz == inteiro(raiz)) {
   escreval("É quadrado perfeito")
}
```

✔️ Se a raiz for inteira → quadrado perfeito

✔️ Caso contrário → não é

---

### ✅ Resumo

✔️ Usa biblioteca matemática

✔️ Calcula raiz com `Matematica.raiz`

✔️ Permite validar quadrados perfeitos

👉 Importante para problemas matemáticos.

---
## 15. Conversão entre Tipos de Informação Lida e Regra Lógica

Em muitos exercícios, o valor digitado pelo usuário não deve apenas ser exibido, mas sim **interpretado** para atender à lógica do problema.

👉 Isso significa que a entrada precisa ser **convertida ou utilizada em decisões** dentro do programa.

---

### 🔹 Ideia principal

* O programa **lê um valor**
* Esse valor é **analisado**
* A partir dele, uma **ação ou classificação** é definida

---

### 💡 Exemplo prático

Ler uma classificação indicativa e transformá-la em uma categoria:

```
leia(classificacao)
```

Depois da leitura, o valor pode ser usado em uma estrutura condicional:

```
se (classificacao == "L") {
   escreval("Livre para todos os públicos")
}
senao se (classificacao == "10") {
   escreval("Não recomendado para menores de 10 anos")
}
senao {
   escreval("Classificação desconhecida")
}
```

---

### 🔎 Dica

Esse tipo de lógica é muito comum quando:

* Transformamos **dados de entrada em decisões**
* Trabalhamos com **menus ou categorias**
* Validamos informações digitadas pelo usuário

✔️ Lembre-se: **ler um valor é só o começo — o programa precisa saber o que fazer com ele.**

---

### ✅ Resumo

✔️ Entrada de dados precisa ser interpretada

✔️ Use estruturas condicionais para decidir ações

✔️ Converta informação em lógica útil

👉 Essencial para transformar dados em comportamento no programa.

---

## 🧠 Exercício 1 — Ano Bissexto

### 📌 Enunciado

Ler um **ano** e verificar se ele é **bissexto**.

👉 Um ano é bissexto quando:

* É divisível por **4**, **mas não** por **100**,
* **Ou** é divisível por **400**.

O programa deve exibir o ano informado e indicar se ele é ou não bissexto.

---

### 🔍 Como interpretar logicamente

Este problema envolve uma **regra de divisibilidade com exceção**:

* Apenas verificar `ano % 4 == 0` **não é suficiente**
* Anos divisíveis por **100** não são bissextos...
* **Exceto** quando também são divisíveis por **400**

✔️ Ou seja, temos uma lógica combinada com **"e"** e **"ou"**

---

### ⚙️ O que o programa precisa fazer

* Ler um ano
* Aplicar a regra de ano bissexto
* Informar o ano lido
* Exibir se ele é ou não bissexto

---

### 📥 Entradas

* Ano (número inteiro)

---

### 🔄 Processamento

Verificar se:

```
(ano % 4 == 0 e ano % 100 != 0) ou (ano % 400 == 0)
```

✔️ Se essa condição for verdadeira → **ano bissexto**

✔️ Caso contrário → **não bissexto**

---

### 📤 Saídas

* Ano informado
* Mensagem indicando se é bissexto ou não

---

### 🧩 Raciocínio passo a passo

1. Declarar uma variável para armazenar o ano
2. Ler o valor digitado
3. Verificar se é divisível por 4 **e não por 100**
4. Verificar a exceção: divisível por 400
5. Combinar as condições com operador lógico
6. Exibir o resultado final

---

### 💡 Exemplo de implementação

```
inteiro ano

leia(ano)

se ((ano % 4 == 0 e ano % 100 != 0) ou (ano % 400 == 0)) {
   escreval(ano, " é bissexto")
}
senao {
   escreval(ano, " não é bissexto")
}
```

---

### ✅ Resumo

✔️ Use `%` para verificar divisibilidade

✔️ Combine condições com `e` e `ou`

✔️ Atenção à **regra especial dos múltiplos de 100 e 400**

👉 Esse é um dos exercícios clássicos para treinar **lógica condicional composta**.

---

## 🧠 Exercício 2 — Classificação de Triângulo

### 📌 Enunciado

Ler **três números** e verificar se eles formam um **triângulo**.
Caso formem, identificar se é:

* **Equilátero** (todos os lados iguais)
* **Isósceles** (dois lados iguais)
* **Escaleno** (todos os lados diferentes)

---

### 🔍 Como interpretar logicamente

Antes de classificar, é necessário verificar se os valores **podem formar um triângulo**.

👉 Isso acontece quando:

```
a < b + c e b < a + c e c < a + b
```

✔️ Somente após essa verificação faz sentido classificar o triângulo.

---

### ⚙️ O que o programa precisa fazer

* Ler três valores
* Verificar se formam um triângulo
* Se sim, identificar o tipo
* Exibir o resultado

---

### 📥 Entradas

* Três números representando os lados (`a`, `b`, `c`)

---

### 🔄 Processamento

1. Verificar a condição de existência do triângulo
2. Se verdadeiro:

   * Verificar se `a == b e b == c` → **Equilátero**
   * Senão, verificar se dois lados são iguais → **Isósceles**
   * Caso contrário → **Escaleno**

---

### 📤 Saídas

* Mensagem informando se forma ou não triângulo
* Caso forme, o tipo do triângulo

---

### 🧩 Raciocínio passo a passo

1. Declarar três variáveis para os lados
2. Ler os valores digitados
3. Testar se cada lado é menor que a soma dos outros dois
4. Se não formar triângulo → exibir mensagem
5. Se formar:

   * Verificar se todos são iguais
   * Senão, verificar se dois são iguais
   * Caso contrário, todos são diferentes
6. Exibir o resultado final

---

### 💡 Exemplo de implementação

```
real a, b, c

leia(a, b, c)

se (a < b + c e b < a + c e c < a + b) {
   
   se (a == b e b == c) {
      escreval("Triângulo Equilátero")
   }
   senao se (a == b ou a == c ou b == c) {
      escreval("Triângulo Isósceles")
   }
   senao {
      escreval("Triângulo Escaleno")
   }

}
senao {
   escreval("Não forma triângulo")
}
```

---

### ✅ Resumo

✔️ Sempre verifique primeiro se **forma triângulo**

✔️ Use **condições aninhadas** para classificar

✔️ Combine operadores lógicos (`e`, `ou`) corretamente

👉 Esse exercício reforça:

* Validação de dados
* Condições encadeadas
* Classificação com base em regras

---

## 🧠 Exercício 3 — Cálculo de Desconto por Faixa

### 📌 Enunciado

Ler o **valor de uma compra** e calcular o **desconto** de acordo com as seguintes regras:

* Menor que **R$100** → **sem desconto**
* Entre **R$100 e R$500** → **10% de desconto**
* Acima de **R$500** → **20% de desconto**

Ao final, exibir o **valor após o desconto**.

---

### 🔍 Como interpretar logicamente

Este exercício trabalha com **faixas de valores**.

👉 Cada faixa determina um **percentual diferente de desconto**
👉 Após identificar a faixa, o programa deve:

1. Calcular o desconto
2. Subtrair do valor original

---

### ⚙️ O que o programa precisa fazer

* Ler o valor da compra
* Identificar a faixa correspondente
* Calcular o desconto
* Calcular o valor final
* Exibir o resultado

---

### 📥 Entradas

* Valor da compra (número real)

---

### 🔄 Processamento

1. Comparar o valor com os limites:

   * `< 100` → desconto = 0
   * `>= 100 e <= 500` → desconto = 10%
   * `> 500` → desconto = 20%

2. Calcular o desconto:

```
desconto = valor * percentual / 100
```

3. Calcular o valor final:

```
valor_final = valor - desconto
```

---

### 📤 Saídas

* Valor original da compra
* Valor final com desconto aplicado

---

### 🧩 Raciocínio passo a passo

1. Declarar variáveis:

   * `valor`
   * `desconto`
   * `valor_final`

2. Ler o valor da compra

3. Verificar a faixa de valor:

   * Se menor que 100 → desconto = 0
   * Senão, se até 500 → 10%
   * Senão → 20%

4. Calcular o desconto

5. Calcular o valor final

6. Exibir os resultados

---

### 💡 Exemplo de implementação

```
real valor, desconto, valor_final

leia(valor)

se (valor < 100) {
   desconto = 0
}
senao se (valor <= 500) {
   desconto = valor * 10 / 100
}
senao {
   desconto = valor * 20 / 100
}

valor_final = valor - desconto

escreval("Valor da compra: ", valor)
escreval("Valor final com desconto: ", valor_final)
```

---

### ✅ Resumo

✔️ Identifique corretamente a **faixa de valores**

✔️ Aplique o percentual adequado

✔️ Separe bem: cálculo do desconto e cálculo do valor final

👉 Esse exercício reforça:

* Estruturas condicionais (`se`, `senao se`, `senao`)
* Uso de porcentagem
* Lógica com intervalos

---

## 🧠 Exercício 4 — Cálculo de Estacionamento

### 📌 Enunciado

Ler o **tempo de permanência** de um veículo em um estacionamento e calcular o **valor a pagar**, considerando:

* Até **2 horas** → **R$ 2,00 por hora**
* Após 2 horas →

  * As 2 primeiras continuam custando R$ 2,00 cada
  * As horas adicionais custam **R$ 1,00 por hora**

---

### 🔍 Como interpretar logicamente

O problema possui **duas regras de cobrança**:

1. Para até 2 horas → cálculo direto
2. Para mais de 2 horas → cálculo dividido em duas partes:

   * Valor fixo das 2 primeiras horas
   * Valor das horas excedentes

---

### ⚙️ O que o programa precisa fazer

* Ler o tempo de permanência
* Verificar se ultrapassa 2 horas
* Calcular o valor total
* Exibir o resultado

---

### 📥 Entradas

* Tempo de permanência (em horas)

---

### 🔄 Processamento

* Se `tempo <= 2`:

```
preco = tempo * 2
```

* Se `tempo > 2`:

```
preco = (2 * 2) + ((tempo - 2) * 1)
```

✔️ `2 * 2` → valor fixo das primeiras 2 horas

✔️ `(tempo - 2)` → horas excedentes

---

### 📤 Saídas

* Tempo de permanência
* Valor total a pagar

---

### 🧩 Raciocínio passo a passo

1. Declarar variáveis:

   * `tempo`
   * `preco`

2. Ler o tempo informado

3. Verificar:

   * Se até 2 horas → cálculo direto
   * Senão:

     * Calcular valor das 2 primeiras horas
     * Calcular horas excedentes
     * Somar os valores

4. Exibir o resultado final

---

### 💡 Exemplo de implementação

```
real tempo, preco

leia(tempo)

se (tempo <= 2) {
   preco = tempo * 2
}
senao {
   preco = (2 * 2) + ((tempo - 2) * 1)
}

escreval("Tempo: ", tempo, " horas")
escreval("Valor a pagar: R$ ", preco)
```

---

### ✅ Resumo

✔️ Problema com **faixa + parte fixa + excedente**

✔️ Separe o cálculo em partes para facilitar

✔️ Use estrutura condicional para decidir a regra

👉 Esse exercício reforça:

* Lógica com **limites e excedentes**
* Organização de cálculos
* Estruturas condicionais

---

## 🧠 Exercício 5 — Etanol ou Gasolina?

### 📌 Enunciado

Ler o **preço do etanol** e da **gasolina** e indicar qual combustível é mais vantajoso.

👉 Regra:

* Se o etanol custar até **70% do preço da gasolina** → usar **etanol**
* Caso contrário → usar **gasolina**

---

### 🔍 Como interpretar logicamente

A decisão não depende apenas de qual combustível é mais barato.

👉 É necessário comparar o preço do etanol com **70% do valor da gasolina**.

✔️ Essa proporção é baseada no rendimento dos combustíveis.

---

### ⚙️ O que o programa precisa fazer

* Ler os preços do etanol e da gasolina
* Calcular 70% do preço da gasolina
* Comparar com o preço do etanol
* Exibir a recomendação

---

### 📥 Entradas

* Preço do etanol
* Preço da gasolina

---

### 🔄 Processamento

1. Calcular 70% da gasolina:

```
limite = gasolina * 70 / 100
```

2. Comparar:

```
etanol <= limite
```

✔️ Verdadeiro → usar etanol

✔️ Falso → usar gasolina

---

### 📤 Saídas

* Mensagem recomendando:

  * **Etanol** ou
  * **Gasolina**

---

### 🧩 Raciocínio passo a passo

1. Declarar variáveis:

   * `etanol`
   * `gasolina`
   * `limite`

2. Ler os preços

3. Calcular 70% da gasolina

4. Comparar com o preço do etanol

5. Exibir a recomendação

---

### 💡 Exemplo de implementação

```
real etanol, gasolina, limite

leia(etanol, gasolina)

limite = gasolina * 70 / 100

se (etanol <= limite) {
   escreval("Abastecer com Etanol")
}
senao {
   escreval("Abastecer com Gasolina")
}
```

---

### ✅ Resumo

✔️ Use **porcentagem** para definir o limite

✔️ Compare corretamente os valores

✔️ Baseie a decisão em uma **regra lógica específica**, não apenas no menor preço

👉 Esse exercício reforça:

* Cálculo de porcentagem
* Comparação entre valores
* Tomada de decisão baseada em regra

---

## 🧠 Exercício 6 — Classificação de Tarifa por Idade

### 📌 Enunciado

Ler a **idade do passageiro** e determinar o tipo de tarifa:

* Até **2 anos** → **Gratuita**
* De **3 a 12 anos** → **Meia tarifa**
* Acima de **12 anos** → **Tarifa completa**

O programa deve exibir o tipo de tarifa correspondente.

---

### 🔍 Como interpretar logicamente

O problema utiliza **faixas de valores (idade)**.

👉 Cada intervalo corresponde a uma **categoria de tarifa**.

✔️ Basta comparar a idade com os limites definidos.

---

### ⚙️ O que o programa precisa fazer

* Ler a idade do passageiro
* Verificar em qual faixa ele se encontra
* Definir a tarifa correspondente
* Exibir o resultado

---

### 📥 Entradas

* Idade do passageiro (número inteiro)

---

### 🔄 Processamento

Verificar as condições:

```
idade <= 2
```

```
idade <= 12
```

✔️ Se `idade <= 2` → Gratuita

✔️ Senão, se `idade <= 12` → Meia tarifa

✔️ Senão → Tarifa completa

---

### 📤 Saídas

* Tipo de tarifa a ser aplicada

---

### 🧩 Raciocínio passo a passo

1. Declarar variável `idade`
2. Ler o valor informado
3. Verificar:

   * Se idade ≤ 2 → gratuita
   * Senão, se idade ≤ 12 → meia tarifa
   * Senão → tarifa completa
4. Exibir o resultado

---

### 💡 Exemplo de implementação

```
inteiro idade

leia(idade)

se (idade <= 2) {
   escreval("Gratuita")
}
senao se (idade <= 12) {
   escreval("Meia tarifa")
}
senao {
   escreval("Tarifa completa")
}
```

---

### ✅ Resumo

✔️ Problema baseado em **faixas de idade**

✔️ Use `se`, `senao se` e `senao` para classificar

✔️ Ordem das condições é importante

👉 Esse exercício reforça:

* Estruturas condicionais
* Comparação com intervalos
* Classificação de dados

---

## 🧠 Exercício 7 — Verificar Vogal

### 📌 Enunciado

Ler um **caractere** e verificar se ele é uma **vogal**.
Exibir o caractere informado e indicar se é ou não uma vogal.

---

### 🔍 Como interpretar logicamente

O problema consiste em comparar o caractere com o conjunto das **vogais**:

👉 `a`, `e`, `i`, `o`, `u`

✔️ Se o caractere for igual a **qualquer uma dessas letras**, então é vogal.

---

### ⚙️ O que o programa precisa fazer

* Ler um caractere
* Comparar com as vogais
* Informar o resultado

---

### 📥 Entradas

* Um caractere

---

### 🔄 Processamento

Verificar se o caractere é igual a uma das vogais:

```
letra == 'a' ou letra == 'e' ou letra == 'i' ou letra == 'o' ou letra == 'u'
```

✔️ Verdadeiro → é vogal

✔️ Falso → não é vogal

---

### 📤 Saídas

* Caractere digitado
* Mensagem informando se é vogal ou não

---

### 🧩 Raciocínio passo a passo

1. Declarar variável do tipo caractere (`letra`)
2. Ler o valor digitado
3. Comparar com cada vogal usando `ou`
4. Se corresponder → é vogal
5. Caso contrário → não é vogal
6. Exibir o resultado

---

### 💡 Exemplo de implementação

```
caractere letra

leia(letra)

se (letra == 'a' ou letra == 'e' ou letra == 'i' ou letra == 'o' ou letra == 'u') {
   escreval(letra, " é uma vogal")
}
senao {
   escreval(letra, " não é uma vogal")
}
```

---

### 🔎 Dica

Se quiser melhorar o programa, você pode:

* Considerar **letras maiúsculas** (`A, E, I, O, U`)
* Converter o caractere para minúsculo antes da comparação

---

### ✅ Resumo

✔️ Use operador `ou` para múltiplas comparações

✔️ Compare com todas as vogais

✔️ Retorne a classificação correta

👉 Esse exercício reforça:

* Comparações com caracteres
* Uso de operadores lógicos
* Estruturas condicionais simples

---

## 🧠 Exercício 8 — Maior de Três Números

### 📌 Enunciado

Ler **três números inteiros** e exibir o **maior** entre eles.

---

### 🔍 Como interpretar logicamente

O objetivo é identificar qual valor é o **maior entre três**.

👉 Isso pode ser feito por **comparações sucessivas**
👉 Ou mantendo uma variável que armazena o maior valor atual

---

### ⚙️ O que o programa precisa fazer

* Ler três números
* Compará-los
* Identificar o maior
* Exibir o resultado

---

### 📥 Entradas

* Três números inteiros (`n1`, `n2`, `n3`)

---

### 🔄 Processamento

Estratégia mais comum:

1. Assumir que o primeiro número é o maior
2. Comparar com o segundo:

   * Se for maior, atualizar
3. Comparar com o terceiro:

   * Se for maior, atualizar novamente

---

### 📤 Saídas

* O maior número entre os três

---

### 🧩 Raciocínio passo a passo

1. Declarar variáveis:

   * `n1`, `n2`, `n3`
   * `maior`

2. Ler os três valores

3. Definir inicialmente:

   ```plaintext
   maior = n1
   ```

4. Comparar:

   * Se `n2 > maior` → atualizar
   * Se `n3 > maior` → atualizar

5. Exibir o valor final

---

### 💡 Exemplo de implementação

```
inteiro n1, n2, n3, maior

leia(n1, n2, n3)

maior = n1

se (n2 > maior) {
   maior = n2
}

se (n3 > maior) {
   maior = n3
}

escreval("Maior valor: ", maior)
```

---

### 🔎 Alternativa

Também é possível resolver usando uma única estrutura condicional com várias comparações, mas a abordagem com variável `maior` é:

✔️ Mais organizada
✔️ Mais fácil de entender
✔️ Escalável para mais valores

---

### ✅ Resumo

✔️ Use comparações sequenciais

✔️ Armazene o maior valor em uma variável

✔️ Atualize conforme necessário

👉 Esse exercício reforça:

* Comparações múltiplas
* Atualização de variáveis
* Lógica sequencial

---

## 🧠 Exercício 9 — Quadrado Perfeito

### 📌 Enunciado

Ler um **número** e verificar se ele é um **quadrado perfeito**.

👉 Um número é quadrado perfeito quando sua **raiz quadrada é um número inteiro**.

---

### 🔍 Como interpretar logicamente

A lógica do problema é:

* Calcular a **raiz quadrada** do número
* Verificar se o resultado **não possui parte decimal**

✔️ Se for inteiro → é quadrado perfeito

✔️ Caso contrário → não é

---

### ⚙️ O que o programa precisa fazer

* Ler um número
* Calcular sua raiz quadrada
* Verificar se a raiz é inteira
* Exibir o resultado

---

### 📥 Entradas

* Um número

---

### 🔄 Processamento

1. Calcular a raiz quadrada:

```
raiz = Matematica.raiz(numero, 2)
```

2. Verificar se é inteiro:

```
raiz == inteiro(raiz)
```

✔️ Verdadeiro → quadrado perfeito
✔️ Falso → não é

---

### 📤 Saídas

* Número informado
* Mensagem indicando se é quadrado perfeito

---

### 🧩 Raciocínio passo a passo

1. Declarar variáveis:

   * `numero`
   * `raiz`

2. Ler o número

3. Calcular a raiz quadrada

4. Verificar se a raiz é inteira

5. Exibir o resultado

---

### 💡 Exemplo de implementação

```
inclua biblioteca Matematica

real numero, raiz

leia(numero)

raiz = Matematica.raiz(numero, 2)

se (raiz == inteiro(raiz)) {
   escreval(numero, " é quadrado perfeito")
}
senao {
   escreval(numero, " não é quadrado perfeito")
}
```

---

### 🔎 Alternativa lógica

Outra forma de verificar:

```
inteiro r

r = inteiro(raiz)

se (r * r == num*
```

---

## 🧠 Exercício 10 — Classificação Indicativa de Filme

### 📌 Enunciado

Ler a **classificação indicativa** de um filme e identificar sua **categoria**, de acordo com as seguintes faixas:

- Até **10 anos** → **Infantil**
- De **11 a 14 anos** → **Infantojuvenil**
- De **15 a 17 anos** → **Juvenil**
- Acima de **17 anos** → **Adulto**

O programa deve exibir a categoria correspondente.

---

### 🔍 Como interpretar logicamente

Neste exercício, o programa precisa **transformar um valor numérico em uma categoria textual**.

👉 Cada faixa de idade corresponde a uma classificação específica.  
👉 Portanto, basta comparar o valor informado com os limites de cada faixa.

---

### ⚙️ O que o programa precisa fazer

- Ler a classificação indicativa
- Verificar em qual faixa ela se encontra
- Associar a categoria correta
- Exibir o resultado

---

### 📥 Entrada

- Classificação indicativa do filme

---

### 🔄 Processamento

Comparar o valor lido com os limites definidos:

- Se `classificacao <= 10` → **Infantil**
- Senão, se `classificacao <= 14` → **Infantojuvenil**
- Senão, se `classificacao <= 17` → **Juvenil**
- Senão → **Adulto**

---

### 📤 Saída

- Categoria do filme

---

### 🧩 Raciocínio passo a passo

1. Declarar uma variável para a classificação indicativa
2. Ler o valor informado
3. Verificar se a classificação é menor ou igual a 10
4. Caso contrário, verificar se é menor ou igual a 14
5. Depois, verificar se é menor ou igual a 17
6. Se não se encaixar em nenhuma faixa anterior, classificar como adulto
7. Exibir a categoria correspondente

---

### 💡 Exemplo de implementação

```
inteiro classificacao

leia(classificacao)

se (classificacao <= 10) {
   escreval("Infantil")
}
senao se (classificacao <= 14) {
   escreval("Infantojuvenil")
}
senao se (classificacao <= 17) {
   escreval("Juvenil")
}
senao {
   escreval("Adulto")
}
```

✅ Resumo

✔️ O exercício trabalha com faixas de valores

✔️ Cada intervalo gera uma categoria diferente

✔️ A estrutura se, senao se e senao é a mais adequada para esse tipo de classificação

👉 Esse exercício reforça:

- Comparações com intervalos
- Classificação por faixas
- Estruturas condicionais encadeadas


---

**Metadata & Attribution**

* **Date:** March 2026

* **Character:** Zahy — Zahroniel Syrran *(from the Zaion Universe)*

* **Character GitHub:** [Zahroniel Syrran](https://github.com/zahroniel-syrran)

* **Author:** Human — Ronildo A. Ferreira

* **Author GitHub:** [Ronildo A Ferreira](https://github.com/ronildo-ferreira)


* **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)







