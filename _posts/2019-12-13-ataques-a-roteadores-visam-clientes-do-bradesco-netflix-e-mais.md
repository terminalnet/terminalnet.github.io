---
layout: post
title: "Ataques a roteadores visam clientes do Bradesco, Netflix e mais"
categories: [ News ]
image: 'assets/images/IMG_20180125_121730-1024x576.jpg'
---

Cuidado com o que você preenche e, principalmente, onde insere suas informações nas páginas da web. Segundo relatório divulgado pela empresa de segurança digital Avast nesta semana, foram bloqueadas pela mesma mais de 7.000 tentativas, só em novembro, de ataques de falsificação de solicitação de dados em sites fakes, conhecidos como Cross-Site Request Forgery (CSRF).

De olho nos dados bancários, a tática se aproveita de GhostDNS, que infecta os equipamentos, para conduzir os usuários a páginas falsas, mas com a mesma aparência das reais. Entre os possíveis alvos de ataque, estiveram usuários de roteadores infectados que tentaram acessar os sites do Bradesco, Santander, Pag Seguro, Terra, Uol e Netflix.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

![Ataques](/assets/images/281283.529563-pagina-nao-segura-web.png)

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

## Como funciona

No golpe, os cibercriminosos aproveitam para executar comandos, sem o conhecimento dos usuários, e a modificar, de forma não perceptível, suas configurações de DNS no roteador. Geralmente, o ataque de CSRF ao roteador é iniciado quando o usuário visita um site comprometido com publicidade maliciosa, que é veiculada através redes de anúncios de terceiros no site.

Infectados, os usuários são redirecionados automaticamente para uma das duas páginas de destino. Isso porque o roteador é reconfigurado para usar servidores DNS não autorizados, que redirecionam as vítimas para páginas de phishing que se parecem muito com sites reais.

Para Simona Musilová, analista de ameaças da Avast, os sites “são escolhidos por serem populares e, em geral, exigem que os usuários façam login ou insiram informações de pagamentos. Depois que os usuários fazem isso, suas credenciais de login e informações de pagamentos vão diretamente para os cibercriminosos, dando a eles o acesso à Netflix e às contas bancárias, por exemplo. Além de alertar seus clientes, o problema é que poucos desses serviços evitam que os usuários sejam vítimas, pois os sites de phishing estão fora de seus domínios.”

Por enquanto, as páginas de destino descobertas que hospedavam a variante GhostDNS foram: hxxp[:]//novonovonovo.users.scale.virtualcloud.com[.]br e hxxp[:]//avast.users.scale.virtualcloud.com[.]br.

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

## Ataques de phishing

"Não sabemos ao certo a razão dos criminosos utilizarem 'avast' na segunda URL, mas suspeitamos que isso tenha ocorrido porque bloqueamos a primeira página de destino", comenta Simona Musilová.

Sobre o alcance do ataque, Musilová explica que “enquanto nossas soluções de segurança bloqueiam tentativas de ataques contra os nossos usuários, não há como sabermos se as mais de 200.000 pessoas redirecionadas para as páginas de destino foram protegidas ou não".

O principal problema é que muitos roteadores estão protegidos com credenciais fracas - aquelas que foram entregues junto ao roteador e cujas informações podem ser facilmente encontradas online. Para se ter uma ideia, 43% dos brasileiros nunca acessaram a interface administrativa web de seus roteadores, onde é possível alterar as credenciais de login de fábrica, de acordo com uma pesquisa também feita pela Avast.

No caso do Bradesco, as vítimas inseriram o URL do site em sua barra de endereços e foram redirecionadas para uma versão de phishing do site do banco, onde poderiam "fazer o login" de suas contas e, inclusive, pedindo seu código de autenticação de dois fatores.

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

Assim que o usuário acessava sua "conta falsa", o site malicioso exibia uma mensagem de erro ou simplesmente agia como se estivesse carregando. Quando os usuários faziam o logoff na versão de phishing, eles eram direcionados para o site real do banco, onde poderiam realmente fazer o login da sua conta.

Já a página de phishing da Netflix exigia que a vítima entrasse com seu endereço de e-mail. Depois solicitava as informações de cartão de crédito, pedindo, inclusive, que o usuário fizesse o upload do escaneamento do cartão de crédito.

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

![Ataques](/assets/images/281285.529565-pagina-web-segura.png)

## Como ficar protegido?

Simona Musilová alerta que “os usuários devem ter cuidado ao visitar o site do seu banco ou da sua conta na Netflix, verificando se a página possui um certificado válido, um cadeado na barra URL do navegador. Além disso, os usuários devem atualizar frequentemente o firmware do roteador para a versão mais recente e configurar as credenciais de login do roteador com uma senha forte.”

Caso o usuário acredite que o seu roteador esteja infectado, ele deve fazer o login na interface administrativa web do próprio dispositivo, onde poderá alterar as credenciais de login.

Via [Avast](https://decoded.avast.io/simonamusilova/ghostdns-exploit-kit-strikes-back/)
