

# 1E: Fluxo de Trabalho do Subsistema - Detalhando o Drivetrain

## Exercício: Montagem da Eletrônica

No design de referência, o Power Distribution Hub (PDH), o disjuntor principal (main breaker), e o RoboRIO são montados na bellypan. O [Featurescript `Electronic Mounting`](https://cad.onshape.com/documents/95c00401c440b44ad8799ef5/w/1f1ebce01a3b8eb6fa102975/e/83cfa4ae1a46ea05581445c9 "Electronic Mounting Featurescript Onshape Document"){:target="_blank"} pode ser muito útil para gerar os furos de montagem dos componentes eletrônicos. e você não puder fabricar com precisão os furos de montagem, a fita dupla face (que vem no Kit of Parts) pode ser uma boa opção para fixar a eletrônica de forma robusta.

### Instruções de Montagem no Bellypan

**Adicione a montagem de alguns componentes eletrônicos ao seu drivetrain.** Você pode se inspirar nos slides de instrução a seguir. 

<!-- <center>**Sample Electronics Mounting Slides**</center> -->
<!-- Slideshow container -->
<div class="slideshow-container">
    <!-- Full-width images with number and caption text -->
    <div id="slide1" class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/elec/elec1s0.webp" style="width:100%">
            <figcaption>0. Eletrônicos montados finalizados.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/elec/elec1s1.webp" style="width:100%">
            <figcaption>1. Desenhe o contorno em forma de caixa para o PDH e o RoboRIO. Também adicione o contorno e os furos para o main breaker. (O Featurescript `Electronic Mounting` infelizmente ainda não suporta furos de montagem para o main breaker).</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <video width="1920" controls>
              <source src="/img/learning-course/stage2-drivebase/elec/elec1s2.webm" type="video/webm">
              Your browser does not support the video tag.
            </video>
            <figcaption>2. Use o Featurescript <code>Electronic Mounting</code> para adicionar os furos de montagem do PDH e do RoboRIO. Opcionalmente, sobrescreva o tamanho do furo do PDH para diâmetro de 5/32”, permitindo que o parafuso de fixação seja rosqueado diretamente na bellypan.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/elec/elec1s0.webp" style="width:100%">
            <figcaption>3. Insira os componentes eletrônicos a partir da biblioteca de peças MKCad e fixe-os. O Pigeon IMU pode ser fixado no RoboRIO.</figcaption>
        </figure>
    </div>
    <!-- Next and previous buttons -->
    <button class="prev" onclick="plusSlides(-1,0)" style="background-color: #000; color: #fff;">&#10094;</button>
    <button class="next" onclick="plusSlides(1,0)" style="background-color: #000; color: #fff;">&#10095;</button>
    <!-- The dots/circles -->
    <div class="dotsContainer" style="text-align:center">
        <!-- Dots will be generated here -->
    </div>
</div>

!!! Tip "Modelos Simplificados"
      Recomenda-se usar modelos eletrônicos **simplificados** para melhorar o desempenho do assembly. Você pode ler mais sobre modelos simplificados na [Página de Boas Práticas de Assembly](/best-practices/assembly-setup/ "Assembly Best Practices Page"){:target="_blank"}. Também podem ser usados modelos simplificados de módulos Swerve para reduzir o lag.

### Luz de Sinal do Robô (RSL)

Todo robô também é obrigado a ter uma Luz de Sinal do Robô (RSL). Um local simples para montar a RSL é na lateral do chassi. Normalmente, apenas uma RSL é necessária e ela precisa ser “facilmente visível a uma distância de 3 pés (~100 cm) de pelo menos um lado do robô”.

**Adicione a montagem de uma RSL ao seu drivetrain da Etapa 1D.** Você pode se inspirar na imagem abaixo. 

<figure>
    <img src="\img\learning-course\stage2-drivebase\elec\RSL.webp" style="width:80%">
    <figcaption>Suporte de RSL construído em policarbonato com 1/8" de espessura. O furo de montagem da RSL tem 1” de diâmetro. O modelo da RSL pode ser encontrado no aplicativo MKCad.</figcaption>
</figure>

### Rádio

Cada robô também é obrigado a ter um rádio. Ele deve ser montado no robô seguindo as [diretrizes de montagem do rádio da Vivid Hosting](https://frc-radio.vivid-hosting.net/getting-started/usage/mounting-your-radio "Vivid Hosting Radio Mounting Guidelines"){:target="_blank"}.



<br>
