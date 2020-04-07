---
layout: post
title: "Microsoft apresenta um novo projeto para o kernel do Linux"
categories: [ News ]
image: 'assets/img/Microsoft-Introduces-A-New-Project-For-Linux-Kernel-640x367'
---

Quase dois meses após o lançamento da Plataforma em Nuvem do Azure baseada na IoT, a Microsoft anunciou agora um novo LSM (Linux Security Module) para dispositivos incorporados. O módulo de segurança, chamado IPE (Integrity Policy Enforcement), visa resolver o problema de integridade no kernel do Linux, adicionando um novo recurso de segurança.

# O que é o IPE (Integrity Policy Enforcement)?

IPE é um módulo de segurança Linux que verifica a integridade do código em todo o sistema, restringindo qualquer execução não autorizada de código. Os administradores têm controle total sobre a execução de processos autorizados.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

De acordo com as [ notas oficiais ](https://microsoft.github.io/ipe/), um administrador do sistema também pode criar uma lista de binários com os atributos de verificação correspondentes. Isso ajuda o IPE a executar apenas os binários com atributos verificados e bloquear o código binário malicioso ou alterado.

Se você não sabe, a plataforma IoT do Azure implementa o mesmo kernel do Linux. Portanto, o projeto IPE foi especialmente desenvolvido para sistemas embarcados com finalidades específicas, como dispositivos de firewall de rede em um data center. No entanto, você não pode usar o IPE para computação de uso geral.

# Como o IPE difere de outros módulos de segurança Linux?

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

Embora o kernel do Linux já tenha vários módulos para verificação de integridade, como o IMA. O IPE oferece especificamente verificação em tempo de execução do código binário. A Microsoft alega que o IPE difere de outros LSMs de várias maneiras que fornecem verificação de integridade.

Por exemplo, o IPE não depende dos metadados do sistema de arquivos e dos atributos que o IPE verifica. Além disso, o IPE não implementa nenhum mecanismo para verificar os arquivos de assinatura do IMA. Isso ocorre porque o kernel do Linux já possui módulos para o mesmo como dm-verity.

Os proprietários do sistema podem criar suas próprias políticas para verificações de integridade e utilizar assinaturas internas do dm-verity para autenticar códigos.


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

Para concluir, o novo projeto traz um novo módulo de segurança Linux que outros módulos falham em proteger o sistema contra a execução de código malicioso.


Via [FossBytes](https://fossbytes.com/microsoft-linux-kernel-security-module-ipe/)
