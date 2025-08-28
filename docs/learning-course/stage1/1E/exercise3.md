# 1E: Fluxo de Trabalho do Subsistema - Detalhando o Drivetrain


## Exercício: Alívio de Peso da Bellypan

Algumas equipes podem optar por aliviar a bellypan (chapa de base) para reduzir peso e facilitar a fiação. Uma bellypan aliviada pode economizar cerca de 1,3 a 1,8 kg. No entanto, isso pode adicionar um tempo significativo de usinagem se você mesmo fabricar a bellypan, ou aumentar o custo caso opte por comprá-la de um serviço de fabricação (eg: [Fabworks](https://fabworks.com/ "Fabworks Sheet Metal Services"){:target="_blank"}). Sua equipe deve considerar cuidadosamente os prós e contras dessa decisão.

### Instruções

**Se você optar por aliviar a bellypan do seu drivetrain**, pode **seguir as instruções nos slides**, que utilizam o `Vent` [Featurescripts](../../../resources/featurescripts.md "Featurescripts Page"){:target="_blank"}. Você também pode usar os scripts `Lighten`, ou o `Part Lighten` [Featurescripts](../../../resources/featurescripts.md "Featurescripts Page"){:target="_blank"} para aliviar a bellypan. Embora o fluxo de trabalho possa variar levemente entre cada Featurescript, a ideia geral é a mesma. Um padrão em formato de losango é recomendado pela resistência e pela facilidade de modelagem..

<!-- <center>**Sample Bellypan Pocketing Slides**</center> -->
<!-- Slideshow container -->
<div class="slideshow-container">
    <!-- Full-width images with number and caption text -->
    <div id="slide1" class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/pocket/pocket1s0.webp" style="width:100%">
            <figcaption>0. Bellypan aliviada. </figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/pocket/pocket1s1.webp" style="width:100%">
            <figcaption>1. Desenhe duas linhas perpendiculares com deslocamento de 45° da vertical. </figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/pocket/pocket1s2.webp" style="width:100%">
            <figcaption>2. Repita as linhas em padrão linear até cobrirem toda a bellypan. Elas serão as nervuras de reforço.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/pocket/pocket1s3.webp" style="width:100%">
            <figcaption>3. Faça um offset do contorno da bellypan em 0,5”.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/pocket/pocket1s4.webp" style="width:100%">
            <figcaption>4. Conecte quaisquer "ilhas" que possam surgir devido a furos de montagem muito distantes de uma nervura. Uma forma de corrigir é adicionar um rasgo conectando a ilha à nervura.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/pocket/pocket1s0.webp" style="width:100%">
            <figcaption>5. Use um Featurescript de alívio para usinar a bellypan. Configurações recomendadas: nervuras de 0,15” de largura e raio de ferramenta de 3/16”.</figcaption>
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



<br>
