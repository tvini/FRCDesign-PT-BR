# 1A: Fundamentos do Onshape - Seção 1
## Exercício 5: Construindo uma Superestrutura de Tubo
### Introdução

Frames feitos de tubos quadrados (box tube) podem ser adicionados ao topo de um drivetrain para oferecer pontos extras de montagem para mais partes de subsistemas, como um lançador (shooter) ou um braço.

<figure style="margin-bottom: 2rem;">
  <img src="/img/learning-course/stage1a/exercise-5-973-example.webp" style="width:60%; border:5px solid #ADADAD">
  <figcaption>Superestrutura 973 de 2022</figcaption>
</figure>


Neste exercício, vamos adicionar um quadro simples de tubos quadrados ao drivetrain que você criou anteriormente.

<figure>
  <img src="/img/learning-course/stage1a/exercise5-frame.webp" style="width:80%">
  <figcaption>Frame Final de Tubos Retangulares</figcaption>
</figure>

---

### Sketch de Layout e Drivetrain

1. Para planejar corretamente, devemos criar um sketch lateral de layout (como usado anteriormente no Exercício 5).  
2. Comece inserindo o **featurescript do cubo de origem** que você adicionou em [ferramentas obrigatórias do curso](../../course-setup/required-course-tools/featurescripts.md){:target="_blank"}. Lembre-se: você pode procurar ferramentas usando `Alt + C`!  
3. Crie um novo sketch, selecione o `plano direito` e comece a copiar este sketch. Descubra sozinho as restrições necessárias para replicá-lo perfeitamente.

    <figure>
      <img src="/img/learning-course/stage1a/exercise5-frame-sketch.webp" style="width:100%">
      <figcaption>Sketch da superestrutura de tubos</figcaption>
    </figure>

    !!! Info "Posicionamento da Origem"
        As rodas são blocos de 1,75 polegadas nos cantos do tubo. Se for esse o caso, onde a origem está posicionada no layout sketch lateral? Por que você acha que ela está ali? Imagine olhando para o robô de lado na vida real.

4. Após terminar o sketch lateral, crie o quadro do drivetrain swerve no seu part studio de acordo com o que você lembra do exercício anterior. (Lembre-se de selecionar o mate connector!)

    !!! Tip
        Se tiver dificuldade, consulte o vídeo anterior depois de tentar.

    !!! Info "Intenção de Projeto"
        Vamos fazer este drivetrain quadrado. Como você abordaria o sketch superior para evitar usar dimensões desnecessárias? Você deve apenas definir o espaçamento do swerve, a distância entre os tubos transversais (8 polegadas) e o offset (deslocamento) do tubo.

    ??? Hint
        Qual comprimento já está definido/restrito? Você pode usar a restrição de igualdade?



### Modelando o Frame
Até agora, os sketches foram criados nos planos padrão e com mate connectors. Para modelar o tubo da superestrutura acima dos tubos transversais, o sketch deve ser feito na face do tubo transversal, porque é onde você quer que o tubo esteja, mesmo que o tubo transversal mude de posição.

!!! Tip "Intenção de Projeto"
    Isso é chamado de modelagem com "design intent" (intenção de projeto). Existem várias formas de modelar algo, mas você pode escolher formas específicas baseadas na intenção de uma peça ou do design geral. Isso ajuda a evitar bloqueios criativos e erros no CAD quando o design mudar.

<figure>
  <img src="/img/learning-course/stage1a/side profile.webp" style="width:80%">
  <figcaption>Sketch da superestrutura de tubos</figcaption>
</figure>

Assista a uma demonstração desta técnica de sketch abaixo.
<figure>
  <iframe width="768" height="432" src="https://www.youtube.com/embed/_b2Gf8IiEEA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</figure>

Agora que você viu a demonstração, **tente completar a superestrutura de tubos** criando um sketch na face do tubo transversal e projetando linhas do sketch de layout para o novo sketch usando a ferramenta `use`.

### Requisitos
- O quadro de tubos deve ser feito **sem usar nenhuma nova dimensão**, tanto no sketch quanto na extrusão.  
- Edite o Tube Converter para usar paredes de 1/16" de espessura e mude de “centered on tube” para “auto offset”.

!!! Warning "Deslocamento de Tubos"
    A distância entre a borda do tubo e o furo varia entre drivetrains e uso típico.  
    Se você usar "centered on tube" para tubos quadrados comuns, o espaçamento dos furos não estará correto.  
    Use “Centered on tube” apenas para as travessas do drivetrain!

---

### Finalizando

Quando terminar, **faça uma pausa de 5 minutos**.


Depois de retornar, **tente melhorar ou corrigir quaisquer erros que encontrar**. Ao terminar, compare seu fluxo de trabalho com a solução.  **Qual foi o processo de pensamento que levou você a fazer algo diferente?**


<center markdown>[Solution Document](https://cad.onshape.com/documents/5f1057b0e7579ff9dd5811fe/w/4c6a1a1d9747b8ea76b238a3/e/b89eed09a1d075135ee83667){.md-button .md-button--primary target="_blank"}</center>

Assista ao vídeo curto abaixo para aprender como renomear suas features, depois renomeie os sketches e features no seu part studio.  
A partir de agora, queremos **sempre nomear nossos sketches e features**.

<figure>
    <iframe width="768" height="432" src="https://www.youtube.com/embed/ELdwPyFnm4Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</figure>

<br>

Depois de renomear suas features, avance para o próximo exercício.

<br>
