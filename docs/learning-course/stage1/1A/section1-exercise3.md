# 1A: Fundamentos do Onshape - Seção 1
## Exercício 3: Mais Extrudes

Neste exercício, você irá extrudir quatro retângulos em duas polegadas de forma simétrica — e transformá-los em tubos.  
Use apenas uma função de extrude. O que acontece?

<figure>
  <img src="/img/learning-course/stage1a/exercise3-rectangles.webp" style="width:70%">
  <figcaption>Configuração inicial com quatro retângulos.</figcaption>
</figure>

Não se esqueça: use o Tube Converter após a extrusão.

---

??? question "Parece meio estranho? Clique aqui depois de tentar."

    Se você seguiu as instruções e usou uma única extrusão, provavelmente todos os quatro retângulos se fundiram em um único bloco grande.  
    Na vida real, você não quer que as peças fiquem fundidas assim, a menos que seja intencional.

    > Consegue descobrir como extrudir **individualmente** para mantê-las separadas?

    Se precisar recomeçar, aqui está um vídeo rápido mostrando como deletar seus tubos errados:

    <iframe width="100%" height="400" src="https://www.youtube.com/embed/2Jzb1Xr6NBE" frameborder="0" allowfullscreen></iframe>

---

??? success "Clique aqui se corrigiu sua extrusão."

    Fazer quatro extrudes manualmente é trabalhoso. Existe uma forma melhor!

    - Delete suas extrudes antigas.
  
    - Use o `Extrude Individual` Featurescript que você adicionou em [ferramentas obrigatórias do curso](../../course-setup/required-course-tools/featurescripts.md){:target="_blank"}.  
    - (Pressione `Alt+C` e pesquise "extrude individual", se necessário.)

    Esta ferramenta permite extrudir múltiplas regiões de sketch separadamente, tudo em um único passo.

    Além disso, se você clicar na opção "Symmetric" dentro do Extrude Individual, é possível forçar a simetria.

    <figure>
      <img src="/img/learning-course/stage1a/extrude-individual.webp" style="width:90%">
      <figcaption>Usando "Symmetric" dentro do Extrude Individual.</figcaption>
    </figure>

---

## Exercício 3.1: Fundamentos do Sketch

No último exercício, você extrudiu um sketch existente. Agora é sua vez de **criar o sketch você mesmo**.

Ao fazermos sketches, usamos retângulos para representar tubos quadrados em 2D, e usamos **dimensões** e **restrições** para travar tudo no lugar.

Acompanhe o vídeo abaixo para praticar os fundamentos do sketch no Onshape.

<br>

<figure>
    <iframe width="768" height="432" src="https://www.youtube.com/embed/ftbpbvuZklc" frameborder="0" allowfullscreen></iframe>
</figure>

<br>

!!! tip "Principais Pontos de Sketch"

    - **Dimensões** controlam distâncias (como fazer um retângulo com exatamente 5 polegadas de largura).  
    - **Restrições** definem relacionamentos (como travar uma aresta de retângulo a outra).  
    - **Linhas pontilhadas amarelas** mostram restrições automáticas — use-as!  
    - **A Origem** é sua âncora. Conecte sketches à origem sempre que possível.  
    - **Azul é ruim** — um sketch azul significa que ainda não está totalmente definido. Tudo deve ficar preto.  
    - **Menos é melhor** — use o mínimo de dimensões necessárias para travar totalmente o design.

---

### What You Learned

- How to extrude multiple tubes separately
- How to create and constrain a sketch
- How to make rectangles properly
- How to use basic dimensions and relationships
- How to mirror using construction lines

---

## Exercise 3.2: Adding Rails

<figure>
  <img src="/img/learning-course/stage1a/3-2-sketch.webp" style="width:100%">
  <figcaption>Edit this sketch</figcaption>
</figure>


Now let's apply this to the robot.

Open the Top Tube Sketch in the Exercise 3.2 part studio and **add two cross tubes** that are **8 inches apart**.  

!!! Tip
    Double-click the sketch in the feature tree to edit it.

Draw the new rails yourself. Only use **one new dimension** total.

The only numbers you should see:

- 4.25" (gap between modules)
- 1" (tube width)
- 8" (distance between cross rails)

<figure>
  <img src="/img/learning-course/stage1a/drivetrain-crossrail-sketch2.webp" style="width:90%">
  <figcaption>Final cross rail sketch setup.</figcaption>
</figure>

---

### Check Your Work

??? info "Click here after you finish your sketch"

    Here's an optimized way to sketch it:

    <iframe width="100%" height="400" src="https://www.youtube.com/embed/ktKuSFVV10U" frameborder="0" allowfullscreen></iframe>

    Compare your approach to the video.  
    > What did you do differently?  
    > How would you avoid mistakes like that next time?

<br>

After you're done checking your work and reviewing your approach, move on to the next exercise.

<br>
