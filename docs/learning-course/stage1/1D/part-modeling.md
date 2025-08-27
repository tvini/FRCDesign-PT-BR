# 1D: Metodologia de Design - Simples Swerve Drivebase 

## Derivando Layout Sketches e Modelagem de Peças

Agora que você criou o layout sketch, você pode começar a modelar as peças individuais.
As dimensões críticas das peças, como o comprimento dos tubos, serão definidas pelo layout sketch.
Dessa forma, os tubos serão atualizados automaticamente sempre que houver alterações no tamanho do drivebase no layout sketch.

### Instruções

Comece **criando uma nova aba de pasta no seu Documento chamada `Drivetrain`**. Em seguida, **crie um novo part studio chamado `Drivetrain`** dentro da pasta `Drivetrain`. **Siga as instruções nos slides** para completar o part studio. Lembre-se de que o Origin Cube deve ser a primeira feature no seu part studio.

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts0.webp" style="width:100%">
      <figcaption>0. O part studio.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts1.webp" style="width:100%">
      <figcaption>1. Comece inserindo o Origin Cube. Em seguida, use a ferramenta <code>Derived</code> para inserir os layout sketches que você desenhou anteriormente no Main Layout Sketch part studio. Essa feature será atualizada automaticamente caso sejam feitas alterações no layout sketch.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts2.webp" style="width:100%">
      <figcaption>2. Use os Featurescripts <code>Extrude Individual</code> e <code>Tube Converter</code> para modelar os tubos. Os tubos de 2"x1" devem ter parede de 1/8" para maior resistência, enquanto o tubo de 2"x2" pode ter parede de 1/16".</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts3.webp" style="width:100%">
      <figcaption>3. Comece com um canto da bellypan. O canto é recortado para criar espaço para o swerve module. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtParts4.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>4. Use a ferramenta de esboço <code>Fillet</code> para adicionar um fillet de 1" de raio nos dois cantos internos do recorte. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtParts5.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Em seguida, use a ferramenta de esboço <code>Circular Pattern</code> para replicar os outros três cantos. Extruda a bellypan com 1/8" de espessura.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts6.webp" style="width:100%">
      <figcaption>6. Use o Featurescript <code>Fillet All Edges</code> para adicionar um fillet de 0,25" de raio às arestas restantes da bellypan, selecionando a face inferior da bellypan.</figcaption>
    </figure>
  </div>

  <!-- <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts7.webp" style="width:100%">
      <figcaption>7. Adicione as instâncias iniciais dos furos da bellypan..</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtParts8.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>8. Em seguida, use a ferramenta <code>Linear Pattern</code> para replicar os furos ao longo da borda.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtParts9.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>9. Use a ferramenta <code>Circular Pattern</code> para replicar os furos em torno da origem, aplicando-os às quatro bordas.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtParts10.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>10. Use a ferramenta <code>Linear Pattern</code> para replicar os furos do tubo 2"x2".</figcaption>
    </figure>
  </div> -->

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts11.webp" style="width:100%">
      <figcaption>7. Adicione os furos de montagem da bellypan. Use uma combinação de <code>Linear Pattern</code> e <code>Circular Pattern</code> para replicar os furos de rebite de 0,196". Você só precisará modelar 2 instâncias iniciais: uma para os furos das bordas e outra para os furos do tubo 2"x2".</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1d/SwerveBase/dtParts12.webm" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>8. Extruda os furos na bellypan. Se o sketch estiver corretamente desenhado, você não precisará selecionar cada furo individualmente.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1d/SwerveBase/dtParts0.webp" style="width:100%">
      <figcaption>9. Por fim, nomeie seus esboços e organize-os em uma pasta na feature tree. Além disso, defina o material da bellypan como Aluminum 6061 e dê nomes às suas peças.</figcaption>
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

### Feature Derived

Nesta seção, você foi apresentado à feature `Derived`. Essa feature é extremamente poderosa e pode ser usada para importar peças de um part studio para outro, permitindo referências para modelagem. No entanto, você deve ter cuidado para não usar excessivamente essa função, pois ela pode diminuir significativamente a performance dos seus part studios.

### Feature Tree Organization

Neste ponto, você deve estar se sentindo cada vez mais confortável com a modelagem no Onshape e com o uso de Featurescripts.
Sempre certifique-se de organizar sua feature tree enquanto trabalha, para mantê-la limpa e fácil de usar.
Você pode aprender mais sobre organização da feature tree em [Feature Tree Best Practices](/best-practices/feature-tree-setup/ "Feature Tree Best Practices Page"){:target="_blank"}.

<br>

