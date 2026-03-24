# Sistemas Embarcados

## 1. Introdução

Os sistemas embarcados estão presentes em diversos dispositivos do nosso cotidiano, como carros, eletrodomésticos, celulares e sistemas de automação residencial. Eles são responsáveis por controlar funções específicas de forma eficiente e integrada.

Com o avanço da Internet das Coisas (IoT), esses sistemas passaram a se comunicar pela internet, permitindo monitoramento e controle remoto. Isso amplia suas aplicações em áreas como cidades inteligentes, saúde, indústria e agricultura.

Neste módulo, você irá compreender os principais conceitos relacionados a projetos de sistemas embarcados e como eles são utilizados na prática.

---

## 2. Conceitos fundamentais

### Internet das Coisas (IoT)

A Internet das Coisas refere-se à conexão de dispositivos físicos à internet, permitindo que coletem e troquem dados. Esses dispositivos podem ser sensores, eletrodomésticos ou sistemas industriais.

**Exemplo:** Um sensor de temperatura conectado à internet que envia dados para um aplicativo no celular, permitindo monitoramento remoto.

---

### Movimento maker e tinkering

O movimento maker incentiva a criação, experimentação e aprendizado prático. Já o tinkering envolve explorar e aprender por meio de tentativa e erro.

**Exemplo:** Montar um circuito com Arduino e testar diferentes sensores para entender como funcionam.

---

### Hardware e software open source aplicados à IoT

Hardware e software open source são aqueles com código aberto, permitindo que qualquer pessoa utilize, modifique e compartilhe.

**Exemplo:** Arduino (hardware) e sua IDE (software) permitem criar projetos sem custos elevados.

---

### Microcontroladores

São pequenos computadores em um único chip, responsáveis por controlar dispositivos eletrônicos.

**Exemplo:** O Arduino Uno utiliza um microcontrolador para ler sensores e controlar LEDs.

---

### Sensores e atuadores

Sensores captam informações do ambiente (temperatura, luz, movimento). Atuadores executam ações (ligar LED, mover motor).

**Exemplo:** Um sensor de luz que aciona uma lâmpada automaticamente.

---

### Linguagens de programação para sistemas embarcados

São utilizadas para programar o comportamento dos microcontroladores. As mais comuns são C/C++ e Python (em alguns casos).

**Exemplo:** Código em C++ no Arduino para acender um LED ao pressionar um botão.

---

### IDEs e simuladores

IDEs são ambientes de desenvolvimento para escrever e testar códigos. Simuladores permitem testar projetos sem hardware físico.

**Exemplo:** Tinkercad e Wokwi permitem simular circuitos com Arduino.

---

## 3. Exemplos práticos

### Exemplo 1: Leitura de sensor de temperatura

```cpp
int sensor = A0;
int valor = 0;

void setup() {
  Serial.begin(9600);
}

void loop() {
  valor = analogRead(sensor);
  Serial.println(valor);
  delay(1000);
}
```
Contexto: Monitoramento de temperatura em uma estufa.

## Exemplo 2: Acionamento de LED
```
int led = 13;

void setup() {
  pinMode(led, OUTPUT);
}

void loop() {
  digitalWrite(led, HIGH);
  delay(1000);
  digitalWrite(led, LOW);
  delay(1000);
}
```

Contexto: Sinalização visual intermitente.

## 4. Exercícios

**Exercício 1 — Pergunta conceitual**  
Explique com suas palavras o que é Internet das Coisas (IoT) e cite um exemplo do cotidiano.

**Exercício 2 — Pergunta de aplicação**  
Descreva como um sistema embarcado poderia ser usado para automatizar a iluminação de uma casa.

**Exercício 3 — Pergunta de investigação**  
Utilize o simulador Wokwi ou Tinkercad para montar um circuito com um LED. Teste diferentes tempos de delay e registre o comportamento observado.

**Exercício 4 — Pergunta de reflexão**  
Quais são as vantagens e desvantagens do uso de hardware open source em projetos de IoT?

**Exercício 5 — Pergunta conceitual**  
Qual a função de um microcontrolador em um sistema embarcado?

**Exercício 6 — Pergunta de aplicação**  
Proponha um projeto simples utilizando sensores e atuadores para resolver um problema real.

**Exercício 7 — Pergunta de investigação**  
No simulador, adicione um botão ao circuito do LED. Programe para que o LED acenda apenas quando o botão for pressionado. Descreva o funcionamento.

**Exercício 8 — Pergunta de reflexão**  
Como o movimento maker contribui para o aprendizado em tecnologia?

**Exercício 9 — Pergunta de aplicação**  
Explique como sensores e atuadores trabalham juntos em um sistema de irrigação automatizado.

**Exercício 10 — Pergunta de investigação**  
Explore um projeto pronto no Wokwi ou Tinkercad. Modifique algum parâmetro (tempo, sensor, etc.) e descreva o que mudou.

---

## 5. Instruções para os alunos

- Modalidade: **em dupla**  
- Entrega: **repositório GitHub**  
- Formato: **arquivo Markdown**  
- Nome do arquivo: **1BIM-M1-Conceitos.md**

### Cada aluno deve:

- contribuir com pelo menos **uma resposta**  
- colaborar na organização do documento  

### As respostas devem:

- ter entre **5 e 10 linhas**  
- ser claras e bem organizadas  

### Regras para o repositório:

- cada aluno deve realizar **seus próprios commits**  
- evitar apenas **um único commit final**  
- o histórico deve demonstrar colaboração  

### Caso utilize fontes externas:

- incluir referências  
- seguir normas **ABNT**  

---

## 6. Critérios de avaliação

- Clareza e organização das respostas  
- Qualidade da pesquisa  
- Aplicação correta dos conceitos  
- Capacidade de explicação e argumentação  
- Organização do Markdown  
- Participação no GitHub (commits)  

---

## 7. Referências

ARDUINO. Arduino Documentation. Disponível em: <https://www.arduino.cc>  

TINKERCAD. Simulador de circuitos. Disponível em: <https://www.tinkercad.com>  

WOKWI. Simulador de Arduino online. Disponível em: <https://wokwi.com>  

MONK, Simon. *Programação com Arduino*. Porto Alegre: Bookman, 2013.







