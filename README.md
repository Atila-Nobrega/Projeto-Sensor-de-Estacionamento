# Projeto-Sensor-de-Estacionamento
Equipe:

* ATILA NOBREGA MAIA AIRES

* LUAN ICARO FERREIRA SANTOS

* TACIO SOARES AGUIAR


Projeto da disciplina de Sistemas Microprocessados - Engenharia de Computação UFC

Nosso projeto busca utilizar um microcontrolador conectado a um sensor ultrassônico e um motor para simular o estacionamento automático e seguro de um veículo em uma determinada distância.

<h2>SOFTWARE:</h2>

* <a href="https://www.labcenter.com/">Proteus</a>
* <a href="https://www.st.com/en/ecosystems/stm32cube.html">STM32Cube IDE</a>

<h2>HARDWARE</h2>

* stm32f103c6
* 1 LED BLUE
* 1 Sensor - HCSR04
* 4 Resistores de 330 Ohm
* 1 AMPOP
* 1 Transistor NPN
* 1 Diodo
* 1 Relé
* 1 Motor DC

<h2>DIAGRAMA:</h2>

<img src="https://github.com/Atila-Nobrega/Projeto-Sensor-de-Estacionamento/blob/main/imagens/diagrama.jpg">


<h2>PROJETO NO PROTEUS:</h2>

<img src="https://github.com/Atila-Nobrega/Projeto-Sensor-de-Estacionamento/blob/main/imagens/projetoproteus.png">

<h2>CONFIGURAÇÃO NO STM32CUBE IDE:</h2>

<img src="https://github.com/Atila-Nobrega/Projeto-Sensor-de-Estacionamento/blob/main/imagens/cubeide.png">

* PA0 configurado para GPIO_Output que será utilizado para o BLUE LED.
* PA1 a PA6 configurados para GPIO_Output e renomeadas de acordo com as entradas do LCD.
* PA8 configurado para GPIO_Input que será conectado ao ECHO do sensor.
* PA9 configurado para GPIO_Output que será conectado ao Trigger do sensor.
* PA10 e PA11 configurado para GPIO_Output que será utilizado para controlar o Motor e seu circuito elétrico.
* TIMERS -> TIM1 -> CLOCK SOURCE = INTERNAL CLOCK

(Opcional): 
* Aumentar o PRESCALE do Timer 
* Utilizar o SYS -> Debug: Serial Wire

<h2>VÍDEO DO PROJETO::</h2>

[![Watch the video](https://img.youtube.com/vi/ZqOWXydNSa4/maxresdefault.jpg)](https://youtu.be/ZqOWXydNSa4)
