# Princípios de Programação de Computadores

## 1. Introdução

A programação de computadores é a atividade de criar instruções que um computador pode executar para resolver problemas. Essas instruções são escritas em linguagens de programação e organizadas em estruturas chamadas **algoritmos**.

Compreender os princípios básicos da programação é importante porque permite desenvolver soluções para diversos tipos de problemas, desde tarefas simples até sistemas complexos utilizados em empresas, aplicações web e dispositivos móveis.

Antes mesmo de aprender uma linguagem específica, é essencial entender conceitos fundamentais como **resolução de problemas**, **lógica de programação**, **algoritmos** e o funcionamento das ferramentas utilizadas no desenvolvimento de software.

Nesta atividade, você irá conhecer esses conceitos e investigar algumas ferramentas utilizadas por programadores, incluindo o **Portugol Studio**, um ambiente utilizado para aprender lógica de programação.

---

## 2. Conceitos fundamentais

### Resolução de problemas

Resolver problemas é uma habilidade fundamental na programação. Antes de escrever qualquer código, o programador precisa compreender claramente o problema, identificar os dados envolvidos e definir os passos necessários para chegar a uma solução.

Normalmente esse processo envolve:

- entender o problema
- dividir o problema em partes menores
- definir uma sequência lógica de passos
- testar e ajustar a solução

**Exemplo simples:**  
Problema: calcular a média de duas notas de um aluno.

Passos possíveis:

1. receber as duas notas
2. somar as notas
3. dividir o resultado por 2
4. mostrar a média

---

### Lógica de programação e algoritmos

A **lógica de programação** é a forma de organizar o raciocínio para resolver problemas utilizando uma sequência lógica de passos.

Um **algoritmo** é a descrição passo a passo de como resolver um problema.

Algoritmos podem ser escritos de diferentes formas:

- linguagem natural
- fluxogramas
- pseudocódigo (como Portugol)

**Exemplo de algoritmo simples:**

```
ler numero1
ler numero2
media = (numero1 + numero2) / 2
mostrar media
```

---

### Código-fonte, código objeto e executável

Quando um programador escreve um programa, ele cria um **código-fonte**.

O código-fonte é um arquivo contendo instruções escritas em uma linguagem de programação.

Esse código precisa ser convertido para uma forma que o computador consiga executar.

Esse processo gera:

- **Código objeto** – versão intermediária do programa após compilação.
- **Executável** – programa final que pode ser executado pelo sistema operacional.

Fluxo simplificado:

```
Código-fonte → compilação → código objeto → executável
```

---

### Compiladores e interpretadores

Para que um programa funcione, o código precisa ser traduzido para linguagem de máquina.

Isso pode ocorrer de duas formas principais.

**Compilador**

Um compilador traduz todo o programa antes de executá-lo, gerando um arquivo executável.

Exemplos de linguagens compiladas:

- C
- C++
- Go
- Rust

**Interpretador**

Um interpretador executa o código linha por linha, traduzindo as instruções enquanto o programa roda.

Exemplos de linguagens interpretadas:

- Python
- JavaScript
- Ruby

Cada abordagem possui vantagens e desvantagens relacionadas a desempenho, facilidade de desenvolvimento e portabilidade.

---

### Kits de desenvolvimento (SDK), IDEs, bibliotecas e frameworks

Durante o desenvolvimento de software, os programadores utilizam diferentes ferramentas.

**SDK (Software Development Kit)**  
Conjunto de ferramentas para desenvolver aplicações para uma determinada plataforma.

Exemplo: Android SDK.

**IDE (Ambiente de Desenvolvimento Integrado)**  
Software que reúne várias ferramentas em um único ambiente para facilitar o desenvolvimento.

Normalmente inclui:

- editor de código
- compilador ou interpretador
- depurador
- ferramentas de execução

Exemplos:

- Visual Studio Code
- IntelliJ IDEA
- Eclipse

**Bibliotecas**

Conjunto de códigos prontos que podem ser reutilizados em programas.

Exemplo: bibliotecas para manipulação de imagens ou cálculos matemáticos.

**Frameworks**

Estruturas de desenvolvimento que organizam a forma de construir aplicações, fornecendo padrões e ferramentas prontas.

Exemplo:

- React
- Spring
- Django

---

### Portugol Studio

O **Portugol Studio** é um ambiente de desenvolvimento voltado ao ensino de lógica de programação.

Ele utiliza uma linguagem simplificada semelhante ao português, chamada **Portugol**, que facilita o aprendizado dos conceitos básicos de algoritmos.

Principais características:

- linguagem simples
- interface visual amigável
- execução passo a passo
- destaque de erros

Exemplo de programa simples em Portugol:

```
programa
{
    funcao inicio()
    {
        inteiro numero

        escreva("Digite um número: ")
        leia(numero)

        escreva("Você digitou: ", numero)
    }
}
```

Esse tipo de ferramenta permite focar no **raciocínio lógico**, antes de aprender linguagens mais complexas.

---
# Explicação linha a linha — Exemplo em Portugol Studio

## Código analisado

```portugol
programa
{
    funcao inicio()
    {
        inteiro numero

        escreva("Digite um número: ")
        leia(numero)

        escreva("Você digitou: ", numero)
    }
}
```

---

# Explicação detalhada do código

A seguir está a explicação de **cada linha do programa**, mostrando o que ela faz e por que é necessária.

---

## Linha 1

```portugol
programa
```

Esta palavra indica o **início da definição de um programa** no Portugol Studio.

Ela informa ao ambiente que o código a seguir representa um programa completo que poderá ser executado.

Em muitas linguagens de programação existe uma estrutura semelhante que define o início do programa.

---

## Linha 2

```portugol
{
```

A chave `{` inicia um **bloco de código**.

Blocos de código agrupam instruções que pertencem a uma mesma estrutura.

Neste caso, o bloco delimita **todo o conteúdo do programa**.

---

## Linha 3

```portugol
funcao inicio()
```

Esta linha define uma **função chamada `inicio`**.

No Portugol Studio, a função `inicio()` é o **ponto de entrada do programa**, ou seja, é onde a execução começa.

Quando o programa é executado, o computador inicia a execução a partir desta função.

Os parênteses `()` indicam que a função **não recebe parâmetros**.

---

## Linha 4

```portugol
{
```

Esta chave abre o bloco de código da função `inicio`.

Tudo que estiver dentro desse bloco será executado quando o programa iniciar.

---

## Linha 5

```portugol
inteiro numero
```

Aqui é feita a **declaração de uma variável**.

Elementos da linha:

- `inteiro` → tipo de dado (número inteiro)
- `numero` → nome da variável

A variável será usada para **armazenar o número digitado pelo usuário**.

Exemplo de valores que poderiam ser armazenados:

```
5
10
-3
42
```

---

## Linha 6

```portugol

```

Linha em branco.

Não possui efeito no funcionamento do programa.

Serve apenas para **melhorar a organização e a leitura do código**.

Boa organização do código facilita a manutenção e compreensão do programa.

---

## Linha 7

```portugol
escreva("Digite um número: ")
```

O comando `escreva` é usado para **mostrar uma mensagem na tela**.

Neste caso, o programa exibirá:

```
Digite um número:
```

Isso serve para **orientar o usuário** sobre o que ele deve fazer em seguida.

A mensagem está entre **aspas**, pois é um texto.

---

## Linha 8

```portugol
leia(numero)
```

O comando `leia` é utilizado para **receber dados digitados pelo usuário**.

Funcionamento:

1. o programa espera o usuário digitar algo
2. o valor digitado é armazenado na variável `numero`

Exemplo de execução:

Usuário digita:

```
8
```

Então o valor **8 será armazenado na variável `numero`**.

---

## Linha 9

```portugol

```

Outra linha em branco utilizada apenas para **organização visual do código**.

---

## Linha 10

```portugol
escreva("Você digitou: ", numero)
```

Esta linha mostra uma mensagem combinando **texto e o valor da variável**.

O programa exibirá algo como:

```
Você digitou: 8
```

Partes da instrução:

- `"Você digitou: "` → texto fixo
- `numero` → valor armazenado na variável

A vírgula separa os elementos que serão mostrados na tela.

---

## Linha 11

```portugol
}
```

Esta chave fecha o **bloco da função `inicio`**.

Isso indica que **todas as instruções da função terminaram**.

---

## Linha 12

```portugol
}
```

Esta chave fecha o **bloco do programa**.

Com isso, o programa está completo.

---

# Fluxo de execução do programa

O comportamento do programa pode ser resumido em três etapas:

## 1. Exibir mensagem

```
Digite um número:
```

---

## 2. Ler entrada do usuário

Usuário digita um número.

Exemplo:

```
15
```

---

## 3. Mostrar resultado

O programa exibe:

```
Você digitou: 15
```

---

# Estrutura geral do programa

Podemos representar a lógica do programa assim:

```
Mostrar mensagem → Ler número → Mostrar número digitado
```

Ou em forma de fluxo:

```
Saída (mensagem)
       ↓
Entrada (usuário digita número)
       ↓
Saída (mostrar número digitado)
```

---

# Conceitos importantes presentes no exemplo

Este pequeno programa demonstra vários conceitos básicos de programação:

- estrutura de um programa
- função principal (`inicio`)
- declaração de variáveis
- entrada de dados (`leia`)
- saída de dados (`escreva`)
- uso de blocos `{ }`

Esses conceitos aparecem em praticamente **todas as linguagens de programação**.

---

# Experimento sugerido

Para compreender melhor o funcionamento do programa:

1. Abra o **Portugol Studio**.
2. Copie o código apresentado.
3. Execute o programa.
4. Digite diferentes números.
5. Observe o resultado mostrado na tela.

Depois tente modificar o programa para:

- mostrar o número **multiplicado por 2**
- mostrar o número **somado com 10**

Essa experimentação ajuda a desenvolver **lógica de programação e compreensão do código**.
---

## 3. Exemplos práticos

### Exemplo 1 — Algoritmo do cotidiano

Problema: preparar um café.

Algoritmo possível:

1. colocar água no recipiente
2. colocar café no filtro
3. aquecer a água
4. passar a água pelo café
5. servir a bebida

Esse exemplo mostra que **algoritmos não existem apenas em programação**, mas em muitas atividades do dia a dia.

---

### Exemplo 2 — Algoritmo simples em Portugol

Programa que calcula a soma de dois números.

```
programa
{
    funcao inicio()
    {
        inteiro a
        inteiro b
        inteiro soma

        escreva("Digite o primeiro número: ")
        leia(a)

        escreva("Digite o segundo número: ")
        leia(b)

        soma = a + b

        escreva("Resultado: ", soma)
    }
}
```

Esse exemplo demonstra:

- entrada de dados
- processamento
- saída de resultados

---

### Exemplo 3 — Fluxo simplificado de um programa

```
Entrada de dados
       ↓
Processamento
       ↓
Resultado
```

Esse modelo aparece em praticamente todos os programas de computador.

---

## 4. Exercícios

### Exercício 1 — Pergunta conceitual

Explique com suas próprias palavras:

- o que é um **algoritmo**
- qual é a relação entre **lógica de programação** e **algoritmos**

Apresente também **um exemplo simples de algoritmo do cotidiano**.

---

### Exercício 2 — Pergunta de aplicação

Considere o seguinte problema:

Um programa deve receber três números e mostrar qual deles é o maior.

1. Descreva um **algoritmo em linguagem natural** para resolver esse problema.
2. Se possível, represente esse algoritmo em **pseudocódigo ou Portugol**.

---

### Exercício 3 — Pergunta de investigação

Realize uma pequena investigação sobre o **Portugol Studio**.

Tarefas sugeridas:

1. Pesquise o que é o Portugol Studio e para que ele é utilizado.
2. Instale o programa ou utilize uma versão disponível online.
3. Crie um pequeno programa que:
   - leia um número
   - mostre o número multiplicado por 2
4. Inclua no trabalho:
   - um trecho do código criado
   - uma captura de tela da execução (se possível)

Explique brevemente sua experiência utilizando a ferramenta.

---

### Exercício 4 — Pergunta de reflexão

Ferramentas como IDEs, bibliotecas e frameworks ajudam os programadores a desenvolver sistemas mais rapidamente.

Reflita e responda:

- Por que essas ferramentas são importantes no desenvolvimento de software?
- Quais problemas poderiam surgir se os programadores precisassem desenvolver **todos os componentes do zero**?

Justifique sua resposta com exemplos.

---

## 5. Instruções para os alunos

Esta atividade deve ser realizada **em grupo**.

O objetivo é discutir os conceitos apresentados, pesquisar informações adicionais e produzir respostas claras e bem explicadas.

### Modalidade da atividade

Trabalho em grupo.

### Local de entrega

Repositório GitHub do grupo.

### Formato do arquivo

Arquivo em **Markdown**.

### Nome do arquivo

```
1B-M1-Questionario.md
```

### Organização das respostas

As respostas devem:

- ser claras e bem organizadas
- demonstrar compreensão dos conceitos estudados
- apresentar explicações próprias
- evitar apenas copiar definições da internet

#### Regras para atividades em grupo

- cada integrante deve contribuir de forma colaborativa
- quando houver diferentes exercícios, indicar qual aluno foi responsável por cada parte
- o trabalho final deve demonstrar organização e participação de todos

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

## 6. Critérios de avaliação

Serão considerados os seguintes critérios:

- clareza e organização das respostas
- qualidade da pesquisa realizada
- aplicação correta dos conceitos estudados
- capacidade de explicação e argumentação
- organização do documento entregue
- participação dos integrantes no repositório GitHub

---

## 7. Referências

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

**Metadata & Attribution**

* **Date:** March 2026

* **Character:** Zahy — Zahroniel Syrran *(from the Zaion Universe)*

* **Character GitHub:** [Zahroniel Syrran](https://github.com/zahroniel-syrran)

* **Author:** Human — Ronildo A. Ferreira

* **Author GitHub:** [Ronildo A Ferreira](https://github.com/ronildo-ferreira)


* **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)