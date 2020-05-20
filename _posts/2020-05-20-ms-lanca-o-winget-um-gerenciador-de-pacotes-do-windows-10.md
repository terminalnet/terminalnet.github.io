---
layout: post
title: "MS lança o winget - um gerenciador de pacotes do Windows 10"
categories: [ News ]
image: 'assets/img/'
---

> Ferramenta foi baseada nos gerenciadores de pacotes de distros Linux como APT, DNF e outros.

Para facilitar a tarefa de instalar alguns aplicativos em suas máquinas, certos sistemas como o Linux além de trazer uma loja de aplicativos, também permitem que as pessoas instalem programas pelo terminal sem ter que acessar o site oficial da aplicação. Agora, quem recebe uma novidade bem parecida em relação a este assunto é o Windows 10, que acaba de ganhar o suporte a um gerenciador de pacotes.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Apesar de se provar bem útil, o novo recurso ainda não acompanha o Windows 10 por padrão e é executado a partir do PowerShell, uma ferramenta que está no sistema operacional da Microsoft para realizar e automatizar tarefas via linha de comando. A seguir, veja como usar o gerenciador de pacotes do Windows 10.

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

# Importante

Esta ferramenta pode ser utilizada na versão estável do Windows 10, mas ainda se encontra em fase de testes e pode apresentar erros com determinados pacotes. Em nossos testes, por exemplo, não foi possível completar a instalação do GIMP, mas outros programas instalaram normalmente.

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

# Como usar o gerenciador de pacotes do Windows 10

O processo para usar o gerenciador de pacotes do Windows não é complicado, entretanto, como foi informado acima, tudo é feito por linha de comando, o que pode não ser amigável para usuários sem muita experiência com o sistema. Confira o passo a passo:

1. Acesse este link do [Windows Package Manager](https://github.com/microsoft/winget-cli/releases) no Github e realize o download de sua última versão no formato App;

2. Abra a pasta em que o arquivo foi baixado e execute-o;
![winget, o lixo](/assets/img/20200519162047.jpg)

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

3. Na janela que surge, clique em “Atualizar”;
![winget, o lixo](/assets/img/20200519162106.jpg)

4. Agora, pelo menu Iniciar, abra o PowerShell;
![winget, a bizarrice](/assets/img/20200519162129.jpg)

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

5. Já para baixar um aplicativo, use o seguinte comando sem as aspas: winget install “nome do aplicativo. Na imagem abaixo, nós mostramos como é feita a instalação do 7-Zip;
![winget, a bosta](/assets/img/20200519162151.jpg)

6. Caso você não tenha configurado o UAC do Windows, pode ser necessário conceder a permissão de administrador na hora de instalar um aplicativo;

7. Agora, pelo menu Iniciar, basta executar o aplicativo baixado.

![winget, alt](/assets/img/20200519162215.jpg)

Além do método mencionado acima para fazer a instalação dos aplicativos, você também pode conferir todos os pacotes disponíveis com o comando: winget show.

![winget, interpertado alt](/assets/img/20200519162241.jpg)

Pronto! Agora, você já sabe como usar o gerenciador de pacotes do Windows para realizar a instalação de aplicativos via linha de comando. Ou seja, agora você terá a facilidade que os usuários Linux sempre tiveram e no momento está muito mais avançado que isso.


