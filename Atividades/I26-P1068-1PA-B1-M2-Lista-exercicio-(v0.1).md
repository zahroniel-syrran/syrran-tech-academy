# Interpretação lógica dos exercícios para criação de programas em Portugol


## Exercícios da página 15/16 da apostila de Portugol Studio

- Modadalidade: em Dupla
- Entrega: Github do grupo

Este material reescreve cada exercício e explica **como pensar logicamente** na construção do programa em Portugol, sem apresentar a solução completa pronta.  
A ideia é treinar a identificação de **entradas**, **processamento** e **saídas**.

---

## Exercício 1

### Enunciado
O Haras Cavalos Brilhantes compra cavalos com frequência. Ler a quantidade de cavalos adquiridos recentemente, calcular a quantidade de ferraduras necessárias para os novos cavalos e exibir a quantidade de novos cavalos e sua respectiva quantidade de ferraduras.

### Como interpretar logicamente
Esse exercício pede para relacionar a quantidade de cavalos com a quantidade de ferraduras.  
A lógica principal é perceber que **cada cavalo usa 4 ferraduras**.

### O que o programa precisa fazer
- Ler a quantidade de cavalos comprados.
- Calcular quantas ferraduras serão necessárias.
- Mostrar os dois valores.

### Entradas
- Quantidade de cavalos.

### Processamento
- Multiplicar a quantidade de cavalos por 4.

### Saídas
- Quantidade de cavalos.
- Quantidade de ferraduras necessárias.

### Raciocínio para montar o programa
1. Declarar uma variável para guardar a quantidade de cavalos.
2. Declarar outra variável para guardar a quantidade de ferraduras.
3. Ler a quantidade de cavalos.
4. Fazer o cálculo das ferraduras.
5. Exibir as informações.

---

## Exercício 2

### Enunciado
Ler o nome e a idade do usuário. Calcular a idade em meses e dias. Exibir o nome e a idade em anos, meses e dias.

### Como interpretar logicamente
Aqui o programa recebe a idade em anos e deve transformá-la também em meses e dias.  
A interpretação lógica é considerar conversões simples de tempo:
- 1 ano = 12 meses
- 1 ano = 365 dias

### O que o programa precisa fazer
- Ler o nome da pessoa.
- Ler a idade em anos.
- Calcular a idade equivalente em meses.
- Calcular a idade equivalente em dias.
- Mostrar tudo.

### Entradas
- Nome.
- Idade em anos.

### Processamento
- Multiplicar a idade por 12 para obter meses.
- Multiplicar a idade por 365 para obter dias.

### Saídas
- Nome.
- Idade em anos.
- Idade em meses.
- Idade em dias.

### Raciocínio para montar o programa
1. Criar uma variável para o nome.
2. Criar variáveis numéricas para idade em anos, meses e dias.
3. Ler nome e idade.
4. Fazer as conversões.
5. Mostrar os resultados de forma organizada.

---

## Exercício 3

### Enunciado
Ler a base e altura de um triângulo. Calcular e exibir a área do triângulo sabendo que área = base * altura / 2.

### Como interpretar logicamente
O exercício já entrega a fórmula.  
A lógica é identificar os valores necessários para aplicar essa fórmula: base e altura.

### O que o programa precisa fazer
- Ler a base.
- Ler a altura.
- Aplicar a fórmula da área.
- Mostrar o resultado.

### Entradas
- Base do triângulo.
- Altura do triângulo.

### Processamento
- Calcular a área usando a fórmula informada no enunciado.

### Saídas
- Base.
- Altura.
- Área do triângulo.

### Raciocínio para montar o programa
1. Declarar variáveis para base, altura e área.
2. Ler base e altura.
3. Aplicar a fórmula.
4. Exibir os dados lidos e o valor calculado.

---

## Exercício 4

### Enunciado
Ler 4 notas, calcular a média ponderada com os pesos 1, 2, 3 e 4 respectivamente e exibir as notas e o resultado da média.

### Como interpretar logicamente
Esse exercício não pede média simples.  
Ele pede **média ponderada**, então cada nota tem um peso diferente:
- primeira nota peso 1
- segunda nota peso 2
- terceira nota peso 3
- quarta nota peso 4

A lógica é:
1. multiplicar cada nota pelo seu peso;
2. somar os resultados;
3. dividir pela soma dos pesos.

### O que o programa precisa fazer
- Ler 4 notas.
- Aplicar os pesos corretos.
- Calcular a média ponderada.
- Mostrar as notas e a média.

### Entradas
- Nota 1
- Nota 2
- Nota 3
- Nota 4

### Processamento
- Multiplicar cada nota pelo peso correspondente.
- Somar os produtos.
- Dividir pela soma total dos pesos.

### Saídas
- As 4 notas.
- A média ponderada.

### Raciocínio para montar o programa
1. Declarar quatro variáveis para as notas.
2. Declarar uma variável para a média.
3. Ler as quatro notas.
4. Fazer o cálculo com os pesos.
5. Mostrar as notas e o resultado final.

---

## Exercício 5

### Enunciado
O motorista de aplicativo abastece o tanque do seu carro com um determinado valor em reais. Ler o preço do litro de combustível e o valor que pretende abastecer. Calcular a quantidade de litro no abastecimento e exibir os dados lidos e o valor calculado.

### Como interpretar logicamente
Esse exercício pede para descobrir quantos litros podem ser comprados com certo valor em dinheiro.  
A lógica é dividir o valor disponível pelo preço de cada litro.

### O que o programa precisa fazer
- Ler o preço do litro.
- Ler o valor em reais que será usado no abastecimento.
- Calcular quantos litros serão abastecidos.
- Mostrar as informações.

### Entradas
- Preço do litro do combustível.
- Valor em reais para abastecer.

### Processamento
- Dividir o valor do abastecimento pelo preço do litro.

### Saídas
- Preço do litro.
- Valor abastecido.
- Quantidade de litros.

### Raciocínio para montar o programa
1. Criar variáveis para preço do litro, valor em reais e litros.
2. Ler os dados.
3. Realizar a divisão.
4. Exibir os valores informados e o resultado.

---

## Exercício 6

### Enunciado
Ler o peso de uma pessoa em quilos, calcular e mostrar o peso em gramas.

### Como interpretar logicamente
É um exercício de conversão de unidade.  
A lógica principal é lembrar que:
- 1 quilo = 1000 gramas

### O que o programa precisa fazer
- Ler o peso em quilos.
- Converter para gramas.
- Exibir o resultado.

### Entradas
- Peso em quilos.

### Processamento
- Multiplicar o peso por 1000.

### Saídas
- Peso em quilos.
- Peso em gramas.

### Raciocínio para montar o programa
1. Declarar uma variável para o peso em quilos.
2. Declarar outra para o peso em gramas.
3. Ler o peso.
4. Fazer a conversão.
5. Mostrar o valor original e o convertido.

---

## Exercício 7

### Enunciado
Ler a base menor, a base maior e a altura. Calcular e mostrar a área de um trapézio: (base menor + base maior) x altura / 2.

### Como interpretar logicamente
O enunciado já traz a fórmula da área do trapézio.  
A lógica é identificar corretamente as três entradas:
- base menor
- base maior
- altura

Depois disso, aplicar a fórmula respeitando a ordem da operação.

### O que o programa precisa fazer
- Ler a base menor.
- Ler a base maior.
- Ler a altura.
- Calcular a área do trapézio.
- Mostrar o resultado.

### Entradas
- Base menor.
- Base maior.
- Altura.

### Processamento
- Somar as duas bases.
- Multiplicar o resultado pela altura.
- Dividir por 2.

### Saídas
- Base menor.
- Base maior.
- Altura.
- Área do trapézio.

### Raciocínio para montar o programa
1. Declarar variáveis para as duas bases, altura e área.
2. Ler os três valores.
3. Aplicar a fórmula corretamente.
4. Exibir os dados e o valor calculado.

---

## Exercício 8

### Enunciado
O vendedor recebe seu salário fixo acrescido de comissões de vendas, calculada a partir do percentual do valor de suas vendas. Ler o salário fixo do vendedor, o valor de suas vendas e o percentual sobre as vendas. Calcular e exibir o salário final do vendedor.

### Como interpretar logicamente
Esse exercício trabalha com salário fixo + comissão.  
A lógica é:
1. descobrir o valor da comissão com base no percentual das vendas;
2. somar a comissão ao salário fixo.

### O que o programa precisa fazer
- Ler o salário fixo.
- Ler o valor das vendas.
- Ler o percentual de comissão.
- Calcular a comissão.
- Calcular o salário final.
- Mostrar os dados e o resultado.

### Entradas
- Salário fixo.
- Valor total das vendas.
- Percentual de comissão.

### Processamento
- Calcular quanto vale a comissão.
- Somar esse valor ao salário fixo.

### Saídas
- Salário fixo.
- Valor das vendas.
- Percentual.
- Salário final.

### Raciocínio para montar o programa
1. Declarar variáveis para salário fixo, vendas, percentual, comissão e salário final.
2. Ler os dados.
3. Calcular a comissão.
4. Calcular o salário final.
5. Exibir todas as informações importantes.

### Atenção lógica
É importante observar como o percentual será usado no cálculo.  
Em programação, normalmente o percentual precisa ser tratado matematicamente antes de ser aplicado ao valor das vendas.

---

## Exercício 9

### Enunciado
Ler o peso de um boi e o percentual de engorda. Calcular e exibir o novo peso do boi.

### Como interpretar logicamente
Esse exercício pede um aumento de peso baseado em percentual.  
A lógica é:
1. calcular quanto representa o percentual de engorda sobre o peso atual;
2. somar esse aumento ao peso original.

### O que o programa precisa fazer
- Ler o peso atual do boi.
- Ler o percentual de engorda.
- Calcular o aumento de peso.
- Calcular o novo peso.
- Exibir o resultado.

### Entradas
- Peso atual do boi.
- Percentual de engorda.

### Processamento
- Descobrir o valor do aumento.
- Somar esse aumento ao peso inicial.

### Saídas
- Peso original.
- Percentual de engorda.
- Novo peso.

### Raciocínio para montar o programa
1. Declarar variáveis para peso atual, percentual, aumento e novo peso.
2. Ler os valores.
3. Calcular o quanto será acrescentado ao peso.
4. Somar ao peso inicial.
5. Mostrar as informações.

---

## Exercício 10

### Enunciado
O caixa do supermercado recebe uma certa quantidade de moedas por dia. Ler a quantidade de moedas recebidas de acordo com cada um dos valores 1, 5, 10, 25 e 50 centavos, e ainda moedas de 1 real. Calcular e exibir o valor recebido de cada um dos tipos de moeda e a soma total em moedas.

### Como interpretar logicamente
Esse exercício exige organização.  
Não basta apenas ler quantas moedas existem. É necessário:
1. ler a quantidade de cada tipo de moeda;
2. calcular o valor correspondente a cada grupo;
3. somar todos os valores no final.

### O que o programa precisa fazer
- Ler a quantidade de moedas de:
  - 1 centavo
  - 5 centavos
  - 10 centavos
  - 25 centavos
  - 50 centavos
  - 1 real
- Calcular quanto cada grupo representa em dinheiro.
- Calcular o valor total.
- Exibir os valores individuais e a soma total.

### Entradas
- Quantidade de moedas de 1 centavo.
- Quantidade de moedas de 5 centavos.
- Quantidade de moedas de 10 centavos.
- Quantidade de moedas de 25 centavos.
- Quantidade de moedas de 50 centavos.
- Quantidade de moedas de 1 real.

### Processamento
- Multiplicar a quantidade de cada moeda pelo seu valor.
- Somar todos os resultados.

### Saídas
- Valor correspondente a cada tipo de moeda.
- Valor total arrecadado.

### Raciocínio para montar o programa
1. Declarar uma variável para a quantidade de cada tipo de moeda.
2. Declarar variáveis para guardar o valor calculado de cada grupo.
3. Declarar uma variável para o total.
4. Ler todas as quantidades.
5. Calcular o valor individual de cada tipo de moeda.
6. Somar tudo no total.
7. Exibir os valores separados e o total final.

### Atenção lógica
Esse exercício pede cuidado com unidades monetárias.  
É importante manter um padrão no cálculo para evitar confusão entre centavos e reais.

---

# Modelo mental para resolver qualquer exercício em Portugol

Antes de programar, tente sempre responder estas 3 perguntas:

## 1. O que entra no programa?
São os dados que o usuário vai digitar.  
Esses dados virarão variáveis de entrada.

## 2. O que o programa faz com esses dados?
É a parte do processamento.  
Pode envolver:
- soma
- subtração
- multiplicação
- divisão
- porcentagem
- conversão de unidade

## 3. O que sai do programa?
São os resultados que precisam ser mostrados na tela.

---

# Estrutura lógica básica em Portugol

Quase todos esses exercícios seguem esta ideia:

1. Declarar variáveis.
2. Ler os dados.
3. Fazer os cálculos.
4. Exibir os resultados.

Essa sequência ajuda a transformar o enunciado em algoritmo de forma clara e organizada.

---

# Dica final de interpretação

Quando ler um exercício, marque mentalmente estas partes:

- **Ler** → indica entrada de dados.
- **Calcular** → indica processamento.
- **Exibir/mostrar** → indica saída.

Se você conseguir separar o enunciado nesses três blocos, a montagem do programa em Portugol fica muito mais fácil.