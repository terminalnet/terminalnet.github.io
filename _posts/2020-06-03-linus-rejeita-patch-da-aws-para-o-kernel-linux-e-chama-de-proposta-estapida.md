---
layout: post
title: "Linus rejeita patch da AWS para o Kernel Linux e chama de proposta 'estúpida'"
categories: [ News ]
image: 'assets/img/linus.jpg'
---

O chefe do kernel Linux, Linus Torvalds, destruiu um patch dos engenheiros da Amazon Web Services (AWS) que visava mitigar o ataque Snoop às CPUs Intel descobertas por um engenheiro da AWS no início deste ano.

Os chamados ataques de 'Amostragem de dados L1 assistida por Snoop' ou Snoop (CVE-2020-0550) que afetam uma variedade de CPUs Intel Xeon e Core foram divulgados em março.

O engenheiro da AWS Pawel Wieczorkiewicz descobriu uma maneira de vazar dados da memória de uma CPU Intel por meio de seu cache L1D, que fica nos núcleos da CPU, através de 'bus snooping' - a operação de atualização de cache que ocorre quando os dados são modificados no L1D.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Após a divulgação, o engenheiro da AWS Balbir Singh propôs um patch para o kernel do Linux para que os aplicativos pudessem optar por liberar o cache L1D quando uma tarefa fosse desativada.

"Isso impede que os dados sejam bisbilhotados ou vazem por canais laterais após a mudança de contexto da tarefa", explicou Singh em abril. O patch foi fornecido com o kernel Linux versão 5.8.

<!-- MINI ANÚNCIO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- Games Root -->
<ins class="adsbygoogle"
style="display:inline-block;width:730px;height:95px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

O recurso permitiria que os aplicativos, opt-in, chamassem o prctl (2) para liberar o cache L1D de uma tarefa assim que sair da CPU, supondo que o hardware o suporte.

Mas, como observado por Phoronix, Torvalds acredita que o patch permitirá que aplicativos que optarem pelo patch degradem o desempenho da CPU para outros aplicativos.

<!-- RETANGULO LARGO 2 -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:block; text-align:center;"
data-ad-layout="in-article"
data-ad-format="fluid"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="8549252987"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

"Porque me parece que basicamente exporta instruções de liberação de cache para o espaço do usuário e fornece aos processos uma maneira de dizer 'desacelere qualquer outra pessoa com quem eu agende' '", escreveu Torvalds ontem.

"Em outras palavras, pelo que posso dizer, isso pega o louco código da Intel 'buggy CPU's' e causa problemas para a virtualização '(com os quais eu não me importo muito), e o transforma em' qualquer um pode optar por essa doença, e agora afeta até pessoas e CPUs que não precisam dela e configurações onde é completamente inútil '.

"Eu não quero que algum aplicativo funcione 'Oh, eu sou muito especial e bonita e uma flor tão delicada, que quero liberar o L1D em cada alternador de tarefas, independentemente de qual CPU eu esteja, e independentemente de saber se há erratas ou não. Como esse aplicativo não está apenas diminuindo a velocidade, também está diminuindo os outros também. "


<!-- RETANGULO LARGO -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- Informat -->
<ins class="adsbygoogle"
style="display:block"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="2327980059"
data-ad-format="auto"
data-full-width-responsive="true"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

A referência de Torvalds à virtualização foi direcionada à AWS, que, como outros fornecedores de nuvem, vende CPUs virtuais frequentemente com o multithreading simultâneo (SMT) ativado.

Ele continua apontando que, com o SMT ativado, "deve desativar totalmente esse tipo de pseudo-segurança maluca, pois é completamente inútil nessa situação".

"No mínimo_, o SMT ativado deve desativar completamente esse tipo de pseudo-segurança maluca, pois é completamente inútil nessa situação. O agendamento simplesmente não é um ponto de sincronização com o SMT ativado, dizendo" claro, eu lavarei o L1 na troca de contexto "é mais do que estúpido", disse ele.

Em uma discussão com Singh, Torvalds observa que "liberar L1D no SMT" é uma loucura, uma vez que um invasor fica sentado em um núcleo irmão e ataca o conteúdo de L1 *antes* da troca de tarefas ".

Conforme observado pelo The Register, o engenheiro principal da AWS, Benjamin Herrenschmidt, também adicionou algum contexto ao debate sobre o patch em uma discussão com o colaborador do kernel do Red Hat Linux, Ingo Molnar.

Herrenschmidt admitiu que o patch não faz sentido com o SMT, mas pediu aos desenvolvedores do kernel que não "joguem o bebê fora com a água do banho" e contestou o argumento de que o patch era porque a AWS quer vender hiper threads como CPUs virtuais.

"Não necessariamente e nem em todas as circunstâncias", escreveu Herrenschmidt. "Sim, as VMs normalmente têm o SMT ativado. Porém, isso não é direcionado a elas. Um exemplo que foi dado durante as discussões foram os contêineres pertencentes a diferentes usuários", disse ele.

"Outro exemplo seria um processo que lida com dados mais críticos, como informações de pagamento, do que o resto do sistema e deseja se proteger (ou o administrador deseja que esse processo seja protegido) contra possíveis vazamentos de dados para processos menos confiáveis".

"A AWS tem mais do que apenas VMs para alugar :-) Há uma pilha de 'serviços' de nível superior que nossos usuários podem usar e nem todos necessariamente executam em VMs cobradas por vCPU."

Herrenschmidt disse que os patches não estão tentando resolver os problemas que ocorrem dentro de uma VM de cliente executando SMT e nem sobre a proteção de VMs contra outras VMs no mesmo sistema.


<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>


Via: [ZDNET](https://www.zdnet.com/article/linus-torvalds-rejects-stupid-aws-made-linux-patch-for-intel-cpu-snoop-attack/)
