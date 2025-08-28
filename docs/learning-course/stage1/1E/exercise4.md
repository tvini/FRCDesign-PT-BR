

# 1E: Fluxo de Trabalho do Subsistema - Detalhando o Drivetrain

## Exercício: Para-choques (Bumpers)
A construção dos bumpers é descrita no manual do jogo de cada ano da FRC. Normalmente, é exigido o uso de dois noodles de piscina de 2,5” de diâmetro apoiados em uma chapa de madeira compensada de 5” de altura e 3/4" de espessura. Consulte sempre o manual mais recente do jogo para conhecer as regras atualizadas sobre bumpers. As regras de recorte e altura em relação ao solo podem variar de ano para ano.

### Modelagem de Bumper
É recomendado posicionar os bumpers em um novo part studio e assembly para manter a árvore de recursos e de montagem organizadas. O nível mínimo de detalhamento deve ser um modelo em bloco do bumper. Algumas equipes podem optar por modelar a madeira, os furos na madeira, suportes em ângulo para a madeira dos bumpers e outros detalhes que auxiliam no processo de fabricação. Você deve se comunicar com os demais membros da equipe para definir o nível de detalhamento necessário.

### Instruções

**Adicione os bumpers ao seu drivetrain.** Você pode se inspirar nos slides a seguir.  

<!-- <center>**Sample Bumper Modeling Slides**</center> -->
<!-- Slideshow container -->
<div class="slideshow-container">
    <!-- Full-width images with number and caption text -->
    <div id="slide1" class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s0.webp" style="width:100%">
            <figcaption>0. Conjunto de bumpers finalizado e inserido na montagem do drivetrain. </figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s1.webp" style="width:100%">
            <figcaption>1. Crie um novo esboço no Main Layout Sketch com o perfil do bumper. É recomendado manter 3/4" de altura do solo e 1/4" de espaço entre o bumper e a estrutura.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s2.webp" style="width:100%">
            <figcaption>2. Crie um novo part studio na pasta do drivetrain para os bumpers. Insira o Origin Cube e derive os esboços do drivetrain e do bumper a partir do Main Layout Sketch.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s3.webp" style="width:100%">
            <figcaption>3. Faça o sweep do perfil do bumper ao longo das arestas do esboço superior do drivetrain para criar o modelo em bloco dos bumpers.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s4.webp" style="width:100%">
            <figcaption>4. Opcionalmente, adicione um filete nos cantos. Ajuste o tamanho de acordo com a forma que sua equipe enrola os macarrões de piscina no bumper.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s5.webp" style="width:100%">
            <figcaption>5. Opcionalmente, modele a madeira dos bumpers. Isso pode ser útil para fins de fabricação.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s6.webp" style="width:100%">
            <figcaption>6. Crie uma montagem de bumpers na pasta do drivetrain e insira todos os componentes. Não esqueça de agrupar os componentes e alinhar o conector do Origin Cube com a origem.</figcaption>
        </figure>
    </div>
    <div class="mySlides fade">
        <figure>
            <img src="/img/learning-course/stage2-drivebase/bumpers/bumper1s0.webp" style="width:100%">
            <figcaption>7. Insira a montagem dos bumpers dentro da montagem do drivetrain.</figcaption>
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

Manter o part studio e o assembly dos bumpers separados do drivetrain mantém a árvore de recursos do drivetrain mais limpa e permite ocultar/exibir os bumpers com mais facilidade no nível superior da montagem, já que você pode mostrar ou esconder todo o conjunto de bumpers de uma vez.




<br>
