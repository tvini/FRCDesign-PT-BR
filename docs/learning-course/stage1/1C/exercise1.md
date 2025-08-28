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
      <figcaption>8. Desenhe o círculo de parafusos de 2" para a montagem do motor. Você pode utilizar a variável do Origin Cube para criar um furo de folga #10-32 digitando <code>#10_32</code> na dimensão e selecionando a <code>#Clearance_Fit_10_32</code> variável. Use um <code>Circular pattern</code> para replicar o esboço do furo. Embora façamos a repetição do furo 6 vezes, definimos três deles como construction geometry, pois precisamos apenas de 3. Defina o furo mais à esquerda para coincidir com a linha central entre as polias. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s9.webp" style="width:100%">
      <figcaption>9. Desenhe os furos de fixação utilizando um linear pattern. Os furos do tubo têm 0,196" de diâmetro (um ajuste justo de #10-32), então vamos usar o mesmo tamanho para a chapa.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s10.webp" style="width:100%">
      <figcaption>10. Finalize o sketch da chapa desenhando o contorno da chapa ao redor das sketch features.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s11.webp" style="width:100%">
      <figcaption>11. Extruza a chapa com espessura de 1/4".</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s12.webp" style="width:100%">
      <figcaption>12. Crie o sketch de magrelação (chamado de alívio de peso profissionalmente, e nos EUA, o termo pocketing é usado) na face externa da chapa. Desenhe nervuras (ribs) para conectar os pontos de fixação.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s13.webp" style="width:100%">
      <figcaption>13. Use o <code>Part Lighten</code> Featurescript para realizar a magrelação (alívio de peso) na chapa. Usamos espessura de 3/16" para rib e wall thickness, e tool diameter de 0.26"</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s14.webp" style="width:70%">
      <figcaption>14. Você deve ter notado no passo anterior que o pocketing criou alguns relevos indesejados ao longo do contorno externo devido aos furos de fixação. Vamos suavizar essas bordas com um truque simples no próximo slide. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s15.webp" style="width:100%">
      <figcaption>15. Abra o sketch de magrelação e desenhe duas linhas espaçadas com o valor exato da metade da wall thickness da magrelação em relação à borda externa do furo de fixação (NÃO do centro do círculo). No nosso caso, isso seria a metade de 3/16". Esse método “engana” o Featurescript Part Lighten criando uma rib extra onde os relevos teriam aparecido.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s16.webp" style="width:100%">
      <figcaption>16. Edite a feature <code>Part Lighten</code> para incluir as duas novas ribs. A peça com pocketing não deve mais apresentar os relevos. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s17.webp" style="width:100%">
      <figcaption>17. Para criar uma referência para a extrusão do tubo superior, usamos a feature <code>Mirror</code> para espelhar a chapa através do plano Right. Como não queremos realmente usar este componente na assembly, podemos alterar a cor da peça e adicionar <code>zREF</code> ao nome da peça, para que ela apareça no final da lista de peças ao inserir componentes na assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s18.webp" style="width:100%">
      <figcaption>18. Usando o sketch do tubo que criamos anteriormente no Part Studio, agora podemos extrudar o perfil do tubo superior até a face interna da chapa espelhada. Isso garante que o tubo superior seja paramétrico às alterações na largura do intake.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s19.webp" style="width:100%">
      <figcaption>19. Converta o sólido em um tubo 2x1 de parede fina com 0,5" de espaçamento entre os furos (hole spacing). </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s20.webp" style="width:100%">
      <figcaption>20. Sketch e extrude a chapa de policarbonato de 0,125" de espessura na face superior do tubo inferior. Ela terá um furo de fixação em cada canto e ficará afastada 0,125" das bordas do tubo 1x1.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s21.webp" style="width:100%">
      <figcaption>21. Modele o eixo do rolo com o Featurescript <code>Shaft</code>. Você pode estimar o comprimento inicialmente e ajustá-lo depois de criar o assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s22.webp" style="width:100%">
      <figcaption>22. Modele a correia usando o Featurescript <code>Belt & Chain Gen</code>. Use um mate connector deslocado do furo do rolamento da chapa como plano de referência e com offset de 3/8". Selecione os PDs das polias no layout sketch para servir como guias.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/s23.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>23. Use o Featurescript Assembly Mirror (você pode adicioná-lo usando o link acima dos slides). O featurescript irá gerar um mate connector na origem da peça selecionada e outro no centro da peça virtualmente espelhada. A utilização desses dois mate connectors ficará clara quando criarmos a assembly.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/s0.webp" style="width:100%">
      <figcaption>24. Finalize o Part Studio nomeando suas features e organizando-as em pastas. Atribua os materiais das peças conforme necessário.</figcaption>
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

**Em seguida, navegue até a aba "Exercise #1 Assembly"** no seu documento copiado e **siga as instruções dos slides** para completar este exercício.

<div class="slideshow-container">
  <!-- Full-width images with number and caption text -->
  <div id="slide1" class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a0.webp" style="width:100%">
      <figcaption>0. Assembly finalizado.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a1.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>1. Insira todos os componentes do part studio, exceto a peça zREF, e agrupe as chapas, tubos e eixo com o Origin Cube. Fasten (fixe) o cubo na origem.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a2.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>2. Copie a chapa lateral e use os mate connectors gerados pelo Featurescript <code>Assembly Mirror</code> para fasten (fixar) a chapa no lugar. A posição da chapa "espelhada" é totalmente paramétrica, pois os mate connectors gerados pelo Featurescript serão atualizados automaticamente quando houver alterações na chapa. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a3.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>3. Insira os acopladores de tubo (tube plugs) superior e faça uma cópia do tubo inferior. Fasten todos os componentes em suas posições corretas.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a4.webp" style="width:100%">
      <figcaption>4. Insira o motor e as polias do roller (rolo) e fasten na posição. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a5.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>5. Fasten a correia na polia do rolo. Verifique se a polia do motor está corretamente alinhada com a correia.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a6.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>6. Insert e fasten o Configurable Spacer Stack e a flex wheel. O spacer stack é um assembly configurável que calcula automaticamente a melhor combinação de espaçadores para preencher uma folga. Embora essa funcionalidade não seja utilizada neste exercício, será muito útil em exercícios posteriores. Depois de fixar o assembly do Spacer Stack, certifique-se de selecionar os mate connectors pré-gerados em cada extremidade e NÃO o corpo do espaçador. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a7.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>7. Use a feature <code>Linear Pattern</code> para replicar o espaçador e a roda. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <video width="1920" controls>
        <source src="/img/learning-course/stage1c/flat-intake/a8.webm" type="video/webm">
        Your browser does not support the video tag.
      </video>
      <figcaption>8. Copie o Spacer Stack, modifique-o para ter 0,5" de comprimento e, em seguida, fasten na posição para finalizar o roller.</figcaption>
    </figure>
  </div>
  
  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a9.webp" style="width:100%">
      <figcaption>9. Insert, fasten e replicate os rebites (rivets) de 3/16" do MKCad para fixar a chapa ao tubo inferior.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a10.webp" style="width:100%">
      <figcaption>10. Insert, fasten e replicate os parafusos #10-32 de 0,5" da Standard Content Library para fixar o tube plug superior. </figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a11.webp" style="width:100%">
      <figcaption>11. Insert, fasten e replicate os parafusos de 1/2" com 10-32 boltwashers do MKCad para retenção do eixo (shaft).</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a12.webp" style="width:100%">
      <figcaption>12. Insert, fasten e replicate os parafusos #10-32 de 0,5" da Standard Content Library para fixar o motor.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a13.webp" style="width:100%">
      <figcaption>13. Insert, fasten e attach (prender) os parafusos #10-32 de 1,5" da Standard Content Library para fixar a chapa de policarbonato. Adicione também porcas (nuts) finas #10-32 da MKCad Library.</figcaption>
    </figure>
  </div>

  <div class="mySlides fade">
    <figure>
      <img src="/img/learning-course/stage1c/flat-intake/a0.webp" style="width:100%">
      <figcaption>14. Finalize seu assembly organizando as peças em pastas e nomeando seus replicates.</figcaption>
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
    Certifique-se de que você e/ou um membro/mentor mais experiente da sua equipe [**review your CAD!**](../1A/focusing-on-improvement.md "Focusing on Improvement Page"){:target="_blank"} Seu assembly deve ter 32 instâncias.

### Modelagem Paramétrica

Alguns dos passos que seguimos para completar este exercício poderiam ter sido simplificados.  
Por exemplo, não era necessariamente *preciso* usar a feature Assembly Mirror para a chapa.  
Também não era *preciso* usar uma extrusão “Up to face” para o tubo superior.

No entanto, praticamos essas técnicas porque, embora possam aumentar marginalmente o tempo de modelagem inicialmente, elas podem economizar ***quantidades significativas*** de tempo ao voltar e editar.  
O CAD é um processo iterativo — seus modelos e projetos não serão perfeitos na primeira tentativa, portanto, tornar seu modelo mais fácil de modificar e mais robusto a mudanças (por exemplo, alterar a largura deste intake) economizará tempo e esforço a longo prazo.  
À medida que você usar as melhores práticas, elas se tornarão naturais.

!!! question "Ajustando Seu Modelo"
    Experimente modificar elementos para entender o que é e o que não é paramétrico no exercício 1. Você pode tentar alterar a largura, comprimento, posições dos tubos ou a relação de engrenagem. Quais dimensões são fáceis de alterar e quais são mais difíceis? Quais alterações de dimensão causam erros de rebuild ou no assembly?

<br>
