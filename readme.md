Silence Warden: Detector de Som com Display LCD e Barra de LEDs

##Índice
1. Descrição
2. Configuração
3. Requisitos
4. Progresso Atual
5. Briefing do Projeto


## 1. Descrição

Este projeto, denominado Silence Warden, utiliza um sensor de som para detectar variações sonoras e exibir o status dessas variações em um display LCD, além de indicar visualmente através de uma barra de LEDs.

## 2. Configuração

Componentes Utilizados/Software/Bibliotecas:

1. Arduino
2. Sensor de Som
3. Display LCD com Interface I2C
4. LEDs
5. Resistores
6. Jumpers
7. Arduino IDE
8. Biblioteca 'LiquidCrystal_I2C'
9. Biblioteca 'SoftwareSerial'

Passo a Passo de Instalação e Configuração:

1. Clone este repositório.
2. Abra o Arduino IDE e carregue o código silence_warden.ino.
3. Conecte os componentes conforme a seguinte configuração:
    Pino 13: Conectado à saída digital do sensor de som.
    Pinos 2 a 11: Conectados aos LEDs.
4. Certifique-se de que as bibliotecas LiquidCrystal_I2C e SoftwareSerial estão instaladas no Arduino IDE.
5. Faça o upload do código para a placa Arduino.
6. Inicie a monitorização serial para visualizar os contadores de som.

## 3. Requisitos

O projeto deve:

1. Detectar sons acima de um certo limiar utilizando o sensor de som.
2. Incrementar um contador a cada detecção de som.
3. Atualizar uma barra de LEDs para representar o número de sons detectados.
4. Exibir as contagens no display LCD:
    soundCount: Contagem de sons detectados.
    tenThousandCount: Contagem de ciclos de 10.000 detecções.
5. Resetar soundCount ao alcançar 10.000 detecções e incrementar tenThousandCount.

## 4. Progresso Atual

Lista de Funcionalidades:
 -Configuração inicial do display LCD com mensagem de boas-vindas.
 -Detecção de sons utilizando o sensor de som.
 -Atualização e exibição das contagens no display LCD.
 -Atualização da barra de LEDs conforme a contagem de sons detectados.
 -Comunicação serial para monitorar as contagens.

Para próximas versões:
 -Ajuste de sensibilidade do sensor de som.
 -Implementação de armazenamento das contagens em memória não volátil.
 -Adição de modos de operação (e.g., modo de silêncio, modo de alarme).

## 5. Briefing do Projeto

Definição do Projeto:

-O projeto Silence Warden foi criado com o objetivo de monitorar e visualizar variações sonoras em um ambiente. Utilizando um sensor de som, o dispositivo detecta sons acima de um determinado limiar e registra essas detecções em um contador. As informações são exibidas em um display LCD e uma barra de LEDs proporciona uma representação visual das detecções. O projeto pode ser expandido para incluir funcionalidades adicionais, como ajustes de sensibilidade e armazenamento de dados.
