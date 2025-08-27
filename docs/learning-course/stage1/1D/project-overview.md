# 1D: Metodologia de Design - Simples Swerve Drivebase

## Visão Geral do Projeto
Nesta etapa, você estará projetando uma base móvel do tipo swerve drive. Uma base móvel (drivebase) é a plataforma sobre a qual todos os outros mecanismos são projetados e fixados. Com o surgimento de módulos swerve COTS confiáveis, projetar uma base móvel swerve tornou-se significativamente mais fácil e se consolidou como o sistema de tração competitiva mais utilizado no FRC.

Uma base swerve drive é composta por quatro swerve modules. Cada módulo possui dois motores: um para girar a roda e outro para direcioná-la. Isso permite que o robô se desloque em qualquer direção de forma independente da rotação do próprio robô. Neste projeto, utilizaremos [SDS MK4i modules](https://www.swervedrivespecialties.com/products/mk4i-swerve-module "SDS MK4i Product Page"){:target="_blank"}. Existem muitas outras opções COTS disponíveis, cada uma com suas próprias vantagens e desvantagens.

<!-- Você pode aprender mais sobre drivetrains em [Design Handbook](/design-handbook/mechanisms/drivetrain/) . -->

<figure>
    <img src="\img\learning-course\stage1d\SwerveBase\DriveAssy.webp" style="width:80%">
    <figcaption>Projeto do swerve drivebase Stage 1D.</figcaption>
</figure>

Como nos exercícios anteriores, o projeto finalizado está disponível como referência. Se precisar de ajuda, sinta-se à vontade para perguntar no [the Discord](https://discord.gg/qdx7pdZKx4 "DDS Discord Invite"){:target="_blank"}!

<center markdown>[1D Drivebase Reference](https://cad.onshape.com/documents/6c6044229091a87cf359270b/w/ed9648f0c04c639a2561615a/e/67a7ed0c6038787281325a51 "1D Drivebase Reference Onshape Document"){:target="_blank" .md-button .md-button--primary }</center>

### Estrutura da Drivebase 

Como foi apresentado no Stage 1A, as estruturas de robôs são tipicamente construídas com tubos de alumínio em formato de caixa (aluminum box tubing). A base móvel não é exceção. A maioria das equipes opta por projetar seus tubos de caixa com um padrão de espaçamento padrão de 0,5" e furos de 0,196" de diâmetro. Isso possibilita modularidade e permite a fácil integração de muitos componentes COTS, como gussets.

As extrusões de tubos de caixa podem ser adquiridas na maioria dos fornecedores de metal, mas muitos fornecedores de FRC, incluindo [WCP](https://wcproducts.com/collections/systems-structure/products/punched-tubing){:target="_blank"}, [TTB](https://www.thethriftybot.com/products/thrifty-box-extrusion){:target="_blank"}, and [REV](https://www.revrobotics.com/MAXTube/){:target="_blank"} vendem tubos de caixa com padrões de furos pré-perfurados, o que pode reduzir significativamente o tempo de fabricação e os requisitos de equipamentos.

<br>
