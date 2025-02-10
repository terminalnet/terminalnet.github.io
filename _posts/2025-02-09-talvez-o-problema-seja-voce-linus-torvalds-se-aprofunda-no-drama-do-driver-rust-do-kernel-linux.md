---
layout: post
title: "'Talvez o problema seja você'... Linus Torvalds se aprofunda no drama do driver Rust do kernel Linux"
categories: [ News ]
image: 'assets/img/1500187704094864457.webp'
---

> Chefe de projeto de código aberto critica 'brigada de mídia social'


Falando sobre mais uma disputa sobre o kernel Linux — dessa vez sobre drivers de dispositivos Rust — o chefe do Linux, Linus Torvalds, atirou no mensageiro.

Em resposta ao apelo do desenvolvedor líder do Asahi Linux, Hector Martin, para que Torvalds "apresente uma resposta confiável" para resolver o impasse do driver de dispositivo, e à defesa de Martin de "envergonhar as mídias sociais" como uma forma de combater a hostilidade dos mantenedores do Linux ao código Rust, Torvalds descartou a abordagem e criticou Martin.

"Que tal você aceitar o fato de que talvez o problema seja você", disse Torvalds, que há vários anos reconheceu sua própria dificuldade com interação diplomática online. "Você acha que sabe mais. Mas o processo atual funciona.

"Tem problemas, mas problemas são um fato da vida. Não existe perfeição.

"No entanto, direi que a brigada nas redes sociais simplesmente faz com que eu não queira ter mais nada a ver com sua abordagem.

"Porque se temos problemas no modelo de desenvolvimento do kernel, então a mídia social com certeza não é a solução. Da mesma forma que com certeza não foi a solução para a política.

"Patches técnicos e discussões são importantes. Brigada nas mídias sociais - não, obrigado."

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

A mensagem relativamente contida de Torvalds — não muito [diferente do aviso omertà descontinuado](https://www.cultofmac.com/news/heres-the-full-text-of-apples-new-app-store-guidelines) da Apple para desenvolvedores, "Se você correr para a imprensa e nos destruir, isso nunca ajuda" — caiu forte. Pouco depois, Martin pediu para ser removido como mantenedor do código Linux upstream que fornece suporte para o hardware compatível com Arm da Apple.

Martin foi acusado de "brigading" - reunir apoio nas mídias sociais - após entrar em conflito com o mantenedor do kernel Christoph Hellwig. A disputa surgiu da oposição de Hellwig a [um patch proposto no mês passado que permitiria que drivers de dispositivos escritos em Rust chamassem a](https://lkml.org/lkml/2025/1/8/803) API DMA principal do kernel, baseada principalmente em C , que aloca e mapeia regiões de memória para acesso direto à memória.

O kernel do Linux foi escrito principalmente em código C, que, junto com C++, se tornou fora de moda nos últimos anos porque linguagens de programação com gerenciamento manual de memória permitem que desenvolvedores cometam erros de segurança de memória. Em alguns casos, isso pode ter consequências sérias de segurança.

Rust, uma linguagem de programação mais nova, é projetada para impor segurança de memória por meio de seu modelo de propriedade, prevenindo muitas vulnerabilidades comuns encontradas em C e C++. Como resultado, ela tem sido amplamente promovida como uma forma de reduzir problemas de segurança de memória no desenvolvimento de software.

O kernel Linux começou a integrar o código Rust em 2022, mas continua sendo uma base de código focada em C. Muitos programadores C que contribuem e mantêm o código deixaram claro que não vão mudar seus hábitos porque o Rust está em ascensão.

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

A tensão entre os desenvolvedores de C e Rust no kernel Linux decorre dos recursos de segurança de memória do Rust serem introduzidos em uma base de código tradicionalmente dominada por C, com alguns mantenedores resistindo à complexidade adicional e ao potencial fardo de manutenção.

A rejeição enfática do patch por Hellwig levou Martin a pedir à equipe do Rust para Linux que "simplesmente fundisse esta série assim que ela fosse revisada e estivesse pronta, ignorando a tentativa aberta de Christoph de sabotar o projeto".

Na terça-feira, Martin postou uma mensagem aconselhando contra se envolver em dramas — apesar de uma postagem apaixonada no Mastodon sobre o assunto, agora removida — porque Torvalds tem a palavra final sobre se o patch do driver do dispositivo será aceito.

"Ou Linus gosta ou não", ele escreveu. "Todo o resto são distrações orquestradas por um subconjunto de mantenedores sabotadores que estão tentando desmoralizá-lo até que você desista, porque eles sabem que estarão no lado perdedor da história mais cedo ou mais tarde. Nenhuma quantidade de sabotagem de antigos mantenedores entrincheirados impedirá o mundo de avançar em direção a linguagens seguras para a memória."

Mas a aversão ao Rust entre os mantenedores do kernel pode desacelerar esse movimento para a comunidade Linux. O destino do patch ainda não foi determinado. ®

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

Fonte: *The Register*


