# 1C: Mecanismos para Praticar

## Exercício 8: Centralização do Indexer 

Neste exercício, você irá modelar um indexer de centralização para bolas de 9,5" de diâmetro, semelhante ao [1678's 2022 indexer](https://www.youtube.com/watch?v=RiUaItTKomUhttps://www.youtube.com/watch?v=RiUaItTKomU "1678 2022 Robot Reveal Video"){:target="_blank"}. Este mecanismo apresenta belts, correntes, engrenagens e tube crush blocks. Certifique-se de prestar atenção aos sketches das chapas durante a modelagem.

### Crush Blocks (Bloco de Impacto)
Crush blocks impressos em 3D podem ser usados para reforçar tubos de parede fina em assemblies onde os parafusos passam sem uma chapa.  
Como a força dos parafusos vem da força de aperto, sem nada para sustentar as paredes finas, o tubo pode colapsar antes de alcançar a força de aperto adequada.  
Os crush blocks distribuem a carga, permitindo o uso total da força de aperto enquanto mantêm a integridade estrutural do tubo.

Alternativamente, uma "crush plate" (chapa de impacto) também pode ser utilizada para distribuir a força do fixador, alcançando um efeito semelhante ao de um crush block.

Neste exercício, você irá usar um [crush block configurável impresso em 3D](https://cad.onshape.com/documents/e9e11d824a8fd8257028a1dc/v/0c7982f1d3823153c353cbdb/e/b6f099050d1db039691ace49 "Configurable Crush Block Onshape Document"){:target="_blank"}.

???+ example "Crush Blocks e Crush Plates"
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/crush-blocks.webp" width="65%">
      <figcaption>Um crush block impresso em 3D (à esquerda) e uma crush plate (à direita).  
As crush plates tendem a funcionar bem no meio dos tubos, onde pode ser difícil inserir um crush block.</figcaption>
    </figure>

### Instruções do Part Studio

**Navegue até a aba "Exercício #8 Part Studio"** no seu documento copiado e **consulte o documento de soluções** para completar o part studio deste exercício.  
Os **slides de instruções a seguir** fornecem apenas um esboço geral e alguns detalhes-chave.

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s0.webp" style="width:100%">
      <figcaption>0. Part Studio finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s1.webp" style="width:100%">
      <figcaption>1. Comece criando o layout sketch no plano superior.  
Assim como no exercício anterior, definimos a distância entre os rollers espelhando a roda do indexador. Adicionamos 0,016" ao centro a centro da corrente para compensar a folga (stretch) da corrente.  </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s2.webp" style="width:100%">
      <figcaption>2. Modele os tubos 2x1 de parede fina usando Extrude Individual e Tube Converter.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s3.webp" style="width:100%">
      <figcaption>3. Modele as chapas superiores e inferiores. As chapas superiores podem ser modeladas no mesmo sketch, já que estão no mesmo plano. Preste muita atenção às restrições das chapas no documento de soluções.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s4.webp" style="width:100%">
      <figcaption>4. Faça a magrelação das chapas usando o featurescript  <code>Part Lighten</code> Lembre-se de que você pode selecionar um sketch inteiro para selecionar automaticamente todas as ribs. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/index-centering/s5.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Modele a corrente #25 usando o featurescript <code>Belt & Chain Gen</code> </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s6.webp" style="width:100%">
      <figcaption>6. Modele a correia 5mm HTD.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s7.webp" style="width:100%">
      <figcaption>7. Modele os eixos. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/s0.webp" style="width:100%">
      <figcaption>8. Finalize o Part Studio nomeando suas features e organizando-as em pastas. Atribua os materiais das peças conforme necessário. </figcaption>
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

**Em seguida, navegue até a aba "Exercício #8 Part Studio"** no seu documento copiado e **consulte o documento de soluções** para completar o assembly deste exercício.  
Os **slides de instruções a seguir** fornecem apenas um esboço geral e alguns detalhes-chave.

<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/a0.webp" style="width:100%">
      <figcaption>0. Assembly finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/a1.webp" style="width:100%">
      <figcaption>1. Adicione as peças do Part Studio ao assembly. Como antes, faça o group mate dos componentes rígidos com o Origin Cube e faça o mate do Origin Cube com a origem do assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/a2.webp" style="width:100%">
      <figcaption>2. Insira, fasten e replicate os plate spacers de 2" de comprimento e 3/8" de diâmetro externo (OD).  
Insira, fasten e replique os motor spacers de 1,5" de comprimento e 3/8" de diâmetro externo (OD).  
Copie e fasten a chapa inferior da engrenagem ao spacer de 2".  
Insira, fasten e replicate os rolamentos de eixo hexagonal arredondado de 1/2".</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/index-centering/a3.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>3. Insert, fasten e replicate os crush blocks impressos em 3D a partir do documento vinculado no topo desta página.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/a4.webp" style="width:100%">
      <figcaption>4. Insert e fasten o motor, a polia do motor, a polia HTD 48T impressa em 3D com insert hexagonal de 1/2", as engrenagens 30T e os configurable spacer stacks do MKCad.  
Fasten (fixe) a correia na polia. Também fasten os eixos.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/index-centering/a5.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Insert e fasten as polias da corrente. Em seguida, fasten a corrente nas polias.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/index-centering/a6.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>6. Insert e fasten as Omni-wheels de 6" a partir de <a href="https://cad.onshape.com/documents/a65c1d6e95e4616e720a3f09/v/a6fbccfafd4bcd323ed0cb23/e/26e504413265b4491ec033b8?showReturnToWorkspaceLink=true" target="_blank">this document</a> e MAXHubs do MKCad.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/a7.webp" style="width:100%">
      <figcaption>7. Insert, configure e fasten o Configurable Spacer Stack para preencher a folga no eixo da roda.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/a8.webp" style="width:100%">
      <figcaption>8. Insert, fasten e replicate todos os fixadores necessários. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/index-centering/a0.webp" style="width:100%">
      <figcaption>9. Para finalizar o assembly, organize seus componentes em pastas e nomeie seus replicates.</figcaption>
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

!!! Success "Verificação"
    Certifique-se de que você e/ou um membro/mentor mais experiente da sua equipe revise o assembly [**review your CAD!**](../1A/focusing-on-improvement.md "Focusing on Improvement Page"){:target="_blank"} Your assembly should have 63 instances.

<br>
