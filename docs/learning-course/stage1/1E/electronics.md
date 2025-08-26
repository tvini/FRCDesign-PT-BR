# 1E: Fluxo de Trabalho do Subsistema - Detalhando o Drivetrain

## Montagem da Eletrônica

Para facilitar a fiação do robô e também a posterior inspeção elétrica, é importante deixar espaço suficiente ao redor de cada componente eletrônico. É recomendável trabalhar junto com a área da elétrica para definir os melhores locais para cada parte do sistema de controle. Normalmente, as equipes tentam montar a eletrônica na bellypan, desde que haja espaço disponível. 

!!! Exemplo
    <figure>
        <img src="\img\learning-course\stage2-drivebase\elec\elecPic.png" style="width:80%">
        <figcaption>Exemplo de disposição de vários componentes eletrônicos em uma bellypan. (Crédito da foto: FRC 3647)</figcaption>
    </figure>

### Componentes Eletrônicos

Abaixo está uma lista dos componentes elétricos mais comuns encontrados em robôs FRC, junto com uma sugestão de localização para montagem. Vale lembrar que a posição pode variar bastante dependendo do restante do robô, por isso, sempre coordene com a área da elétrica para decidir o que é melhor.

!!! note "Componentes Elétricos da FRC"
    | **Componente** | **Função** | **Localização Sugerida** | **Imagem** |
    |---|---|---|---|
    | REV Power Distribution Hub (PDH) ou  CTRE Power Distribution Panel (PDP) | Distribui energia para todos os outros componentes | Bellypan | ![PDH](\img\learning-course\stage2-drivebase\elecComponents\pdh.webp) |
    | Main Breaker | Liga/desliga o robô e protege a eletrônica contra correntes extremamente altas | Local de fácil acesso, próximo ao PDH e à Bateria | ![Main Breaker](\img\learning-course\stage2-drivebase\elecComponents\mbreak.webp) |
    | RoboRIO | Controlador central de todas as operações do robô | Bellypan | ![RoboRIO](\img\learning-course\stage2-drivebase\elecComponents\rio.webp) |
    | Controlador de motor integrado (eg: Falcon 500, Kraken X60) | Alimenta e controla o motor integrado | Não requer montagem elétrica dedicada | ![Integrated motor controller](\img\learning-course\stage2-drivebase\elecComponents\kx60.webp) |
    | Controlador de motor (eg: Spark Max, Talon SRX) | Necessário para alimentar e controlar alguns motores (eg: NEO, CIM) | Próximo ao motor controlado ou no bellypan | ![Discrete motor controller](\img\learning-course\stage2-drivebase\elecComponents\smax.webp) |
    | Rádio do Robô (Robot Radio) | Permite que o robô estabeleça conexão sem fio com o campo ou driver station | Seguir as [diretrizes de montagem do rádio da Vivid Hosting](https://frc-radio.vivid-hosting.net/getting-started/usage/mounting-your-radio "Vivid Hosting Radio Mounting Guidelines"){:target="_blank"}. | ![Robot Radio](\img\learning-course\stage2-drivebase\elecComponents\vh109.webp) |
    | Luz de Sinal do Robô (RSL) | Indica se o robô está ligado e habilitado/desabilitado | Local de fácil visibilidade | ![Robot Signal Light](\img\learning-course\stage2-drivebase\elecComponents\rsl.webp) |
    | Unidade de Medição Inercial (IMU) | Usada para determinar a orientação e aceleração do robô | O ideal é próximo ao centro (na Bellypan ou fixado com fita dupla face ao RoboRIO) | ![Inertial Measurement Unit](\img\learning-course\stage2-drivebase\elecComponents\imu.webp) |
    | Módulo Regulador de Voltagem (VRM) | Pode ser usado para circuitos customizados | Bellypan | ![Voltage Regulator Module](\img\learning-course\stage2-drivebase\elecComponents\vrm.webp) |
    | Hub Pneumático | Controla os componentes pneumáticos | Bellypan | ![Pneumatics Hub](\img\learning-course\stage2-drivebase\elecComponents\pcm.webp) |

<br>
