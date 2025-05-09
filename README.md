<div align="center">
🚦 #SemáforoInteligente 🚦
⭐️ ⭐️ ⭐️ ⭐️ ⭐️

</div>
📋 #Sumário
🚀 #VisãoGeral

🔧 #Protótipos

1️⃣ #Protótipo1: SemáforoBásico

2️⃣ #Protótipo2: BotãoPedestres

3️⃣ #Protótipo3: SensorInfrared

🎯 #ProtótipoFinal: CruzamentoCompleto

⚙️ #ComoUsar

🤝 #Contribuições

📝 #Licença

🚀 #VisãoGeral
Bem-vindo ao Semáforo Inteligente! Este repositório mostra a evolução de um sistema de controle de tráfego via Arduino, partindo de um simples sequenciador de LEDs até uma simulação completa de cruzamento urbano com detecção de veículos e chamadas de pedestres. A cada etapa, incorporamos novas funcionalidades, reforçando conceitos de IoT, programação embarcada e design de sistemas adaptativos. Vamos juntos explorar o passo a passo!

🔧 #Protótipos
1️⃣ Protótipo 1: #SemáforoBásico
📌 Link no Tinkercad:

https://www.tinkercad.com/things/crLNLab5RRq-trabalha01

#Objetivo
Conectar LEDs (🟢 verde, 🟡 amarelo, 🔴 vermelho) ao Arduino e programar o ciclo de luzes.

#SequênciaDeLuzes (loop infinito):

cpp
Copiar
Editar
digitalWrite(verde, HIGH);   // 🟢 ON por 5s  
delay(5000);  
digitalWrite(verde, LOW);  

digitalWrite(amarelo, HIGH); // 🟡 ON por 2s  
delay(2000);  
digitalWrite(amarelo, LOW);  

digitalWrite(vermelho, HIGH);// 🔴 ON por 5s  
delay(5000);  
digitalWrite(vermelho, LOW);
✅ Destaque: Base fundamental para entender hardware, protoboard e lógica Arduino.

2️⃣ Protótipo 2: #BotãoPedestres
📌 Link no Tinkercad:

https://www.tinkercad.com/things/fGDRABPrAXn-trabalho02

#Novidade
Adicionamos um botão de pedestre (🚶‍♂️) para solicitar travessia.

#FluxoDeTravessia:

Semáforo de veículos no ciclo normal.

Pedestre pressiona botão → sinal “pedido registrado”.

No próximo ciclo, semáforo de carros vira 🔴 e LED “pedestre verde” acende.

⚡ Impacto: Simula o controle real, garantindo segurança e autonomia para pedestres.

3️⃣ Protótipo 3: #SensorInfrared
📌 Link no Tinkercad:

https://www.tinkercad.com/things/lXt8ejKZsI6-trabalho03

#ComponenteNovo
Sensor infravermelho (IR) para detecção de veículos.

#LógicaAdaptativa:

🌵 Sem tráfego → reduz tempo do 🟢 verde.

🚗 Alto fluxo → estende tempo do 🟢 verde.

🔍 Benefício: Sistema mais eficiente e responsivo, reduzindo esperas desnecessárias.

🎯 Protótipo Final: #CruzamentoCompleto
📌 Link no Tinkercad:

https://www.tinkercad.com/things/4wrWFSQffOk-sprint3

#Cenário
Simulação de cruzamento entre duas vias (“+”), com:

🚦 Dois semáforos independentes

🚶 Botões de pedestres em ambos os lados

👁️ Sensor IR em cada pista

#SincronizaçãoEControle:

Código modular: funções separadas para veículos e pedestres.

Janela de prioridade para travessia de pedestres.

Ajuste dinâmico de tempos conforme fluxo de trânsito.

🌟 Resultado: Representação realista de um sistema urbano inteligente e cooperativo.

