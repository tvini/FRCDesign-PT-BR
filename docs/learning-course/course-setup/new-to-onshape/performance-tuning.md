# Novo no Onshape

## Ajuste de desempenho
Depois da configuração inicial da conta, o Onshape vai verificar seu navegador para ter certeza que ele é compatível. Dependendo do navegador, configurações adicionais podem ser requeridas para melhorar sua performance.

!!! Tip
    Você pode testar sua performance atual na [Página de teste de compatibilidade do Onshape](https://cad.onshape.com/check "Compatibility Check").

!!! Note
    Se o teste do navegador falhar, você pode tentar usar um navegador diferente. Atualmente, Navegadores baseados em chromium como Chrome, Edge, Opera e etc, são os melhores nevagadores suportados pelo Onshape, mas normalmente o Firefox funciona sem problemas. O Safari normalmente não funciona direito.

### Melhorando a Performance do Chrome
Se você estiver usando o Chrome, você pode tentar modificar as configurações a seguir para melhorar sua velocidade de processamento.

- Primeiro, escreva `chrome://settings/` na barra de pesquisa do Chrome para acessar suas configurações. Certifique-se que a opção "Use graphics acceleration when available" está ativada. Reinicie o Chrome se você precisou ativar essa configuração.

  <center><img src="/img/learning-course/course-setup/performance-tuning/graphicsacceleration.webp" style="width:80%;border:5px solid #ADADAD; border-radius: 2%"></center>

- Vá para `chrome://flags/` e habilite "Override Software Rendering List":

  <center><img src="/img/learning-course/course-setup/performance-tuning/override-rendering-list.png" style="width:80%;border:5px solid #ADADAD; border-radius: 2%"></center>

- E por último tente mudar o "ANGLE graphics backend":

  <center><img src="/img/learning-course/course-setup/performance-tuning/ANGLE-backend.png" style="width:80%; border:5px solid #ADADAD; border-radius: 2%"></center>

Lembre-se que a performance depende dos componentes do seu computador. Nós sugerimos o processo a seguir:

- Escolha um "ANGLE graphics backend": `chrome://flags/#use-angle`
- Clique no botão "Reiniciar"
- [Teste sua performance](https://cad.onshape.com/check "Compatibility Check")

Repita esses passos para cada opção e use a que melhor performar. Aqui estão alguns exemplos, todos retirados da mesma máquina.

<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure markdown="span">
      <img src="/img/learning-course/course-setup/performance-tuning/performance-examples/default.png" style="width:80%; data-description="The default configuration">
      <figcaption>A configuração padrão</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure markdown="span">
      <img src="/img/learning-course/course-setup/performance-tuning/performance-examples/opengl.png" style="width:80%; data-description="OpenGL performance">
      <figcaption>OpenGL</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure markdown="span">
      <img src="/img/learning-course/course-setup/performance-tuning/performance-examples/D3D9.png" style="width:80%; data-description="Direct3D9">
      <figcaption>Direct3D 9</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure markdown="span">
      <img src="/img/learning-course/course-setup/performance-tuning/performance-examples/D3D11.png" style="width:80%; data-description="Direct3D11">
      <figcaption>Direct3D 11</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure markdown="span">
      <img src="/img/learning-course/course-setup/performance-tuning/performance-examples/D3D11on12.png" style="width:80%; data-description="Direct3don12">
      <figcaption>Direct3D 11 on 12</figcaption>
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

No exemplo acima, o Direct3D 11 ganha por pouco do openGL, mas isso nem sempre é o caso.

<br>
