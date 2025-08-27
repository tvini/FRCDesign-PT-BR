# 1D: Metodologia de Design - Simples Swerve Drivebase

## Montagem de um Robô de Alto Nível

Agora que você tem um uma drivebase, você pode criar um robô de alto nível (top level robot assembly). A montagem de robô de alto nível é a mais alta na hierarquia de assemblies. Organizar as montagens dessa forma mantém tudo organizado, tanto do ponto de vista do CAD quanto da montagem na vida real.

Você irá criar um assembly de um robô de alto nível para acompanhar o seu drivetrain. O mecanismo que você irá adicionar é o mecanismo de pontuação do [robô 1678 de 2023]. (https://www.thebluealliance.com/team/1678/2023 "1678 2023 Blue Alliance Page"). O CAD do mecanismo de pontuação pode ser acessado aqui:

<center markdown>[1678 2023 Scoring Mechanism Document](https://cad.onshape.com/documents/28a750426de8e2bc17d5b900/w/8e79c6217ae2ce07ff57d900/e/a4d266d03289620078d13a80 "Team 1678 2023 Scoring Mechanism Onshape Document"){:target="_blank" .md-button .md-button--primary }</center>

### Instruções

Comece **criando uma nova aba de assembly acima do part studio `Main Layout Sketch`** e nomeie-a **`Top Level Robot Assembly`**. **Siga as instruções nos slides** para completar a montagem do robô de alto nível.

<!-- <center>**Top Level Robot Assembly**</center> -->
<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/TopLevel/topL0.webp" style="width:100%">
      <figcaption>0. Robô de alto nível completo.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/TopLevel/topL1.webm" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>1. Insira a montagem do drivetrain e fixe o origin cube na origem do assembly. Pode ser necessário desocultar o origin cube para fazer o mate.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/TopLevel/topL2.webm" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>2.Insira o mecanismo de pontuação da 1678 de 2023 colando o link do mecanismo de pontuação na caixa de texto do menu <code>Insert</code>. Em seguida, fixe o origin cube dessa montagem na origem da assembly. Pode ser necessário ocultar o origin cube do drivetrain para acessar a origem da montagem e realizar o mate.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/TopLevel/topL0.webp" style="width:100%">
      <figcaption>3. Montagem de alto nível completa </figcaption>
    </figure>
  </div>

  <!-- Next and previous buttons -->

<button class="prev" onclick="plusSlides(-1,0)"style="background-color: #000; color: #fff;">&#10094;</button>
<button class="next" onclick="plusSlides(1,0)" style="background-color: #000; color: #fff;">&#10095;</button>

  <!-- The dots/circles -->
  <div class="dotsContainer" style="text-align:center">
    <!-- Dots will be generated here -->
  </div>
</div>

!!! success "Verificação"
Seu gerenciador de abas agora deve se parecer com isto:
<figure>
<img src="/img/learning-course/stage1d/SwerveBase/dtTabManager2.webp" style="width:100%">
</figure>

É isso! A montagem de um robô de alto nível está completa. O uso do origin cube facilita muito o mate entre assemblies. Em etapas futuras, você explorará como criar assemblies flexíveis (braços, elevadores, etc.) utilizando o origin cube. Se tiver interesse, você pode conferir um preview [aqui].(/best-practices/assembly-setup/#utilizing-origin-cube-for-flexible-assemblies "Origin Cube Information Page"){:target="\_blank"}.

<br>
