# 1D: Metodologia de Design - Simple Swerve Drivebase

## Assembly

Agora que o Part Studio está finalizado, você pode criar o assembly do drivetrain

<!-- Previously, in Stage 1A when you created assemblies one of the parts in the group mate was fixed in place. However, this is not considered a good practice as it is not parametric. This is where the origin cube comes in: the origin cube has a mate connector placed at the origin of the part studio.  -->

Assim como nos exercícios de prática do estágio anterior, após inserir e agrupar todas as peças, você deve prender o origin cube à origem do assembly. Isso alinha a origem do Part Studio com a origem do assembly.

### Instruções

Comece **criando uma nova aba de assembly chamada `Drivetrain Assembly`** na pasta `Drivetrain`. **Siga as instruções nos slides** para completar o assembly.

<!-- <center>**Drivetrain Assembly**</center> -->
<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAssy0.webp" style="width:100%">
      <figcaption>0. A montagem.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAssy1.webp" style="width:100%">
      <figcaption>1. Adicione as peças do Part Studio ao assembly. Como antes, faça o group mate dos componentes rígidos com o Origin Cube e faça o mate do Origin Cube à origem do assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtAssy2.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>2. Insira o módulo MK4i do app MKCad no assembly e faça o mate para posicioná-lo corretamente. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtAssy3.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>3. Use a ferramenta de assembly <code>Circular Pattern</code> para finalizar a montagem dos módulos. </figcaption>
    </figure>
  </div>

  <!-- <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtAssy4.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>4. Insira um rebite de 3/16" do app MKCad no assembly e faça o mate. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtAssy5.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Use a ferramenta de assembly <code>Replicate</code> para replicar o rebite e o mate do rebite em toda a geometria correspondente na face inferior do bellypan.</figcaption>
    </figure>
  </div> -->

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAssy4.webp" style="width:100%">
      <figcaption>4. Insira, prenda e replique o rebite de 3/16" do MKCad nos furos do bellypan. Para a feature de replicate, você pode usar "Select edges on face" em vez de "Select individual edges", já que queremos que todos os furos tenham um rebite.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAssy0.webp" style="width:100%">
      <figcaption>5. Para finalizar o assembly, organize seus componentes em pastas e nomeie seus replicates.</figcaption>
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

### Ferramenta Replicate

A ferramenta `Replicate` é uma ferramenta muito poderosa para duplicar peças em assemblies. O `Replicate` funciona criando uma cópia das peças selecionadas e duplicando o mate selecionado na geometria escolhida. Note que a geometria selecionada deve corresponder exatamente à geometria do mate de origem, por exemplo: o diâmetro do furo deve ser o mesmo para que o replicate copie um rebite.

No seu assembly, você usa a opção select the face para aplicar o replicate. Isso identifica toda a geometria que corresponde ao mate original e então copia os componentes e mates selecionados para essas posições correspondentes na face escolhida. Se você quiser replicar apenas em furos específicos, pode alterar o menu suspenso para "Match Individual Edges".

!!! Video "Match Individual Edges para Replicate"
    <video width="1920" controls>
      <source src="/img/learning-course/stage1d/replicateExample.webm" type="video/mp4">
    </video>


<br>
