# 1C: Mecanismos para Praticar

## Exercício 6: Troca de Direção

Neste exercício, você irá modelar uma transmissão de potência com uma engrenagem de troca de direção.
Esse mecanismo apresenta uma transmissão 1:1 que inverte o sentido de rotação do motor, o que pode ser útil quando se deseja que dois eixos diferentes sejam acionados pelo mesmo motor, mas girem em direções opostas.
Certifique-se de prestar atenção ao layout e aos sketches das chapas durante a modelagem.

### Espaçadores Impressos em 3D, COTS e de Alumínio Sob Medida
Até agora, você utilizou tanto spacers personalizados gerados com o `Spacer` Featurescript quanto spacers COTS de 3/8" OD da biblioteca MKCad (o [WCP Spacers de alumínio](https://wcproducts.com/products/aluminum-spacers "WCP Aluminum Spacers Product Page"){:target="_blank"}).
Existem prós e contras em usar spacers COTS ou personalizados, que você deve discutir com sua equipe.

Spacers impressos em 3D são uma opção fantástica para equipes com acesso a impressoras 3D, sendo baratos e fáceis de fabricar.
Se você quiser usar spacers de alumínio, mas não tiver acesso a máquinas para cortá-los (por exemplo, um torno), spacers de alumínio COTS podem ser uma boa opção, pois também podem ser estocados previamente.
No entanto, eles podem ser caros e estão disponíveis apenas em certos comprimentos, embora você possa contornar isso facilmente projetando para comprimentos de spacer padrão.

???+ Example "Estoque de Spacers"
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/spacers.webp" width="100%">
      <figcaption>Spacers podem ser impressos em 3D (à esquerda), comprados como spacers COTS pré-cortados (centro) ou fabricados internamente a partir de spacer stock (à direita). (Fonte da imagem: WCP)</figcaption>
    </figure>

Ao modelar, recomenda-se usar o `Spacer` Featurescript para spacers que você irá fabricar internamente (por exemplo, impressão 3D ou usando [round tube stock](https://wcproducts.com/products/shaft-stock "WCP Tube Stock Product Page"){:target="_blank"}) e usar a peça configurável de spacer do MKCad para spacers COTS.
Isso ajuda a deixar claro quais peças são personalizadas e quais são COTS.

### Instruções do Part Studio

**Navegue até a aba "Exercício #6: Part Studio"** no seu documento copiado e **consulte o documento de soluções** para completar o Part Studio deste exercício. Os **slides de instruções a seguir** fornecem apenas um resumo geral e alguns detalhes importantes.

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s0.webp" style="width:100%">
      <figcaption>0. Part Studio finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s1.webp" style="width:100%">
      <figcaption>1. Comece criando o layout sketch no plano Right. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s2.webp" style="width:100%">
      <figcaption>2. Usando um mate connector deslocado 0,5" do plano Right como plano de sketch, desenhe a chapa.  
Preste muita atenção às folgas utilizadas para definir as bordas da chapa.  
A posição dos dois spacers à esquerda do motor é determinada pela tangência entre o spacer de 3/8" OD e o círculo de folga do motor de 2,5".</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="100%" controls>
        <source src="/img/learning-course/stage1c/dir-swap/s3.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>3. Use o <code>Driven Dimension</code> para mostrar a distância entre a engrenagem esquerda e o spacer e verificar se há folga suficiente.  
Uma dimensão driven, ao contrário de uma dimensão driving, apenas informa a distância entre os elementos selecionados e aparece esmaecida em cinza para indicar que não define a geometria do sketch.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s4.webp" style="width:100%">
      <figcaption>4. Espelhe a chapa através do plano Right e adicione o recorte do motor.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s5.webp" style="width:100%">
      <figcaption>5. Se você optar por não usar spacers COTS, pode usar o Featurescript <code>Spacer</code> para criar o spacer da chapa. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s6.webp" style="width:100%">
      <figcaption>6. Modele todos os eixos e correias. Neste ponto, você já deve estar bastante confortável usando os Featurescripts <code>Shaft</code> e <code>Belt & Chain Gen</code>.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s7.webp" style="width:100%">
      <figcaption>7. Faça a magrelaão nas duas chapas. Como as chapas são idênticas, exceto pelo recorte do motor, você pode usar o mesmo sketch para magrelar ambas. Crie apenas um sketch com as ribs.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/s0.webp" style="width:100%">
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

**Em seguida, navegue até a aba "Exercício #6: Assembly"** no seu documento copiado e **consulte o documento de soluções** para completar a assembly deste exercício. Os **slides de instruções a seguir** fornecem apenas um resumo geral e alguns detalhes importantes.

<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a0.webp" style="width:100%">
      <figcaption>0. Assembly finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a1.webp" style="width:100%">
      <figcaption>1. Adicione as peças do Part Studio ao assembly. Como antes, agrupe e fasten os componentes rígidos com o Origin Cube e fasten o Origin Cube à origem do assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a2.webp" style="width:100%">
      <figcaption>2. Fasten o spacer à chapa e replicate ele.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a3.webp" style="width:100%">
      <figcaption>3. Insert, fasten e replicate os rolamentos. Também insert a flex wheel de 2" e o motor Kraken do MKCad.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a4.webp" style="width:100%">
      <figcaption>4. Insert e fasten as polias e os spacers. Use o Configurable Spacer Stack do MKCad para todos os spacers.  
Para as polias, você pode utilizar polias HTD impressas em 3D da biblioteca do MKCad com inserts hexagonais de 1/2".  
Também fasten as correias na posição. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a5.webp" style="width:100%">
      <figcaption>5. Insert, fasten e replicate todos os fasteners necessários.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a6.webp" style="width:100%">
      <figcaption>6. Ao replicate os parafusos da chapa, inverta o lado de montagem deste parafuso para que a porca não bata na correia. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/dir-swap/a0.webp" style="width:100%">
      <figcaption>7. Para finalizar o assembly, organize seus componentes em pastas e nomeie seus replicates.</figcaption>
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
    Certifique-se de que você e/ou um membro/mentor mais experiente da sua equipe [**revise seu CAD!**](../1A/focusing-on-improvement.md "Focusing on Improvement Page"){:target="_blank"} Seu assembly deve ter 38 instâncias.


### Dimensões Driving e Driven

Nos sketches, dimensões driving definem e controlam a geometria, aparecendo em preto e sendo editáveis. Dimensões driven, por outro lado, são cinza claro e refletem a geometria existente sem alterá-la, sendo úteis para manter a intenção do projeto, como preservar uma folga ou espessura específica. 

Para alternar entre elas, clique com o botão direito na dimensão e selecione "Driving/Driven" no menu de contexto — útil quando uma nova dimensão iria sobrecarregar o sketch ou quando você precisa inspecionar a geometria sem alterá-la.

!!! tip "Alternando Entre Dimensões Driving e Driven"
    <figure>
      <video width="100%" controls>
        <source src="/img/learning-course/stage1c/dir-swap/driven-dims.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>Alterne uma dimensão de driving para driven e vice-versa clicando com o botão direito na dimensão. Observe que a dimensão driven será atualizada com base em outras features.</figcaption>
    </figure>

<br>
