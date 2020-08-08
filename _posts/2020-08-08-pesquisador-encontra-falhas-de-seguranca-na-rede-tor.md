---
layout: post
title: "Pesquisador encontra falhas de segurança na rede Tor"
categories: [ News ]
image: 'assets/img/tor.jpg'
---

> Segundo o Dr. Neal Krawetz, vulnerabilidades podem banir acesso de usuários à rede Tor; pesquisador vai divulgar outros três problemas de segurança.

Apesar de o projeto Tor garantir a proteção de dados e o anonimato dos usuários enquanto navega pela internet — permitindo o acesso à deep web, por exemplo — o navegador alternativo tem sido acusado de apresentar grandes falhas de segurança. Em julho, o pesquisador de segurança Neal Krawetz divulgou duas ocorrências zero-day (graves vulnerabilidades desconhecidas do desenvolvedor) no sistema Tor, e pretende anunciar mais três erros em breve.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

O primeiro erro foi reportado no dia 23 de julho. O Dr. Neal Krawetz publicou que empresas e provedores de internet poderiam impedir que os usuários se conectassem à rede Tor, examinando as conexões de rede em busca de "uma assinatura de pacote distinta", recurso exclusivo do software. O banimento do tráfego pelo Tor poderia ser realizado por regimes opressores que restringem o acesso à internet, já que o navegador permite que usuários tenham acesso a 'sites proibidos' pelos seus países.

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

A segunda falha descoberta aponta que operadores de rede podem reconhecer o tráfego do Tor mesmo por acessos indiretos — conexões com as pontes Tor. Ou seja, o rastreamento de pacotes TCP não só permitiria a identificação de acessos diretos pela rede Tor (primeiro zero-day), como também detectaria uma via alternativa de acesso encontrada pelos "mais espertos".

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

"Com minhas duas publicações, você agora tem tudo o que precisa para aplicar a política [de bloquear o Tor em uma rede] com um pacote de inspeção de sistema em tempo real. Você pode impedir o acesso de todos os usuários à rede Tor, estejam eles conectados de forma direta ou indireta", aponta Krawetz.

As publicações do Dr. Neal Krawetz são resultantes da falta de correções de bugs anteriores — descobertos pelo próprio pesquisador —, fazendo com que Neal abandonasse o projeto Tor. Krawetz já havia reportado:

+  um bug que permite que sites detectem as impressões digitais de usuários do Tor por meio de uma estimativa da largura de sua barra de rolagem;
+  um bug que expõe os servidores de ponte Tor à redes concorrentes por meio do roteamento Onion;
+  um bug que permite a detecção da SSL — criptografia de dados entre duas aplicações — utilizada nos servidores Tor.

# Tor se posiciona

Pelo Twitter, a companhia disse estar ciente dos possíveis métodos de identificações relatados pelo pesquisador, mas afirmou que os banimentos não podem ser realizados em escala. 

"Pessoas têm nos questionado sobre uma série de bugs que estão sendo veiculados e classificados incorretamente como zero-days. Sempre que formos notificados de bugs com alto risco de segurança, nós iremos, como sempre, abordar esses problemas e formalizar respostas para que vocês saibam o que está acontecendo", diz o tuíte

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

>     People have asked us about a series of bugs that are being publicized and incorrectly labeled as 0-days. Whenever we are notified of high-risk security bugs, we will, as always, address these issues and release formal responses so you know what's happening. [ pic.twitter.com/2KcVYPv02x ](https://t.co/2KcVYPv02x)
    — The Tor Project (@torproject) [July 30, 2020](https://twitter.com/torproject/status/1288955073322602496?ref_src=twsrc%5Etfw)


A companhia informou que estava ciente sobre a falha referente à identificação do sistema do usuário pela largura da barra de rolagem, mas a não comunicação entre o sistema operacional do usuário com o navegador Tor pode resultar em crashes de alguns sites. A Tor afirmou já estar trabalhando para eliminar essa violação de privacidade, mas como a empresa não quer comprometer o acesso a páginas da web durante esse intervalo, o reparo pode levar tempo.

<a href="https://terminalroot.com.br/newsletter" target="_blank" class="btn btn-danger btn-block">Receba novidades por e-mail!</a> 

Quanto à identificação da impressão digital de dispositivo baseadas nos protocolos de tráfego SSL e TLP, a Tor afirmou que há uma equipe de segurança atuando no problema e tem investido para a solução do caso.

O post abordou ainda o erro que permite operadores de rede reconhecerem o tráfego do Tor por acessos indiretos ou indiretos. Segundo a companhia, além de o método não ser totalmente eficaz, dificilmente pode ser usado em larga escala, dado o alto custo operacional.

# Assista à um vídeo sobre Tor Browser 

<iframe width="1234" height="694" src="https://www.youtube.com/embed/UYFCql7ca_Y" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Via: [ZDNet](https://www.zdnet.com/article/multiple-tor-security-issues-disclosed-more-to-come/) por [Olhar Digital](https://olhardigital.com.br/noticia/pesquisador-encontra-falhas-de-seguranca-na-rede-tor/104490)
