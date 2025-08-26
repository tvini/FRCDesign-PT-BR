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

### O Que Você Aprendeu

- Como extrudir múltiplos tubos separadamente  
- Como criar e restringir um sketch  
- Como fazer retângulos corretamente  
- Como usar dimensões e relacionamentos básicos  
- Como espelhar usando linhas de construção

---

## Exercício 3.2: Adicionando Travessas

<figure>
  <img src="/img/learning-course/stage1a/3-2-sketch.webp" style="width:100%">
  <figcaption>Edite este sketch</figcaption>
</figure>


Agora vamos aplicar isso ao robô.

Abra o Top Tube Sketch no part studio do Exercício 3.2 e **adicione dois tubos transversais** que fiquem **8 polegadas de distância**.

!!! Tip
    Dê um duplo clique no sketch na árvore de features para editá-lo.

Desenhe as novas travessas você mesmo. Use **apenas uma nova dimensão** no total.

Os únicos números que você deve ver:

- 4,25" (espaço entre módulos)  
- 1" (largura do tubo)  
- 8" (distância entre as travessas)

<figure>
  <img src="/img/learning-course/stage1a/drivetrain-crossrail-sketch2.webp" style="width:90%">
  <figcaption>Configuração final do sketch das travessas.</figcaption>
</figure>

---

### Verifique Seu Trabalho

??? info "Clique aqui depois de terminar seu sketch"

    Aqui está uma forma otimizada de desenhar:

    <iframe width="100%" height="400" src="https://www.youtube.com/embed/ktKuSFVV10U" frameborder="0" allowfullscreen></iframe>

    Compare sua abordagem com o vídeo.  
    > O que você fez diferente?  
    > Como você evitaria erros assim da próxima vez?

<br>

Após verificar seu trabalho e revisar sua abordagem, avance para o próximo exercício.

<br>
