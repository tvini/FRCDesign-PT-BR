# 1D: Metodologia de Design - Simples Swerve Drivebase 

## Esboços do Layout do Drivetrain
Para começar, você criará um esboço de layout do drivetrain. Esse esboço irá definir o tamanho e a posição dos tubos de tração. O layout será desenhado a partir da vista lateral e da vista superior do drivetrain. Para o seu swerve drivebase, você o fará com dimensões de 26" x 26".

### Instruções

Comece **criando um novo Documento no Onshape chamado `Stage 1D Robot`** e, dentro dele, **um novo part studio chamado `Main Layout Sketch`**. Em seguida, use o Featurescript `Origin Cube` para criar um origin cube. **Siga as instruções nos slides** para completar o layout sketch.


<!-- <center>**Drivetrain Layout Sketch Slides**</center> -->
<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtFinalLayout.webp" style="width:100%">
      <figcaption>0. Layout sketch finalizado.</figcaption>
    </figure>
  </div>

  <!-- <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/originCube.webp" style="width:100%">
      <figcaption>1. Start by inserting the origin cube.</figcaption>
    </figure>
  </div> -->

  <!-- <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtSideLayout1.webp" style="width:100%">
      <figcaption>2. </figcaption>
    </figure>
  </div> -->

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtSideLayout2.webp" style="width:100%">
      <figcaption>1. Desenhe o perfil lateral do drivetrain no Right Plane. Colocamos o tubo a 1,75" do chão, que é a distância do solo até a parte inferior do tubo para os módulos MK4i.
                  Em seguida, desenhe a área de folga da roda, que representa a área ocupada pela roda.
                  Para os módulos MK4i, a caixa tem 4,625" de largura.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtTopLayout1.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>2. Crie o layout sketch superior usando o mate connector inferior na linha vertical do esboço lateral. A utilização de mate connectors gerados automaticamente para planos de esboço é uma ferramenta muito útil de se ter. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtTopLayout2.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>3. Desenhe o contorno superior da base do drivetrain. Faça o retângulo ser um quadrado e defina o comprimento do lado igual ao comprimento do tubo do esboço lateral. Isso garante que o tamanho do layout superior sempre corresponda ao layout lateral, tornando o design paramétrico. Perceba que o esboço está totalmente definido, mesmo sem possuir dimensões de esboço.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtTopLayout3.webp" style="width:100%">
      <figcaption>4. Para esboçar os tubos, desenhe um quadrado 1" menor que o quadrado anterior.
                    Isso representará os quatro tubos de 2"x1" que compõem a estrutura externa.
                    Em seguida, desenhe o perfil superior do tubo de 2"x2".
                    No canto inferior direito, desenhe duas linhas, cada uma com um offset de 4,25" a partir da borda.
                    Esse é o deslocamento necessário para os módulos MK4i. Outros módulos terão valores diferentes.</figcaption>
    </figure>
  </div>

  <!-- <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtTopLayout4.webp" style="width:100%">
      <figcaption>5. Next, we need to make the cutouts on the drivetube for the swerve modules. Start by drawing two lines, each offset by 4.25" from the edge. This is the required offset for MK4i modules. Other modules will differ.</figcaption>
    </figure>
  </div> -->

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtTopLayout5.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Para aplicar o recorte em todos os quatro tubos, usamos a ferramenta <code>Circular Pattern</code> para copiar as linhas para os quatro cantos.
Para usar <code>Circular Pattern</code>, primeiro definimos o número de instâncias e, em seguida, o eixo de rotação.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtFinalLayout.webp" style="width:100%">
      <figcaption>6. Por fim, nomeie seus sketchs e organize-os em pastas na feature tree. Todos os seus sketch devem estar totalmente definidos.</figcaption>
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

Como explicado anteriormente, este método de top-down modeling é extremamente poderoso, pois permite entender as dimensões mais importantes em um único lugar. No entanto, você deve ter cuidado para não detalhar demais os layout sketches. Você irá praticar layout sketches ao longo de todo o Estágio 2 e os utilizará no Estágio 3, junto com práticas envolvendo múltiplos documentos, para projetar um robô completo.

<br>
