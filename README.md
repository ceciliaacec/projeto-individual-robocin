# Projeto MPU-6050 com STM32F767ZI

Este projeto implementa a comunicação entre o microcontrolador STM32F767ZI e o sensor inercial MPU-6050, permitindo a leitura e interpretação dos dados do giroscópio. A solução calcula o deslocamento angular e a velocidade angular do robô para controle em tempo real.

## Estrutura do Repositório
- `src/`: Código-fonte principal do projeto.
- `stm32/`: Arquivos gerados pelo STM32CubeMX.
- `docs/`: Documentação do projeto, incluindo entregas parciais e finais.
- `tests/`: Arquivos para teste e análise de dados do sensor.

## Como rodar o projeto
1. Configure a pinagem do MPU-6050 com o STM32F767ZI:
   - **VCC**: Conecte ao pino **3.3V**
   - **GND**: Conecte ao **GND**
   - **SCL**: Conecte ao pino **PB8**
   - **SDA**: Conecte ao pino **PB9**
2. Carregue o firmware no microcontrolador.
3. Teste os valores de leitura utilizando o log de testes disponibilizado.

## Resultados esperados
- Leitura contínua de deslocamento angular e velocidade angular em rad/s.
- Comunicação estável entre o sensor e o microcontrolador usando I²C.
- Dados calibrados e filtrados para uso no controle de robôs.

## Ferramentas utilizadas
- Microcontrolador: STM32F767ZI
- Sensor inercial: MPU-6050
- IDE: STM32CubeIDE
- Log de testes: Disponível em `tests/sensor_logs.csv`
