<img width="871" height="80" alt="image" src="https://github.com/user-attachments/assets/5a809363-f6cb-4e26-9273-eae55a86bf44" /># 1C: Mecanismos para Praticar
## Introdução

Bem-vindo à etapa 1C! Nesta etapa, você irá modelar diversos mecanismos diferentes para praticar suas habilidades em CAD e a execução de pequenos detalhes.  
Você será apresentado a novas peças COTS e a dicas e truques do Onshape ao longo do caminho para ajudar no seu fluxo de trabalho.

Como esses mecanismos foram projetados especificamente para ajudar na prática de habilidades e na introdução de conceitos, eles são modelados fora do contexto de um robô completo.  
Embora esses mecanismos incluam algumas boas técnicas de design, eles não são necessariamente sistemas completos.  
Os modelos são estritamente para prática de CAD e não são recomendados para uso em robôs reais.

### Layout Sketches

Certifique-se de usar um layout sketch para cada mecanismo, como os introduzidos nos exercícios da Etapa 1B.  Os layout sketches são úteis em qualquer escala, permitindo definir dimensões-chave em um único sketch, o que facilita ajustes quando necessário.

!!! Dica
    Adicione os componentes que direcionam o design ao layout sketch (por exemplo, transmissão de potência, caminho da peça de jogo, rollers etc.), mantendo os detalhes específicos das peças em seus próprios sketches e features (por exemplo, um sketch separado para os furos dos rolamentos e o contorno da chapa, a ser extrudado).

<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
      <figure>
          <img src="/img/learning-course/stage1c/exercise_1_layout.webp" style="width:80%">
      <figcaptions>Exercício 1 - vista lateral. Observe como o layout sketch direciona a geometria do mecanismo.</figcaption>
      </figure>
  </div>

  <div class="mySlides fade">
      <figure>
          <img src="/img/learning-course/stage1c/exercise_1_layout_final.webp" style="width:80%">
          <figcaptions>Layout sketch do Exercício 1. Observe que apenas os detalhes geométricos principais estão incluídos no layout sketch.</figcaption>
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

!!! Nota
    O conceito de layout sketches será expandido mais adiante, quando você começar a usá-los no contexto de um robô.

### Mantendo Origens Consistentes

Como mencionado nas seções anteriores da Etapa 1, você deve manter uma origem consistente entre seu Part Studio e o assembly. Você irá usar o [`Origin Cube` Featurescript](https://cad.onshape.com/documents/321c197a842fc5f1a29e6621/w/fc3cdd5ca7edcd93e02f13cc/e/2b321cb91b74224b9c14b433 "Origin Cube Featurescript Onshape Document"){:target="_blank"} para alcançar isso. **Certifique-se de que o Origin Cube seja sempre a primeira feature em qualquer Part Studio.** Os slides abaixo fornecem uma demonstração de como usar o Origin Cube.

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/origin-cube-tutorial/origin-cube-tutorial-1.webp" style="width:90%">
      <figcaption> Coloque o featurescript Origin Cube como a primeira feature no Part Studio.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/origin-cube-tutorial/origin-cube-tutorial-2.webp" style="width:90%">
      <figcaption>Modele seu mecanismo.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video controls style="width:80%">
        <source src="/img/learning-course/stage1c/flat-intake/a1.webm" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <figcaption>Insert o Part Studio no assembly usando o check verde.  
Agrupe todas as peças estáticas com a peça Origin Cube e, em seguida, fasten o mate connector do Origin Cube à origem do assembly.</figcaption>
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

Seguir esses passos permitirá que a origem do assembly esteja vinculada a uma peça que nunca mudará ou desaparecerá. A posição das outras peças em relação ao Origin Cube será consistente com o Part Studio, mesmo quando houver alterações no Part Studio.  
Isso será particularmente útil para assemblies flexíveis, como um braço ou elevador, no Stage 2 e seguintes.

<br>

<!-- The following is just notes that can be used in the final content of the page.

Remember, practice is essential – the more CAD models you create, the more proficient and efficient you'll become. Using keyboard shortcuts can significantly accelerate your CAD workflow. Be attentive to best practices to avoid developing any bad habits.


Change this feedback form out and add one at the end of each section? Or do that but keep this one and edit the questions a bit and add one at the end of stage 2, since there's useful content here like the time it takes to complete it that we maybe wouldn't get from the smaller feedback forms? Idk I'll figure this out

Optionally, please fill out [this feedback form](https://forms.gle/J1QNvRkvpi7xyfuU8 "Learning Course Feedback Form"){:target="_blank"} about stages 0 and 1. -->
