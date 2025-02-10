---
layout: post
title: "Misturar Rust e C no Linux é comparado ao câncer pelo mantenedor do kernel"
categories: [ News ]
image: 'assets/img/sick-penguin-which-glutted-himself-became-ill-31872907.webp'
---

> Alguns temem que vários idiomas dificultem a manutenção deste superprojeto de código aberto, outros discordam

Os desenvolvedores que tentam adicionar código Rust ao kernel do Linux continuam enfrentando oposição dos mantenedores do kernel, que acreditam que usar várias linguagens é uma complicação indesejada e arriscada.

Preocupações surgiram em setembro passado, quando o engenheiro de software da Microsoft Wedson Almeida Filho se afastou do projeto Rust para Linux , alegando frustração com "bobagens não técnicas" — que é uma maneira de descrever a dificuldade de colaborar com aqueles que têm objetivos diferentes.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

O problema surgiu novamente no mês passado, quando uma abstração proposta para permitir que drivers de dispositivos escritos em Rust chamassem a API DMA principal do kernel baseado principalmente em C encontrou resistência do mantenedor do kernel, Christoph Hellwig.

Especificamente, foi enviado um patch que permitiria que os drivers Rust usassem a dma_alloc_coherent()função C da API DMA para alocar e mapear grandes regiões de memória para acesso direto à memória.

Em uma mensagem para a lista de discussão do kernel Linux, Hellwig escreveu : "Nenhum código Rust em kernel/dma, por favor." Pelo que vale a pena, o patch adicionou código à parte rust/kernel da árvore de código-fonte do Linux, não kernel/dma , até onde sabemos.

Miguel Ojeda, do projeto Rust para Linux, pediu que Hellwig sugerisse uma alternativa.

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

Hellwig respondeu: "Mantenha os wrappers em seu código em vez de tornar a vida dos outros dolorosa", e continuou argumentando que "as interfaces para a API DMA devem permanecer em código C legível e não em ligações estranhas para que [permaneçam] grepáveis ​​e sustentáveis". O desejo de Hellwig parece ser que os drivers não C tenham suas próprias ligações privadas ao código C, e que essas abstrações não sejam mantidas separadamente, nem mesmo na árvore rust/kernel.

Desafiado por Danilo Krummrich, um engenheiro de software da Red Hat envolvido no projeto Rust para Linux, Hellwig deixa claro que não está interessado em lidar com código Rust.

"Não me force a lidar com sua linguagem brilhante do dia", ele escreveu . "Manter projetos multilíngues é uma dor com a qual não tenho interesse em lidar. Se você quer usar algo que não seja C, seja assembly ou Rust, você escreve para interfaces C e lida com a incompatibilidade de impedância você mesmo, no que me diz respeito."

Em resposta, Krummrich explicou que o esforço Rust para Linux está criando código Rust que abstrai as APIs C para todos os drivers Rust e é mantido pelos desenvolvedores Rust. Em outras palavras, o lado C do kernel permanece o mesmo, e os drivers Rust usam abstrações para esse código C, e que essas abstrações são mantidas por uma equipe centralizada em rust/kernel, o que é indiscutivelmente melhor do que drivers tendo suas próprias ligações C individuais.

Mas Hellwig não parece estar interessado em manter abstrações DMA Rust separadamente. Ele explicou que não quer outro mantenedor:

> Se você quiser tornar o Linux impossível de manter devido a uma base de código entre linguagens, faça isso no seu driver para que você tenha que fazer isso em vez de espalhar esse câncer para os subsistemas principais (onde esse câncer é explicitamente uma base de código entre linguagens e não o Rust em si, apenas para escapar da brigada do flameware).

Estudantes de história da tecnologia podem se lembrar que o próprio Linux foi comparado ao câncer pelo ex-CEO da Microsoft, Steve Ballmer, em 2001. "O Linux é um câncer que se apega, em um sentido de propriedade intelectual, a tudo que toca", disse Ballmer , antes do Linux ter se espalhado para o Subsistema Windows para Linux.

Hellwig continuou argumentando que ter outros mantendo a camada de abstração Rust para o alocador coerente DMA como um componente separado não melhora as coisas e dificulta a manutenção do kernel:

> Cada bit adicional que outra linguagem introduz reduz drasticamente a manutenibilidade do kernel como um projeto integrado. A única razão pela qual o Linux conseguiu sobreviver por tanto tempo é por não ter limites internos, e adicionar outra linguagem quebra isso completamente. Você pode não gostar da minha resposta, mas farei tudo o que puder para impedir isso. NÃO é porque eu odeio Rust. Embora não seja minha linguagem favorita, é definitivamente uma das melhores novas e eu encorajo as pessoas a usá-la para novos projetos onde ela se encaixa. Não quero que ela chegue perto de uma enorme base de código C que eu preciso manter.

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

Hector Martin, líder de projeto da Ashai Linux, compartilhou sua crença de que as observações de Hellwig constituem uma violação do Código de Conduta, mas duvida que qualquer ação disciplinar seja tomada. O Register perguntou a Martin se ele pretende registrar uma reclamação do Código de Conduta, e não obtivemos resposta.

Martin argumenta que os desenvolvedores do Rust para Linux deveriam ignorar as preocupações de Hellwig e enviar seu patch para aprovação do chefe do kernel, Linus Torvalds:

"Se Linus não der uma resposta autoritativa a este tópico, Miguel e o pessoal do Rust devem simplesmente mesclar esta série assim que for revisada e estiver pronta, ignorando a tentativa aberta de Christoph de sabotar o projeto. Se Linus [aceitar a solicitação de pull], o que Christoph disser não importa. Se Linus não [aceitar], o projeto [Rust para Linux] estará essencialmente morto até que Linus ou Christoph façam um movimento. Todo o resto é rodeios."


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

Via: ®

