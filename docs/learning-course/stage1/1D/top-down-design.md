# 1D: Metodologia de Design - Simples Swerve Drivebase

## Metodologia de Design Top-Down
Ao projetar um modelo em CAD, existem duas estratégias de alto nível que podem ser empregadas: top-down e bottom-up. O top-down design utiliza esboços de alto nível e baixo detalhe para ditar o projeto, refinando depois os detalhes e componentes dentro desse framework. Por outro lado, o bottom-up design envolve criar componentes ou peças individuais separadamente e, em seguida, montá-los para formar o produto final.

O top-down design oferece uma abordagem holística, permitindo melhor integração do sistema, consistência e maior parametricidade. O bottom-up design oferece flexibilidade e independência no projeto de peças individuais. No design de robôs FRC, a abordagem top-down é preferida, pois a integração do sistema costuma ser o aspecto mais desafiador. O top-down garante que a arquitetura do robô dite o design das peças.

### Main Layout Sketch

Para isso, é utilizado um **esboço de layout principal** (main layout sketch). Às vezes, eles também são chamados de esboços "master". O main layout sketch consiste em uma série de esboços que capturam as dimensões principais de cada mecanismo, as interações com os elementos do campo e as restrições de tamanho do robô. Em seguida, o(s) esboço(s) do layout principal são inseridos em cada part studio do mecanismo, e os componentes individuais são modelados em torno do esboço importado.
Mais informações sobre layout sketches podem ser encontradas em [Boas práticas para Layout Sketch](../../../best-practices/mastersketch-setup.md "Layout Sketch Best Practices Page"){:target="_blank"}.

???+ Example "Exemplo de Main Layout Sketch"
    <figure>
    <img src="\img\learning-course\stage1d\exampleMasterSketch.webp" style="width:60%">
    <figcaption>Exemplo de um main layout sketches. Cada mecanismo possui vários layout sketches que capturam os detalhes importantes. (Crédito da foto: FRC 3647)</figcaption>
    </figure>


### Posicionamento da Origem e Origin Cube
Para utilizar plenamente o top-down design com layout sketches, devemos escolher uma origem unificada para todos os part studios. Utilizar a mesma origem do main layout sketch em todos os part studios e assemblies possui duas vantagens:

1. A origem será sempre um ponto central consistente que você pode referenciar. Isso também ajuda a manter o projeto paramétrico.
2. Para unificar o ponto de origem do CAD do robô com o ponto de origem do software do robô. Ao ter a mesma origem no CAD e no código, o robô pode ser exportado de forma integrada para [AdvantageScope](https://github.com/Mechanical-Advantage/AdvantageScope "AdvantageScope Repository"){:target="_blank"} e as transformações da câmera possam ser medidas com mais facilidade.

!!! Nota
    Embora as definições possam variar de equipe para equipe, a origem de um robô FRC é tipicamente definida como o ***centro da drivebase, no nível do chão***.

Para alcançar isso, usamos o [`Origin Cube` Featurescript](https://cad.onshape.com/documents/321c197a842fc5f1a29e6621/w/fc3cdd5ca7edcd93e02f13cc/e/df3afdbec8d1356c2af15e4b?renderMode=0&uiState=6637caa6ccbcaa36badca03a "Origin Cube Featurescript Document"){:target="_blank"} que gera um cubo transparente de 2" na origem e fornece várias constantes e funções úteis que já foram utilizadas em estágios anteriores.

O Origin Cube será muito útil posteriormente para fazer mates em assemblies, mas por enquanto tudo o que você precisa lembrar é que **o Origin Cube deve ser a primeira feature em todos os part studios**. Você pode ler mais sobre o Origin Cube em… [Boas práticas de assembly](../../../best-practices/assembly-setup.md "Assembly Best Practices Page"){:target="_blank"}.

<br>
