---
layout: post
title: "Falha grave de segurança do comando sudo no Linux"
categories: [ News ]
image: 'assets/images/sudo.jpg'
---

> Falha ocorreu no comando "sudo" do programa, que permite dar aos usuários privilégios de outro usuário para executar tarefas dentro do sistema, de maneira segura e controlável pelo administrador.

Aqueles acostumados com as linhas de comando do [Linux](https://terminalroot.com.br/linux) ou com alguma plataforma [Unix](http://cse.google.com.br/cse?cx=004473188612396442360:qs2ekmnkweq&q=UNIX), como o [macOS](http://cse.google.com.br/cse?cx=004473188612396442360:qs2ekmnkweq&q=macOS), devem estar familiarizados com o comando `sudo`, que permite executar tarefas com permissões diferentes daquelas que você teria em outro local. Apesar de importante, o comando foi comprometido com uma falha de segurança que permitia o acesso até o nível raiz, possibilitando que invasores executem ações no sudo em qualquer máquina.

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

A vulnerabilidade girou em torno do tratamento do ID dos usuários no sudo. Se digitassem um ID de -1, ou seu equivalente não assinado 4294967295, o comando trataria você como se tivesse acesso à raiz, mesmo registrando o real ID do usuário. Já que estas identidades não existem no banco de dados de senhas, não era exigido nenhum código para logar.

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

<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
	 style="display:inline-block;width:336px;height:280px"
	 data-ad-client="ca-pub-2838251107855362"
	 data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Os desenvolvedores da Linux identificaram e corrigiram o problema. Para os usuários, é recomendado atualizar uma nova versão do sudo (1.8.28 ou a mais nova) para evitar qualquer complicação. É importante lembrar que você não está imediatamente vulnerável, uma vez que qualquer invasor precisa ter controle de linha de comando sobre seu sistema antes que eles possam considerar explorar a falha. Provavelmente, até este ponto, você já estará protegido caso instale a última atualização.

<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-2838251107855362"
     data-ad-slot="9652691879"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>

Via: [Engadget](https://www.engadget.com/2019/10/14/linux-unix-sudo-command-security-flaw/)

<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- Games Root -->
<ins class="adsbygoogle"
	 style="display:inline-block;width:336px;height:50px"
	 data-ad-client="ca-pub-2838251107855362"
	 data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>


