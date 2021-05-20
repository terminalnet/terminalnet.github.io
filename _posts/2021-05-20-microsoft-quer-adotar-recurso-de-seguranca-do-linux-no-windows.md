---
layout: post
title: "Microsoft quer adotar recurso de segurança do Linux no Windows"
categories: [ News ]
image: 'assets/img/ms-heart-linux.jpg'
---

A Microsoft abraçou o Linux com o WSL (Windows Subsystem for Linux), mas essa relação pode ficar ainda mais próxima. A companhia planeja levar para o Windows um importante mecanismo de segurança que faz parte dos recursos nativos do kernel Linux há muito tempo: o eBPF (Extended Berkeley Packet Filter).

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

# O que é eBPF?

O BPF (assim mesmo, sem o ‘e’ no começo) foi desenvolvido para filtrar pacotes de redes com base em determinadas regras. Na prática, esse sistema funciona como uma espécie de firewall, com a diferença primordial de que a filtragem é feita dentro de uma máquina virtual baseada em registro.

Mas, com o passar do tempo, o BPF ficou obsoleto, de certa forma. O mecanismo de máquina virtual e seus conjuntos de instruções não aproveitam o potencial de processadores de 64 bits, por exemplo.

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

A versão estendida do BPF, chamada de eBPF, resolveu essa limitação por “conversar” com hardware mais moderno, incluindo chips de 64 bits. Esse e outros avanços permitem ao eBPF ser muito mais do que um firewall virtualizado.

Hoje, essa solução permite que determinadas aplicações sejam executadas pelo kernel de maneira isolada, sem comprometimento da segurança do sistema operacional ou de outras tarefas em execução.

Especialista no assunto, o engenheiro de software Brendan D. Gregg explica em seu blog que o eBPF está para o Linux como o JavaScript está para o HTML. Enquanto este último limita uma página web a conteúdo estático, o JavaScript permite que pequenos programas sejam executados no navegador como se este funcionasse como uma máquina virtual, sem comprometer todo o sistema.

O eBPF segue um princípio semelhante. Com essa solução, aplicações podem acessar a estrutura do kernel, mas sem modificá-lo ou comprometer a sua segurança, pois a execução é feita em um sandbox que dá acesso a um conjunto limitado de recursos do sistema.

Como toda a execução pode ser inspecionada em tempo real, o eBPF é muito usado para monitorar, analisar ou até filtrar tarefas relacionadas às áreas de rede ou segurança — o mecanismo pode ser usado para mitigar ataques DDoS (negação de serviço), por exemplo.

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

# O projeto ebpf-for-windows

Por aí já é possível entender o interesse da Microsoft pelo assunto. A companhia anunciou o projeto ebpf-for-windows com o intuito de criar uma camada de compatibilidade no Windows 10 e no Windows Server 2016 (e versões posteriores) que, na prática, transforma o eBPF em submódulo para esses sistemas operacionais.

Note que o objetivo da companhia não é criar um fork ou uma versão própria do eBPF, mas aproveitar o fato de esse projeto ter código-fonte aberto para implementá-lo em seu ecossistema:

> O projeto ebpf-for-windows visa permitir que desenvolvedores possam utilizar o conjunto de ferramentas e de interfaces de programação de aplicativos (APIs) relacionados ao eBPF em versões disponíveis para Windows. ~Microsoft

Teoricamente, essa abordagem permitirá que recursos de eBPF criados originalmente para Linux possam ser implementados ou adaptados para ambientes Windows com relativa facilidade.

Mas os desenvolvedores interessados em usufruir do ebpf-for-windows precisam ter paciência. O projeto está em fase inicial, portanto, funciona de modo bastante limitado. Os detalhes podem ser conferidos na página do [ebpf-for-windows no GitHub](https://github.com/microsoft/ebpf-for-windows).

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

Via: [Bleeping Computer](https://www.bleepingcomputer.com/news/security/microsofts-new-project-ports-linux-ebpf-to-windows-10-server/) por [Tecnoblog](https://tecnoblog.net/441643/microsoft-quer-levar-ebpf-do-linux-para-windows/)

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

