## Leia atentamente o texto e DEPOIS responda os questinamento no final e poste no GitHub do grupo.

# 🌐 IoT — Conceitos Básicos de Eletricidade, Eletrônica, Sensores e Atuadores

## 🎯 Objetivos da aula

Ao final desta aula, o estudante deverá compreender:

* o que são tensão e corrente elétrica;
* a relação entre tensão, corrente e resistência;
* o princípio básico da Lei de Ohm;
* o que é um microcontrolador;
* o que são sensores e atuadores;
* como esses elementos trabalham juntos em um projeto de IoT.

---

# 1. IoT e o mundo físico

IoT significa **Internet of Things**, ou **Internet das Coisas**.

Em muitos projetos de IoT, um sistema precisa:

1. perceber alguma informação do ambiente;
2. processar essa informação;
3. tomar uma decisão;
4. executar alguma ação;
5. em alguns casos, comunicar os dados por uma rede.

Por exemplo, imagine um sistema automático para controlar a iluminação de uma sala:

```text
Luminosidade do ambiente
        ↓
      Sensor
        ↓
 Microcontrolador
        ↓
     Decisão
        ↓
      Relé
        ↓
     Lâmpada
```

O sensor percebe a luminosidade.

O microcontrolador analisa a informação.

Se estiver escuro, ele poderá acionar um dispositivo que liga a lâmpada.

Antes de desenvolver sistemas desse tipo, precisamos compreender alguns conceitos básicos de eletricidade.

---

# ⚡ 2. Tensão elétrica

A **tensão elétrica** representa uma diferença de potencial elétrico entre dois pontos.

Sua unidade de medida é o:

**Volt (V)**

Podemos fazer uma comparação simplificada com um sistema de água.

Imagine uma caixa-d'água:

```text
     Caixa-d'água
         │
         │ pressão
         ▼
       Cano
         │
         ▼
      Torneira
```

Quanto maior a diferença de pressão, maior será a tendência de a água se movimentar.

Na eletricidade, podemos pensar na tensão como algo semelhante à **diferença de pressão que impulsiona as cargas elétricas**.

Exemplos comuns:

```text
Pilha AA ................. 1,5 V
USB tradicional .......... 5 V
Algumas placas ........... 3,3 V
```

> A analogia com água serve apenas para ajudar na compreensão inicial. Eletricidade e sistemas hidráulicos não são exatamente a mesma coisa.

---

# 🔌 3. Corrente elétrica

A **corrente elétrica** representa o movimento de cargas elétricas através de um material.

Sua unidade de medida é:

**Ampere (A)**

Também encontramos frequentemente:

```text
mA = miliampere
```

Sendo:

```text
1 A = 1000 mA
```

Utilizando novamente a comparação com água:

```text
Tensão  → pressão

Corrente → quantidade de água
           passando pelo cano
```

Em um circuito eletrônico, diferentes componentes podem utilizar diferentes quantidades de corrente.

Esse ponto é muito importante em IoT.

Um microcontrolador possui limites para a quantidade de corrente que pode fornecer ou receber em seus pinos.

---

# ⚠️ 4. Tensão e corrente não são a mesma coisa

Um erro comum é confundir esses dois conceitos.

Podemos pensar, de maneira simplificada:

```text
Tensão
↓
"força" que favorece o movimento das cargas

Corrente
↓
fluxo das cargas elétricas
```

Portanto:

```text
Volt (V)
≠
Ampere (A)
```

Os dois conceitos estão relacionados, mas representam grandezas diferentes.

---

# 🧱 5. Resistência elétrica

Existe ainda outra grandeza importante:

**resistência elétrica**

Ela representa a oposição à passagem da corrente elétrica.

Sua unidade é:

**Ohm (Ω)**

Um resistor é um componente eletrônico utilizado para controlar ou limitar a corrente em determinados circuitos.

Exemplo:

```text
Microcontrolador
      │
      ▼
   Resistor
      │
      ▼
     LED
```

O resistor pode ajudar a limitar a corrente que passa pelo LED.

Sem a resistência adequada, uma corrente excessiva poderá danificar o componente.

---

# ⚡ 6. Lei de Ohm

Tensão, corrente e resistência estão relacionadas pela **Lei de Ohm**.

genui{"learning_viz":{"type_id":"OHMS_LAW","locale_override":"pt-BR"}}

Onde:

```text
I = corrente elétrica (A)

V = tensão elétrica (V)

R = resistência elétrica (Ω)
```

A mesma relação pode ser reorganizada para determinar outras grandezas.

```text
V = R × I
```

ou:

```text
R = V / I
```

---

# 🧮 7. Pequeno exemplo

Imagine:

```text
Tensão = 5 V

Resistência = 1000 Ω
```

A corrente será:

```text
I = V / R

I = 5 / 1000

I = 0,005 A
```

Como:

```text
1 A = 1000 mA
```

temos:

```text
0,005 A = 5 mA
```

A corrente será aproximadamente:

**5 mA**

---

# 💡 8. Por que a Lei de Ohm é importante em IoT?

Imagine que queremos ligar um LED a uma placa.

Não devemos pensar apenas:

> "O LED acendeu."

Também precisamos perguntar:

* Qual é a tensão utilizada?
* Qual corrente poderá circular?
* O LED suporta essa corrente?
* O pino do microcontrolador suporta essa corrente?
* Precisamos utilizar um resistor?

Portanto, eletrônica não significa apenas fazer uma ligação funcionar.

Também precisamos garantir que ela funcione **dentro dos limites dos componentes utilizados**.

---

# 🧠 9. Microcontrolador

Um **microcontrolador** é um pequeno sistema computacional integrado em um único componente.

Ele pode:

* receber informações;
* executar um programa;
* realizar cálculos;
* tomar decisões;
* controlar outros dispositivos.

Em projetos educacionais podemos encontrar plataformas como:

```text
Arduino
ESP32
micro:bit
Raspberry Pi Pico
```

O microcontrolador funciona como uma espécie de **centro de controle** do projeto.

Exemplo:

```text
      ENTRADAS

Sensor de luz ─────┐
                   │
Sensor de temp. ───┤
                   ▼
            MICROCONTROLADOR
                   │
                   ├────────► LED
                   │
                   ├────────► Motor
                   │
                   └────────► Buzzer

                     SAÍDAS
```

---

# 👁️ 10. Sensores

Um **sensor** é um dispositivo capaz de detectar alguma condição ou grandeza do ambiente e fornecer uma informação ao sistema.

Podemos encontrar sensores para detectar:

* temperatura;
* luminosidade;
* umidade;
* distância;
* movimento;
* pressão;
* presença;
* gases;
* som.

Por exemplo:

```text
Temperatura
     ↓
   Sensor
     ↓
Microcontrolador
```

O sensor transforma alguma característica do mundo físico em uma informação que poderá ser utilizada pelo sistema.

---

# 🌡️ 11. Exemplo: sensor de temperatura

Imagine uma estufa.

O sensor mede:

```text
Temperatura = 34 °C
```

O microcontrolador possui uma regra:

```text
SE temperatura > 30 °C
ENTÃO ligar ventilador
```

Temos:

```text
Temperatura
     ↓
   Sensor
     ↓
Microcontrolador
     ↓
    Regra
     ↓
Ventilador
```

O sensor **não precisa decidir o que fazer**.

Sua principal função é fornecer uma informação.

---

# ⚙️ 12. Atuadores

Um **atuador** realiza uma ação no ambiente físico a partir de um comando recebido pelo sistema.

Exemplos:

* LED;
* motor;
* servo motor;
* buzzer;
* relé;
* válvula;
* bomba de água;
* display.

Podemos simplificar:

```text
SENSOR
↓
percebe

MICROCONTROLADOR
↓
processa e decide

ATUADOR
↓
age
```

---

# 🚰 13. Exemplo: sistema de irrigação

Imagine uma pequena horta automatizada.

Um sensor verifica a umidade do solo.

```text
Solo
 ↓
Sensor de umidade
 ↓
Microcontrolador
 ↓
Se estiver seco...
 ↓
Bomba de água
```

Neste exemplo:

### Sensor

```text
Sensor de umidade
```

detecta a condição do solo.

### Microcontrolador

```text
ESP32
```

processa a informação.

### Atuador

```text
Bomba de água
```

executa a ação.

---

# 🏠 14. Outro exemplo: casa inteligente

Imagine um sistema de iluminação automática.

```text
Sensor de presença
        │
        ▼
      ESP32
        │
        ▼
       Relé
        │
        ▼
     Lâmpada
```

Quando uma pessoa entra no ambiente:

```text
Sensor detecta presença

        ↓

Microcontrolador recebe informação

        ↓

Programa toma uma decisão

        ↓

Atuador é acionado
```

---

# 🌐 15. Onde aparece a Internet das Coisas?

Nem todo projeto com sensores e microcontroladores é necessariamente IoT.

Para termos um sistema conectado, podemos acrescentar comunicação em rede.

Por exemplo:

```text
Sensor
   ↓
ESP32
   ↓
Wi-Fi
   ↓
Internet
   ↓
Servidor
   ↓
Aplicativo
```

Agora uma pessoa poderia consultar pelo celular:

```text
Temperatura: 28 °C

Umidade: 62%

Bomba: desligada
```

ou enviar um comando:

```text
Ligar bomba
```

O comando poderia percorrer:

```text
Celular
  ↓
Internet
  ↓
ESP32
  ↓
Relé
  ↓
Bomba
```

É nesse momento que começamos a unir:

**eletrônica + programação + redes + Internet.**

---

# 🔄 16. Entrada, processamento e saída

Uma forma muito útil de analisar projetos é identificar três partes:

```text
ENTRADA
   ↓
PROCESSAMENTO
   ↓
SAÍDA
```

Em sistemas IoT:

```text
Sensor
   ↓
Microcontrolador
   ↓
Atuador
```

Exemplo:

| Etapa         | Componente            |
| ------------- | --------------------- |
| Entrada       | Sensor de temperatura |
| Processamento | ESP32                 |
| Saída         | Ventilador            |

Outro exemplo:

| Etapa         | Componente         |
| ------------- | ------------------ |
| Entrada       | Sensor de presença |
| Processamento | Arduino            |
| Saída         | LED                |

Essa classificação ajuda muito na hora de planejar um projeto.

---

# ⚠️ 17. Cuidados importantes

Ao trabalhar com componentes eletrônicos, não devemos ligar dispositivos sem verificar suas especificações.

Precisamos observar:

* tensão de funcionamento;
* corrente máxima;
* polaridade;
* resistência necessária;
* tensão dos pinos do microcontrolador;
* forma correta de alimentação.

Por exemplo, um dispositivo desenvolvido para trabalhar com:

```text
3,3 V
```

pode não aceitar diretamente:

```text
5 V
```

Da mesma forma, motores e outros atuadores podem exigir mais corrente do que um pino do microcontrolador consegue fornecer.

Nessas situações podem ser necessários componentes adicionais, como:

* resistores;
* transistores;
* módulos de relé;
* drivers;
* fontes externas.

> **Antes de realizar uma ligação, consulte as especificações do componente.**

---

# 🧩 Resumindo

Podemos representar muitos projetos de IoT assim:

```text
MUNDO FÍSICO
     │
     ▼
   SENSOR
     │
     ▼
MICROCONTROLADOR
     │
     ▼
   DECISÃO
     │
     ▼
  ATUADOR
     │
     ▼
MUNDO FÍSICO
```

E, quando há comunicação:

```text
Sensor
  ↓
Microcontrolador
  ↓
Rede / Internet
  ↓
Sistema
  ↓
Microcontrolador
  ↓
Atuador
```

---

# 💭 Questões reflexivas — Trabalho em grupo

As questões seguintes devem ser discutidas pelo grupo. O objetivo não é apenas encontrar uma definição, mas analisar situações e justificar as respostas.

## Questão 1 — O LED acendeu. Está tudo certo?

Um grupo ligou um LED diretamente a um pino de um microcontrolador. O LED acendeu normalmente.

Um dos alunos afirmou:

> "Se acendeu, significa que a ligação está correta."

Vocês concordam?

Expliquem por que conhecer **tensão, corrente e resistência** continua sendo importante mesmo quando aparentemente o circuito está funcionando.

---

## Questão 2 — Escolhendo sensores

Uma escola deseja desenvolver um sistema para evitar que as luzes das salas permaneçam ligadas quando não houver ninguém no ambiente.

O grupo deverá propor uma solução.

Discutam:

* Qual informação precisa ser detectada?
* Que tipo de sensor poderia ser utilizado?
* Qual seria a função do microcontrolador?
* Qual seria o atuador?
* Que decisões o programa precisaria tomar?

Representem a solução utilizando:

```text
ENTRADA → PROCESSAMENTO → SAÍDA
```

---

## Questão 3 — Sensor ou atuador?

Um projeto possui os seguintes componentes:

* sensor de temperatura;
* sensor de luminosidade;
* botão;
* motor;
* LED;
* buzzer;
* ESP32.

Classifiquem cada componente como:

* entrada;
* processamento;
* saída.

Depois respondam:

**Por que um mesmo projeto pode precisar de vários sensores e vários atuadores ao mesmo tempo?**

Apresentem um exemplo.

---

## Questão 4 — Automatizar tudo é sempre melhor?

Imagine um sistema de irrigação que utiliza um sensor de umidade para ligar automaticamente uma bomba de água.

Um estudante sugere:

> "Sempre que o sensor indicar solo seco, a bomba deve ligar imediatamente."

Essa regra é suficiente?

Discutam outros fatores que poderiam ser considerados antes de permitir que o sistema ligue automaticamente a bomba.

Por exemplo:

* defeito no sensor;
* duração da irrigação;
* disponibilidade de água;
* horário;
* possibilidade de acionamento manual;
* falha na comunicação.

Ao final, expliquem por que um sistema automatizado também precisa prever **situações inesperadas**.

---

## Questão 5 — Quando um projeto se torna IoT?

Considere os dois sistemas:

### Sistema A

```text
Sensor de temperatura
        ↓
      Arduino
        ↓
        LED
```

### Sistema B

```text
Sensor de temperatura
        ↓
       ESP32
        ↓
       Wi-Fi
        ↓
      Internet
        ↓
    Aplicativo
```

Os dois sistemas utilizam sensores e microcontroladores.

**Podemos considerar os dois como sistemas de IoT?**

Discutam quais características tornam um dispositivo simplesmente eletrônico ou automatizado e quais características o aproximam do conceito de **Internet das Coisas**.

---

# ✅ Conceitos fundamentais

Ao final da atividade, o grupo deve conseguir relacionar:

```text
Tensão
Corrente
Resistência
Lei de Ohm
       ↓
Circuitos eletrônicos
       ↓
Microcontroladores
       ↓
Sensores
       ↓
Processamento
       ↓
Atuadores
       ↓
Comunicação
       ↓
IoT
```

## Ideia principal

Em IoT, programação e eletrônica trabalham juntas.

> **O sensor permite que o sistema perceba o mundo, o microcontrolador permite que ele processe informações e tome decisões, e o atuador permite que ele interfira no mundo físico.**

Eu manteria essa primeira aula **sem montagem de circuitos complexos**. Na aula prática seguinte, um excelente primeiro experimento seria **microcontrolador + LED + resistor**, usando a Lei de Ohm para explicar por que o resistor está presente; depois, **sensor → microcontrolador → LED**, fazendo a ponte direta entre a teoria desta aula e um sistema real.
