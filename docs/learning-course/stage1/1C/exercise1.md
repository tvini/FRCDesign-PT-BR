# 1C: Mecanismos para Praticar

## Exercício 1: Intake Plano

Neste exercício, você irá modelar um tipo de manipulador de game pieces planas. Este mecanismo possui um eixo vivo com rodas compliant, redução por correia e acopladores de tubo.

### Acopladores de Tubo (Tube Plugs)
Os acopladores de tubo são uma ótima maneira de construir estruturas simples e robustas.  
Muitos fornecedores, incluindo [WCP](https://wcproducts.com/products/tube-plugs "WCP Tube Plug Product Page"){:target="_blank"}, [REV](https://www.revrobotics.com/MAXTube-Endcaps/ "REV Tube Plugs Product Page"){:target="_blank"}, [Andymark](https://www.andymark.com/products/tube-plugs "Andymark Tube Plug Product Page"){:target="_blank"}, e [Last Anvil](https://lastanvil.com/products/1-x-1-x-0-0625-end-cap "Last Anvil Tube Plug Product Page"){:target="_blank"} oferecem tubos de vários tamanhos.  
Eles podem ser usados para conectar chapas aos tubos ou para conectar tubos entre si sem a necessidade de um gusset.

???+ Example "Tube Plugs"

    <div class="grid cards" markdown>

    -   <center markdown><img src="/img/learning-course/stage1c/flat-intake/high-tide-tube-plugs.webp" width="100%"></center>

    -   <center markdown><img src="/img/learning-course/stage1c/flat-intake/miso-tube-plug.webp" width="100%"></center>

    </div>

    <figure>
      <figcaption>Os acopladores de tubo podem ser usados para criar conexões sem gussets, como tubo a tubo (à esquerda) e tubo a chapa (à direita). (Créditos da foto: FRC 4414, FRC 9442)</figcaption>
    </figure>

Este exercício também apresenta a você o uso do [`Assembly Mirror Featurescript`](https://cad.onshape.com/documents/0f7d68295ff4dab57adcf92c/v/88fbfa19a2e2555d18599db4/e/bcf3052f00f1f9d3d95a89c7?jumpToIndex=1392&showReturnToWorkspaceLink=true "Assembly Mirror FS Onshape Document"){:target="_blank"}. Certifique-se de adicionar isso aos seus Featurescripts, caso você ainda não tenha feito.

- Essa featurescript permite espelhar a posição de uma peça duplicada no assembly. 
- Isso é frequentemente útil para evitar criar uma peça duplicada no Part Studio (para preservar a Lista de Materiais) e manter o assembly paramétrico.
- O featurescript pega uma peça e um plano para espelhar e gera um par de mate connectors para simular um espelhamento no assembly.
- No assembly, basta copiar a peça e conectá-la ao mate connector do outro lado. Para mostrar os mate connectors, pressione a tecla `k`.


### Instruções do Part Studio

**Vá até a aba "Exercise #1 Part Studio"** no seu documento copiado e **siga as instruções dos slides** para completar o Part Studio deste exercício.

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s0.webp" style="width:100%">
      <figcaption>0. Part Studio Finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s1.webp" style="width:100%">
      <figcaption>1. Crie o layout sketch no plano Right. Comece desenhando os contornos dos tubos. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s2.webp" style="width:100%">
      <figcaption>2. Usando as funções do Origin Cube que você aprendeu anteriormente, esboce as polias e a correia. Esta é uma transmissão de pitch de 5 mm, com polias de 12T e 30T e uma correia de 70T. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s3.webp" style="width:100%">
      <figcaption>3. Finalize o layout sketch desenhando um círculo de 60 mm para representar o motor e um círculo de 2" para a roda do intake.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/s4.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>4. Crie o plano do sketch do tubo utilizando como referência um mate connector com offset.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s5.webp" style="width:100%">
      <figcaption>5. Desenhe os tubos traçando sobre o layout sketch. Não deve haver cotas neste sketch.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s6.webp" style="width:100%">
      <figcaption>6. Faça a extrusão do tubo inferior e use o tube converter para transformá-lo em um 1x1 de parede fina com furação espaçada a cada 0,5". O tubo superior será criado em um passo posterior.  </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s7.webp" style="width:100%">
      <figcaption>7. Crie o sketch da chapa na face externa do tubo 1x1. Comece desenhando o furo do rolamento e o furo do motor.</figcaption>
    </figure>
  </div>

  <!-- switch  s8 to a video? -->

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s8.webp" style="width:100%">
      <figcaption>8. Desenhe o círculo de parafusos de 2" para a montagem do motor. Você pode utilizar a variável do Origin Cube para criar um furo de folga #10-32 digitando <code>#10_32</code> na dimensão e selecionando a <code>#Clearance_Fit_10_32</code> variável. Use um <code>Circular pattern</code> para replicar o esboço do furo. Embora façamos a repetição do furo 6 vezes, definimos três deles como geometria de construção, pois precisamos apenas de 3. Defina o furo mais à esquerda para coincidir com a linha central entre as polias. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s9.webp" style="width:100%">
      <figcaption>9. Sketch the mounting holes by using a linear pattern. The tube holes are 0.196" in diameter (A #10-32 "close fit") so we will use the same size for the plate.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s10.webp" style="width:100%">
      <figcaption>10. Finish the plate sketch by drawing the plate outline around the sketch features.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s11.webp" style="width:100%">
      <figcaption>11. Extrude the plate to be 1/4" thick.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s12.webp" style="width:100%">
      <figcaption>12. Create the pocketing sketch on the outside face of the plate. Sketch ribs to connect the mounting points.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s13.webp" style="width:100%">
      <figcaption>13. Use the <code>Part Lighten</code> Featurescript to pocket the plate. We use 3/16" rib and wall thickness, and 0.26" tool diameter.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s14.webp" style="width:70%">
      <figcaption>14. You may have noticed in the previous step that the pocketing created some unsightly bumps along the outside contour as a result of the mounting holes. We will make these edges smooth with a simple trick in the next slide. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s15.webp" style="width:100%">
      <figcaption>15. Open the pocketing sketch and sketch two lines spaced exactly half the pocketing wall thickness away from the outer edge of the mounting hole (NOT the center of the circle). In our case, this would be half of 3/16". This "tricks" the Part Lighten Featurescript by creating an extra rib where the bumps would have been.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s16.webp" style="width:100%">
      <figcaption>16. Edit the <code>Part Lighten</code> feature to include the two new ribs. The pocketed part should no longer have the bumps. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s17.webp" style="width:100%">
      <figcaption>17. To create a reference for extruding the upper tube, we use the <code>Mirror</code> feature to mirror the plate across the Right plane. Since we do not want to actually use this component in the assembly, we can change the color of the part and add <code>zREF</code> to the part name so that it will appear at the very bottom of the part list when inserting parts in the assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s18.webp" style="width:100%">
      <figcaption>18. Using the tube sketch we created earlier in the part studio, we can now extrude the upper tube profile up to the mirrored plate's inside face. This ensures that the upper tube is parametric to changes in intake width.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s19.webp" style="width:100%">
      <figcaption>19. Convert the solid into a 2x1 thin-wall tube with 0.5" hole pattern spacing. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s20.webp" style="width:100%">
      <figcaption>20. Sketch and extrude the 0.125" thick polycarbonate plate on the top face of the bottom tube. It will have a mounting hole in each corner and be spaced away from the edges of the 1x1 tube by 0.125".</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s21.webp" style="width:100%">
      <figcaption>21. Model the roller shaft with the <code>Shaft</code> Featurescript. You can estimate the length first and then adjust it once you create the assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s22.webp" style="width:100%">
      <figcaption>22. Model the belt using the <code>Belt & Chain Gen</code> Featurescript. Use a mate connector offset from the plate's bearing hole as the reference plane and offet by 3/8". Select the layout sketch pulley PDs to use as the guides.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/s23.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>23. Use the Assembly Mirror Featurescript (you can add this using the link above the slides). The featurescript will generate a mate connector at the origin of the selected part, and another at the center of the virtually mirrored part. The usage of these two mate connectors will become clear when we create the assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s0.webp" style="width:100%">
      <figcaption>24. Finish the part studio by naming your features and organizing them into folders. Assign the part materials accordingly.</figcaption>
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

### Assembly Instructions

**Next, navigate to the "Exercise #1 Assembly" tab** in your copied document and **follow the instructions in the slides** to complete this exercise. 

<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a0.webp" style="width:100%">
      <figcaption>0. Final assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a1.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>1. Insert all of the part studio components, except for the zREF part, and group the plates, tubes, and shaft with the origin cube. Fasten the cube to the origin.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a2.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>2. Copy the side plate and use the mate connectors generated by the <code>Assembly Mirror</code> Featurescript to fasten the plate into place. The location of the "mirrored" plate is fully parametric as the mate connectors generated by the Featurescript will automatically update when changes to the plate occur. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a3.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>3. Insert the upper tube plugs and make a copy of the lower tube. Fasten all the components to their correct locations.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a4.webp" style="width:100%">
      <figcaption>4. Insert the motor and roller pulleys and fasten them into place. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a5.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Fasten the belt to the roller pulley. Double check that the motor pulley is properly lined up with the belt.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a6.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>6. Insert and fasten the Configurable Spacer Stack and flex wheel. The spacer stack is a configurable assembly that will automatically calculate the optimal stack of spacers to fill a gap. While this functionality is not used for this exercise, it will be very useful in later exercises. When fastening the Spacer Stack assembly, make sure to select the pre-generated mate connectors on each end and NOT the spacer body. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a7.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>7. Use the <code>Linear Pattern</code> feature to pattern the spacer and wheel.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a8.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>8. Copy the Spacer Stack and modify it to be 0.5" long, then fasten it into place to finish the roller.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a9.webp" style="width:100%">
      <figcaption>9. Insert, fasten, and replicate 3/16" rivets from MKCad to attach the plate to the lower tube.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a10.webp" style="width:100%">
      <figcaption>10. Insert, fasten, and replicate 0.5" long #10-32 bolts from the Standard Content Library for attaching the the tube plug on the upper tube. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a11.webp" style="width:100%">
      <figcaption>10. Insert, fasten, and replicate 1/2" long 10-32 boltwashers from MKCad for shaft retention.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a12.webp" style="width:100%">
      <figcaption>11. Insert, fasten, and replicate 0.5" long #10-32 bolts from the Standard Content Library for attaching the motor.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a13.webp" style="width:100%">
      <figcaption>12. Insert, fasten, and attach 1.5" long #10-32 bolts from the Standard Content Library for attaching the polycarb panel. Also add #10-32 thin jam nuts from MKCad Library.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a0.webp" style="width:100%">
      <figcaption>13. Finish your assembly by organizing the parts into folders and naming your replicates.</figcaption>
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
    Make sure to have you and/or a more experienced member/mentor of your team [**review your CAD!**](../1A/focusing-on-improvement.md "Focusing on Improvement Page"){:target="_blank"} Your assembly should have 32 instances.

### Parametric Modeling

Some of the steps we took to complete this exercise could have been simplified.
For instance, we didn’t necessarily *need* to use the Assembly Mirror feature for the plate.
We didn’t *need* to use an “Up to face” extrude for the upper tube. 

However, we practice these techniques because, while they may marginally increase modeling time upfront, they can save ***significant*** amounts of time when going back and editing.
CAD is an iterative process — your models and designs won’t be perfect the first time around, so making your model easier to modify and more robust to changes (e.g., changing the width of this intake) will save you time and effort in the long run.
As you use best practices, they’ll become second nature.

!!! question "Tweaking Your Model"
    Try playing around to get a feel for what things are and aren't parametric in exercise 1. You can try changing things like the width, length, tube positions, or gear ratio. Which dimensions are easy to change and which are difficult? Which dimension changes cause rebuild or assembly error?

<br>
