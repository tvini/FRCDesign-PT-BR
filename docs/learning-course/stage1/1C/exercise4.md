# 1C: Mecanismos para praticar

## Exercise 4: Gancho telescópico

Nesse exercício, você vai modelar um climber telescópico. Esse mecanismo utiliza os [Bloco de rolamento telecópico GreyT da WCP](https://wcproducts.com/products/greyt-telescope "GreyT Telescope Product Page"){:target="_blank"} e as [Reduções MAXPlanetary da REV](https://www.revrobotics.com/frc/maxplanetary-system/ "Rev MAXPlanetary System Product Page"){:target="_blank"}. Preste bastante atenção com os sketchs do gancho e da caixa de redução quando estiver modelando. 

### Aproveitando componentes COTS.
Utilizar componentes COTS é crucial em uma build season com tempo muito limitado.
Mesmo se você tiver a capacidade de fabricar todas as partes do seu robô, aproveitar peças COTS permite seu time a gastar mais tempo em tarefas mais importantes tipo refinar o design ou testar o robô. 
Isso ajuda você a ter certeza que seu tempo está sendo usado da melhor maneira possível, ao invés de tentar reinventar peças que já estão disponíveis no mercado.

???+ Example "Exercício 4 componentes COTS"
    <div class="grid cards" markdown>

    -   <center><img src="/img/learning-course/stage1c/telescope/greyt.webp" width="100%"></center>

    -   <center><img src="/img/learning-course/stage1c/telescope/maxplanetary.webp" width="100%"></center>

    </div>

    <figure>
      <figcaption>O bloco de rolamento possui uma complexa geometria que seria difícil e gastaria muito tempo para manofaturar para muitos times.
                  A redução MAXPlanetaria é uma forma fácil de conseguir grandes reduções sem precisar de uma redução customizada. (Creditos: WCP, REV)</figcaption>
    </figure>

### Instruções do part studio

**Navege até a aba "Part studio Exercício #4"** no seu documento copiado e  **siga os slides de instruções a seguir** para completar o pat studio para este exercício.

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s0.webp" style="width:100%">
      <figcaption>0. Part Studio final.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s1.webp" style="width:100%">
      <figcaption>1. Comece criando um sketch lateral base dos tubos telescópicos no right plane.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s2.webp" style="width:100%">
      <figcaption>2. Use dois extrudes para cirar os corpos sólidos para os tubos. Depois, use o featurescript Tube Converter para converter os sólidos em tubes de parede fina sem buracos laterais.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s3.webp" style="width:100%">
      <figcaption>3. Adicione os buracos para os blocos de rolamento da WCP em ambos os tubos. As dimensões são da <a href="https://docs.wcproducts.com/greyt-telescope/overview-and-features/tubing-hole-pattern">documentação da WCP</a>.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s4.webp" style="width:100%">
      <figcaption>4. Modele o bloco tampão que fica no topo do tubo menor. Você adicionará buracos que passam pelo bloco tampão após modelar o gancho..</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s5.webp" style="width:100%">
      <figcaption>5. Desenhe o gancho. Preste atenção nas relações no sketch presentes no documento solução.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s6.webp" style="width:100%">
      <figcaption>6. Extrude o gancho. Deppis, extrude os buracos de fixação que furaram o tubo e o bloco tampão. Também adicione o espaçador do gancho.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/telescope/s7.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>7. Modele o espaçador impresso em 3d do gancho. Com o sketch imprinting ativado, nós só precisamos desenhar a linha até onde o bloco impresso em 3d começa. Não há necessidade de usar a função <code>Use</code> para copiar o contorno do gancho para o sketch.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s8.webp" style="width:100%">
      <figcaption>8. Desenhe a placa de acoplamento da redução na face externa do tubo. Deve haver uma pequena folga de 0.01 polegadas entre os espaçadores de fixaçaõ de três oitavos e o tubo para ter certeza que a caixa de redução será montada corretamente. O circulo de construção de 13,75mm representa o carretel. O furo com rosca #10-32 permite que um parafuso seja rosqueado na chapa e encaixe perfeitamente dentro do tubo maior para prender a redução sem interferir com o tubo menor. </figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s9.webp" style="width:100%">
      <figcaption>9. Desenhe a corda do mecanismo apartir de uma linha tangente ao carretel. Note que vamos usar essa linha para fazer um sweep da corda, por isso está linha não pode ser de construção.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s10.webp" style="width:100%">
      <figcaption>10. Extrude a chapa, deopis adicione buracos com metade da grossura da chapa. Os buracos devem deixar 1/16 de polegada de material no fundo. Os buracos com meia grossura permitem que o contato entre a chapa da redução e o tubo seja sólido. A chapa deve ser espelhada para gerar uma chapa oposta no outro lado do tubo.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s11.webp" style="width:100%">
      <figcaption>11. Adicione um buraco de 10-32 para o parafuso que está rosqueado na chapa da caixa de redução. Modele também um espaçador e o eixo do carretel.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s12.webp" style="width:100%">
      <figcaption>12. Modele a corda a partir de um circulo de 3mm no final da linha vertical criada anteriormente. Então, use a função sweep para criar um modelo para a corda. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/s0.webp" style="width:100%">
      <figcaption>13. Termine o part studio nomeando as funções usadas e separando elas em pastas. Também coloque materiais de acordo com o design de referencia. </figcaption>
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

### Instruções do assembly

**Em seguida navegue até a aba "Assembly do exercício #4** no seu documento copiado e **siga as instruções no slides a seguir** para completar esse exercício. 

<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a0.webp" style="width:100%">
      <figcaption>0. Final assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/telescope/a1.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>1. Insira os componentes do climber e com a função group mate fixe apenas os componentes do estágio base com o cubo de origem. Isso é por que o segundo estágio se move relativo ao primeiro estágio, por isso não podemos fixar eles juntos.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a2.webp" style="width:100%">
      <figcaption>2. Fixe os componentes do segundo estágio com a função group mate. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a3.webp" style="width:100%">
      <figcaption>3. Insira e fixe o bloco de rolamento Greyt da WCP do <a href="https://cad.onshape.com/documents/3f21b4b70302525a1e1f2c29/v/4ec8cc58f734f29f41a0fdb8/e/4646e6fc60ff8c4fe2a9d4dd" target="_blank">documento do elevador telescópico GreyT da WCP </a>.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/telescope/a4.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>4. Use dois <code>Slider</code> mates para relacionar os dois estágios do elevador. Usando 2 slider mates, um na base e um no topo, o movimento segundo estágio está parametrizado para mudanças no tamanho no estágio base. assim não precisando explicitar uma distancia de viagem. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a5.webp" style="width:100%">
      <figcaption>5. Fixe o espaçador e replique ele. Insira e fixe o rolamento e o eixo. Note que nós só colocamos um rolamento na chapa, já que a caixa de redução já tem rolamento na sua saída, assim podendo tensionar em excesso o eixo com mais um rolamento.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a6.webp" style="width:100%">
      <figcaption>6. Insira e fixe a redução MAXPlanetaria pelo MKCad. nós usamos a saída de 90° com uma redução de 25:1.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a7.webp" style="width:100%">
      <figcaption>7. Insira, Fixe e replique todos os fixadores necessários.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a8.webp" style="width:100%">
      <figcaption>8. Detalhe do parafuso usado para prender a chapa da caixa de redução no lugar. Esse parafuso faz com que a redução não consiga deslizar.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/telescope/a0.webp" style="width:100%">
      <figcaption>9. Termine o assembly organizando as partes em pastas e nomeando os replicates.</figcaption>
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
    Cerfique-se de você ou um mentor/membro mais experiente do seu time [**revise seu CAD!**](../1A/focusing-on-improvement.md "Focusing on Improvement Page"){:target="_blank"} seu assembly deve ter perto de 27 instancias.

### Vistas seccionada

Vistas seccionadas são uma ferramenta útil e permitem você a ver o interior das partes ou assembly como se estivesse cortando eles. Você pode selecionar um plano, uma face, um cilindro, um cone ou um mate para usar como plano a seccionar. Você também pode escolher se quer incluir ou excluir partes específicas da vista seccionada.

!!! Tip "Criando uma vista seccionada"
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/telescope/section-view.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>Criando uma vista seccionada para ter melhor visão do parafuso.</figcaption>
    </figure>

<br>
