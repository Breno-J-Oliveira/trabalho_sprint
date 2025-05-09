🚦 Visão Geral do Projeto

O objetivo deste trabalho é desenvolver um semáforo inteligente, começando por conceitos básicos de Arduino e evoluindo até uma simulação de cruzamento real com múltiplas vias e botões para pedestres. Cada protótipo adiciona uma funcionalidade nova, mostrando a progressão das ideias e o ganho de complexidade passo a passo.

🔧 Protótipo 1: Semáforo Básico
Link no Tinkercad:
https://www.tinkercad.com/things/crLNLab5RRq-trabalha01

Objetivo: Aprender a conectar LEDs à placa Arduino e programar a sequência de luzes.

Componentes:

3 LEDs (verde, amarelo e vermelho)

Resistores de 220 Ω

Placa Arduino Uno

Protoboard e fios de conexão

Lógica Implementada:

Acende o LED verde por 5 s

Passa para o amarelo por 2 s

Fecha no vermelho por 5 s

Repete em loop

Essa etapa garantiu o entendimento da estrutura básica de hardware e software, servindo de base para as melhorias seguintes.

🚶 Protótipo 2: Botão para Pedestres
Link no Tinkercad:
https://www.tinkercad.com/things/fGDRABPrAXn-trabalho02

Novidade: Inclusão de um botão que simula o pedido de travessia de pedestres.

Como Funciona:

Enquanto o semáforo de veículos está no ciclo normal, o botão fica aguardando ser pressionado.

Ao apertar, o código armazena o pedido e, quando chegar a vez, força o semáforo de carros a ficar vermelho, permitindo que o LED “pedestre verde” acenda.

Benefício: Aproxima o sistema da realidade, onde pedestres podem solicitar a travessia de forma autônoma.

👁️ Protótipo 3: Sensor Infravermelho
Link no Tinkercad:
https://www.tinkercad.com/things/lXt8ejKZsI6-trabalho03

Novo Componente: Sensor infravermelho (IR) para detecção de veículos.

Objetivo: Tornar o semáforo “inteligente” ao ajustar os tempos de cada luz conforme presença de carros.

Fluxo de Funcionamento:

Sensor IR monitora a via;

Se não há carro detectado, reduz o tempo do verde (otimizando espera desnecessária);

Se detectar tráfego intenso, mantém o verde por mais tempo (evita congestionamento).

Vantagem: Eficiência nas trocas de sinal, simulando semáforos adaptativos de grandes centros urbanos.

🚦🏙️ Protótipo Final: Cruzamento Completo
Link no Tinkercad:
https://www.tinkercad.com/things/4wrWFSQffOk-sprint3

Cenário: Duas vias interseccionando em “T” (ou “+”), com semáforos independentes para cada direção.

Funcionalidades Integradas:

Ciclo de semáforo para cada via (verde/amarelo/vermelho)

Botões para pedestres em ambos os lados

Detecção de veículos por sensor IR

Lógica de sincronização para evitar conflitos de sinal

Destaques do Código:

Estrutura modular (funções separadas para cada semáforo e pedestre)

Controle de prioridades (pedestres têm janela especial de travessia)

Ajuste de tempos dinâmico conforme detecção de tráfego

Este protótipo final simula de forma realista a operação de um cruzamento urbano, demonstrando como um semáforo pode ser programado para reagir a diferentes estímulos em tempo real.

🎯 Conclusão
Ao longo dos quatro protótipos, partimos de um simples sequenciador de LEDs até chegar a um semáforo inteligente capaz de:

Controlar fluxos de veículos e pedestres;

Ajustar tempos de sinal via sensor IR;

Simular cruzamentos reais com múltiplas vias e prioridades.

Esse projeto mostra, de maneira prática, a integração de hardware (Arduino, sensores, botões) e software (lógica em C/C++) para criar sistemas inteligentes de controle de tráfego. Fique à vontade para explorar cada link no Tinkercad, clonar o código e propor melhorias!

