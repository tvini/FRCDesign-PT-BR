# 1D: Metodologia de Design - Simples Swerve Drivebase 

## Adicionando Mais Componentes

Quando você modelar mais peças no Part Studio, poderá inseri-las no Assembly de forma semelhante ao que fez antes. Clique em Insert e, em seguida, imediatamente no check verde. Depois, edite o `Group` inicial que você criou e adicione a peça a esse grupo. Fazendo isso, você garante que as peças adicionadas sempre permanecerão na mesma posição em que foram modeladas no Part Studio.

Vamos adicionar um gusset para conectar o tubo de 2"x2" ao tubo de 2"x1".

### Instruções

Comece **navegando até o `Drivetrain` Part Studio** na pasta `Drivetrain`. **Siga as instruções nos slides** para adicionar o gusset.

<!-- <center>**Adding a Gusset**</center> -->
<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAdd0.webp" style="width:100%">
      <figcaption>0. Montagem finalizada do Drivetrain.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAdd1.webp" style="width:100%">
      <figcaption>1. Adicione o gusset ao cruzamento de tubos com o <code>Gusset</code> Featurescript.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtAdd2.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>2. Insira o gusset no assembly e adicione-o ao <code>Group</code>.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAdd3.webp" style="width:100%">
      <figcaption>3. Copie o gusset e faça o mate no outro lado. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtAdd4.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>4. Edite a feature replicate para adicionar rebites ao gusset. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtAdd0.webp" style="width:100%">
      <figcaption>4. Montagem finalizada do Drivetrain. </figcaption>
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

Certifique-se de organizar as instâncias do seu assembly em pastas (ex.: estrutura, swerve modules) e nomeie qualquer pattern e replicates utilizados. Isso ajudará você a localizar os componentes no assembly posteriormente.

!!! success "Verificação"
    Certifique-se de que você e/ou um membro/mentor mais experiente da sua equipe [**revise seu CAD!**](../1A/focusing-on-improvement.md "Focusing on Improvement Page"){:target="_blank"} 
    
    Sua montagem deve pesar aproximadamente 37,2 lbs (16,87 kg)

    Seu gerenciador de abas deve ter as seguintes abas e pasta:
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtTabManager.webp" style="width:100%">
    </figure>

### Nível de Detalhe

Vale notar que, embora modelar todos os detalhes do hardware do robô (parafusos, rebites, porcas) seja útil para compras e montagem na vida real, isso não é estritamente necessário. O tempo é um recurso precioso, especialmente durante a build season, então você deve gastá-lo no que trará o maior retorno.

Mais detalhes sobre as melhores práticas para montagens no Onshape estão disponíveis em [Assembly Best Practices Page](/best-practices/assembly-setup/ "Assembly Best Practices Page"){:target="_blank"}.


<br>
