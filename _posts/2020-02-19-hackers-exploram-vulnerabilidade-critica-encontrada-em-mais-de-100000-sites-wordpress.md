---
layout: post
title: "Hackers exploram vulnerabilidade crítica encontrada em mais de 100.000 sites WordPress"
categories: [ News ]
image: 'assets/img/hacked-640x438.jpg'
---

> A falha em plug-in permite que hackers tenham acesso irrestrito aos sites com Wordpress, permitindo alterar seu conteúdo e até mesmo trocar as informações de propriedade, sequestrando assim sites inteiros.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Os hackers vem explorando ativamente uma vulnerabilidade crítica de um plug-in do WordPress que lhes permite limpar completamente todos os bancos de dados de sites e, em alguns casos, assumir o controle total dos sites afetados.

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

A falha está no ThemeGrill Demo Importer instalado em mais de 100.000 sites e foi divulgada no fim de semana passado pela empresa de segurança do site WebARX. Hoje, o WebArx informou que a falha ainda estava sendo explorada, com quase 17.000 ataques bloqueados até o momento. Hanno Böck, jornalista que trabalha no Golem.de, havia visto ataques ativos várias horas antes e relatado no Twitter.
Fonte: Hackers exploram vulnerabilidade crítica encontrada em mais de 100.000 sites WordPress
https://www.oficinadanet.com.br/seguranca/29792-hackers-exploram-vulnerabilidade-critica-encontrada-em-mais-de-100-000-sites-wordpress?utm_source=lec

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

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">There&#39;s currently a severe vuln in a wordpress plugin called &quot;themegrill demo importer&quot; that resetss the whole database. <a href="https://t.co/tT4xiqjna5">https://t.co/tT4xiqjna5</a> It seems attacks are starting: Some of the affected webpages show a wordpress &quot;hello world&quot;-post. /cc <a href="https://twitter.com/webarx_security?ref_src=twsrc%5Etfw">@webarx_security</a></p>&mdash; hanno (@hanno) <a href="https://twitter.com/hanno/status/1229716599227195393?ref_src=twsrc%5Etfw">February 18, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

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

Atualmente, existe um grande problema em um plug-in do wordpress chamado "importador de demonstração de temas" que redefine todo o banco de dados do wordpress", escreveu Böck.

> https://webarxsecurity.com/critical-issue-in-themegrill-demo-importer/ Parece que os ataques estão começando: Algumas das páginas afetadas mostram um post do wordpress com a mensagem "olá mundo". Se você usar este plug-in e sua página da web ainda não foi excluída considere-se com sorte. Remova o plug-in o quanto antes. (REMOVA! Não adianta atualizar o mesmo)

A mensagem "Hello World" é a padrão exibida em sites que usam o WordPress quando o sistema de gerenciamento de conteúdo de código aberto é instalado pela primeira vez ou quando limpo.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Os hackers parecem estar explorando a vulnerabilidade do ThemeGrill na esperança de obter controle administrativo sobre os sites afetados. As aquisições de sites ocorrem apenas quando um site vulnerável tem uma conta com o nome "admin". Nesses casos, depois que os hackers exploram a vulnerabilidade e limpam todos os dados, eles são automaticamente conectados como um usuário com direitos administrativos.

> Na maioria dos casos, a redefinição do banco de dados não chega a ser um problema visto que a maioria das hospedagens possui backup, ou seja, isso não é realmente útil para um hacker, mas se existe um usuário "admin"', o invasor pode assumir tomar conta do site inteiro redefinindo as suas configurações para qualquer conta que não seja a sua.

Portanto, é de se esperar que esses hackers estejam agindo para sequestrar os sites e cobrar um resgate por eles. Isso já aconteceu inclusive com o meu site. Por sorte não era um hacker mal intencionado, ele apenas estava na época alertando a vulnerabilidade de sites com Wordpress que não utilizam o capcha para login. Instalei um dos plug-ins e ele restaurou meu acesso.

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

Mas parece que agora nenhum dos sites afetados está dando essa sorte. Ou eles tem seus sites apagados ou sequestrados.

O ThemeGrill Demo Importador é usado para importar automaticamente outros plugins disponíveis na empresa de desenvolvimento da Web https://themegrill.com/. As estatísticas do WordPress inicialmente disseram que o plugin importador recebeu 200.000 instalações. Mais recentemente, o número foi revisado e caiu para cerca de 100.000, provavelmente porque muitos sites optaram por remover o plug-in.

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

Segundo o WebARX, a vulnerabilidade está ativa há cerca de três anos e reside nas versões 1.3.4 a 1.6.1. A correção está disponível na versão 1.6.2, embora uma versão mais recente (conhecida como 1.6.3) tenha sido disponibilizada nas últimas 12 horas.

O bug decorre de uma falha na autenticação dos usuários antes de permitir que eles executem comandos administrativos privilegiados. Os hackers podem abusar dessa falha enviando solicitações da Web que contêm seqüências de texto especialmente criadas.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Pesquisadores do WebARX descobriram a vulnerabilidade e relataram aos desenvolvedores do ThemeGrill em 2 de fevereiro. O desenvolvedor do plugin não emitiu uma correção até o último domingo.

Os sites que usam o ThemeGrill devem buscar outras soluções e não mais utilizar o plug-in vulnerável.
