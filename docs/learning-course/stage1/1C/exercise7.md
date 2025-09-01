# 1C: Mecanismos para Praticar

## Exercício 7: Rollers Verticais 

Neste exercício, você irá modelar alguns rolos verticais. Este mecanismo apresenta o [Configurable Rollers](https://cad.onshape.com/documents/b75886a5660c38eee7d50e47/w/58faeca16d5b2008a9485b5c/e/6274f59b451ed6222cd7523d "Configurable Rollers Onshape Document"){:target="_blank"} assembly e um spacer de motor impresso em 3D. Certifique-se de prestar atenção ao layout sketch e ao mating do assembly durante a modelagem. 

### Impressão 3D para Reduzir a Quantidade de Peças
A impressão 3D pode ser usada para criar blocos de spacer.  
Em vez de usar múltiplos spacers para conectar dois componentes, podemos optar por usar um bloco impresso em 3D que combine todos os spacers em uma única peça, o que ajuda a reduzir a quantidade de peças e facilita a montagem.  
Se você tiver uma impressora 3D, essa pode ser uma boa opção.

???+ example "Bloco de Spacer Impresso em 3D"
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/3dp-spacer.webp" width="65%">
      <figcaption>Vários spacers podem ser combinados em um único bloco impresso em 3D para reduzir a quantidade de peças. </figcaption>
    </figure>

### Instruções do Part Studio

**Navegue até a aba "Exercício #7: Part Studio"** no seu documento copiado e **consulte o documento de soluções** para completar o Part Studio deste exercício. Os **slides de instruções a seguir** fornecem apenas um resumo geral e alguns detalhes importantes.

<!-- Slideshow container -->
<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s0.webp" style="width:100%">
      <figcaption>0. Part Studio finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s1.webp" style="width:100%">
      <figcaption>1. Comece criando o layout sketch em um mate connector deslocado 3" acima da origem.  
Subtraímos 0,015" de cada c-c da correia para reduzir o atrito, já que estamos conectando múltiplas belts em série.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/vertical-rollers/s2.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>2. Use o <code>Mirror</code> ferramenta do sketch para criar uma referência direita para os rollers e a posição dos tubos. Utilize a distância entre os pares de roller para definir a localização dos rollers. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s3.webp" style="width:100%">
      <figcaption>3. Extrude a placa inferior. Em seguida, crie a placa superior com offset de 5" em relação à placa inferior.  
Preste muita atenção aos sketches das chapas no documento de soluções.  
Observe que o tube plug 1x1" requer 4 furos espaçados 3/8" entre si em um padrão quadrado. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s4.webp" style="width:100%">
      <figcaption>4. Sketch, extrude e, em seguida, use tube convert para transformar em tubo de parede fina 1x1.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s5.webp" style="width:100%">
      <figcaption>5. Modele o bloco de spacer de motor impresso em 3D e extrude-o para ter 1" de comprimento.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s6.webp" style="width:100%">
      <figcaption>6. Modele as correias. O comprimento de passo calculado é ligeiramente menor que um múltiplo de 5 mm, pois subtraímos 0,015" de cada c-c.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s7.webp" style="width:100%">
      <figcaption>7. Use the <code>Assembly Mirror</code> Featurescript to create a reference mate connector for the 1x1 tube. This will be used in the assembly for mating.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/s0.webp" style="width:100%">
      <figcaption>8. Finalize o Part Studio nomeando suas features e organizando-as em pastas. Atribua os materiais das peças conforme necessário.</figcaption>
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

### Instruções do Assembly 

**Em seguida, navegue até a aba "Exercise #7 Assembly"** no seu documento copiado e **consulte o documento de soluções** para completar o assembly deste exercício. Os **slides de instruções a seguir** fornecem apenas um resumo geral e alguns detalhes importantes.

<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/a0.webp" style="width:100%">
      <figcaption>0. Assembly finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/a1.webp" style="width:100%">
      <figcaption>1. Add the part studio parts to the assembly. Like before, group mate the rigid components with the Origin Cube and mate the Origin Cube to the assembly origin.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/vertical-rollers/a2.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>2. Copy the 1x1 tube and fasten the Assembly Mirror mate connectors together.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/a3.webp" style="width:100%">
      <figcaption>3. Insert four 1x1 tube plugs and fasten them into place on the 1x1 tubes.
                    Then, copy and fasten the rest of the frame pieces on the right hand side.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/a4.webp" style="width:100%">
      <figcaption>4. Insert the Configurable Roller assembly from the link at the top of this page.
                  Set the overall roller length to 5" and use 24T pulleys on each end. Duplicate and fasten the roller assembly into place.
                  Then, insert and fasten the motor and motor pulleys. Also fasten the left hand side belts into place. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/vertical-rollers/a5.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Copy and fasten the right hand side belts. 
                  Note that you will need to flip the fasten mate in order for the belt to line up correctly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/a6.webp" style="width:100%">
      <figcaption>6. Insert, fasten, and replicate all of the required fasteners. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/vertical-rollers/a0.webp" style="width:100%">
      <figcaption>7. To finish the assembly, organize your components into folders and name your replicates.</figcaption>
    </figure>
  </div>

  <!-- Next and previous buttons -->
  <button class="prev" onclick="plusSlides(-1,1)" style="background-color: #000; color: #fff;">&#10094;</button>
  <button class="next" onclick="plusSlides(1,1)" style="background-color: #000; color: #fff;">&#10095;</button>
  <!-- The dots/circles -->
  <div class="dotsContainer" style="text-align:center">
    <!-- Dots will be generated here -->
  </div>
</div>

!!! Success "Verification"
    Make sure to have you and/or a more experienced member/mentor of your team [**review your CAD!**](../1A/focusing-on-improvement.md "Focusing on Improvement Page"){:target="_blank"} Your assembly should have 37 instances.


<br>
