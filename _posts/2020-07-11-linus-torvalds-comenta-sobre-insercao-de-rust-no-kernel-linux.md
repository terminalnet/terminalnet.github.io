---
layout: post
title: "Linus Torvalds comenta sobre inserção de Rust no Kernel Linux"
categories: [ News ]
image: 'assets/img/linus-rust.jpg'
---

Os desenvolvedores do kernel parecem ansiosos para debater os méritos de permitir potencialmente o código Rust no kernel do Linux. O próprio Linus Torvalds fez algumas observações iniciais sobre o tópico antes da conferência Linux Plumbers 2020, onde o assunto será discutido detalhadamente.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

No tópico da lista de discussão os comentários anteriores de Greg Kroah-Hartman sobre as perspectivas do Rust para o kernel, foi mencionado que uma das condições buscadas é que ele seria efetivamente desativado por padrão até que haja testes suficientes.

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

Linus Torvalds entrou na conversa com sua própria opinião sobre o assunto. Linus comentou que gostaria que fosse efetivamente ativado por padrão para garantir que haja testes generalizados e não qualquer uso isolado onde os desenvolvedores possam fazer coisas "loucas". Ele não está exigindo que o Rust seja um requisito para o kernel, mas se o compilador Rust for detectado no sistema, o Kconfig habilitará o suporte ao Rust e continuará construindo qualquer código hipotético do kernel do Rust para ver se ele está corretamente construído .

> "Não, faça uma opção de configuração automática "is rust available". Exatamente da mesma maneira que já fazemos as versões do compilador e verificamos a disponibilidade de vários sinalizadores do compilador no momento da configuração."

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

> "O init/Kconfig haverá coisas tipo isso:"

```sh
config LD_IS_LLD
def_bool $(success,$(LD) -v | head -n 1 | grep -q LLD)

and the rust support should be similar. Something like

config RUST_IS_AVAILABLE
def_bool $(success,$(RUST) ..sometest..) 
```

> Porque eu não quero que estejamos na situação em que qualquer novo suporte de Rust nem é testado por compilação por padrão.
> Muito pelo contrário. Eu gostaria que o primeiro driver do Rust fosse introduzido em um formato tão simples que as falhas fossem óbvias e simples.
> A pior situação em que se encontra é que esse (pequeno) grupo de pessoas começa a testar sua situação muito especial e faz coisas ruins e loucas porque "ninguém mais se importa".
> Não obrigado
> 
> [ Linus ]


Pelo menos ele não descartou a idéia de suporte a Rust dentro do kernel. Veremos aonde a direção do suporte à linguagem Rust no kernel Linux leva após o LPC2020.

A virtual Linux Plumbers Conference acontece de 24 a 28 de agosto. O encontro anual dos principais desenvolvedores de kernel do Linux aconteceria em Halifax, no Canadá, até que eles tivessem que abandonar esses planos como resultado do coronavírus, agora fazendo seu primeiro evento de LPC on-line.

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

Via: [Phoronix](https://www.phoronix.com/scan.php?page=news_item&px=Torvalds-Rust-Kernel-K-Build)

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

