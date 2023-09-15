# Lixeiras Inteligentes - Longest Wave Tech


## Draft da arquitetura
![Draft da Arquitetura](img/arquitetura.png)

## Visão Geral

As lixeiras inteligentes da Longest Wave Tech possuem um sistema inteligente de gerenciamento de resíduos que utiliza a tecnologia IoT (Internet das Coisas) para monitorar, alertar e melhorar o gerenciamento de lixeiras. Este sistema é projetado para melhorar a eficiência e reduzir o esforço humano envolvido na coleta e monitoramento de resíduos sólidos por meio da integração de dispositivos IoT.

## Componentes IoT Utilizados

- Módulo ESP32 4G
- Sensor Ultrassônico HC-SR04
- Módulo Buzzer
- Display LCD I2C
- Sensor Infravermelho (IR)
- Microservo Motor
- Protoboard
- Jumpers
- Lixeiras

## Funcionamento

São utilizados sensores ultrassônicos para monitorar a altura do lixo em qualquer lixeira. O transmissor ultrassônico emite uma onda ultrassônica que viaja pelo ar e, quando atinge qualquer material, é refletida de volta em direção ao sensor.

Além disso, um sensor infravermelho (IR) é utilizado para detecção de movimento, permitindo que o Smart Bin saiba quando alguém se aproxima para descartar o lixo.

### Buzzer, Display LCD e Microservo Motor

- Quando a capacidade da lixeira atinge um determinado limite (por exemplo, 75%), o módulo Buzzer é ativado, emitindo um sinal sonoro para alertar que a lixeira está quase cheia.
- O Display LCD I2C exibe a capacidade atual da lixeira em tempo real, permitindo uma visualização conveniente.
- O microservo motor pode ser usado para abrir automaticamente a tampa da lixeira quando alguém se aproxima para descartar o lixo. O motor pode ser controlado pelo ESP32 4G para facilitar o descarte de lixo sem a necessidade de tocar na tampa.

## Website e Dashboard

O projeto também inclui um website dedicado. Este website contém um painel de controle com informações sobre as diferentes lixeiras, sua capacidade atual e status de ocupação. O painel exibe a localização das lixeiras em um mapa para uma melhor visualização. Os dados são atualizados em tempo real e fornecem uma visão abrangente do estado das lixeiras.

