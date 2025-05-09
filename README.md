<div align="center">
🚦 Semáforo Inteligente



</div>
📋 Sumário
Visão Geral

Protótipos

Protótipo 1: Semáforo Básico

Protótipo 2: Botão para Pedestres

Protótipo 3: Sensor Infravermelho

Protótipo Final: Cruzamento Completo

Como Usar

Contribuições

Licença

🚀 Visão Geral
Este projeto demonstra a evolução de um semáforo inteligente, desde a ligação de LEDs em um Arduino até um sistema que simula um cruzamento urbano completo com detecção de veículos e botão para pedestres. Cada etapa incorpora novas tecnologias e conceitos de programação embarcada, mostrando como construir soluções IoT simples e eficientes. 
daily.dev

🔧 Protótipos
Protótipo 1: Semáforo Básico
Link Tinkercad:
https://www.tinkercad.com/things/crLNLab5RRq-trabalha01

Objetivo: Conectar LEDs (verde, amarelo, vermelho) ao Arduino e implementar a lógica ciclicamente.
Sequência de Luzes:

cpp
Copiar
Editar
digitalWrite(verde, HIGH);
delay(5000);
digitalWrite(verde, LOW);
digitalWrite(amarelo, HIGH);
delay(2000);
digitalWrite(amarelo, LOW);
digitalWrite(vermelho, HIGH);
delay(5000);
digitalWrite(vermelho, LOW);
(Loop infinito) 
GitHub Docs

Protótipo 2: Botão para Pedestres
Link Tinkercad:
https://www.tinkercad.com/things/fGDRABPrAXn-trabalho02

Novidade: Inclusão de um botão para que o pedestre possa solicitar a travessia.
Fluxo Adicional:

Aguarda pressionamento do botão;

Ao ativar, registra o pedido;

Próxima transição força semáforo de veículos ao vermelho e habilita LED “pedestre verde”. 
daily.dev

Protótipo 3: Sensor Infravermelho
Link Tinkercad:
https://www.tinkercad.com/things/lXt8ejKZsI6-trabalho03

Componente: Sensor IR para detectar presença de veículos.
Lógica Adaptativa:

Sem tráfego → reduz tempo de verde;

Tráfego intenso → estende tempo de verde. 
Shields

Protótipo Final: Cruzamento Completo
Link Tinkercad:
https://www.tinkercad.com/things/4wrWFSQffOk-sprint3

Cenário: Duas vias interseccionando, cada uma com semáforo, sensor IR e botão de pedestre.
Sincronização:

Modularização do código em funções para cada semáforo e pedestre;

Prioridade de travessia para pedestres em janela específica;

Ajuste dinâmico de tempos conforme detecção de tráfego. 
daily.dev
