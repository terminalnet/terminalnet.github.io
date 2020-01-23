---
layout: post
title: "Três modos de impedir que o provedor de acesso monitore a sua navegação"
categories: [ News ]
image: 'assets/images/app-security.jpg'
---

> Após o Senado amaericano aprovar a lei que permite aos provedores monitorar os usuários e vender seu histórico de navegação para anunciantes é bom conhecer algumas medidas que ajudam a resguadar o que você faz na Internet.

Se empresas como Google e Facebook podem monitorar a navegação de seus usuários para vender publicidade, então os provedores de acesso internet também podem. Pelo menos no entender dos senadores americanos, que nesta sexta-feira aprovaram a legislação que passa a permitir que os ISPs passem a monitorar e a vender o histórico de navegação de seus clientes para anunciantes. O projeto segue agora para votação na Câmara, onde a maioria republicana é favorável à medida.

Portanto, qualquer pessoa preocupada com sua privacidade, e a do tráfego web dos funcionários da sua empresa, terá de buscar meios de proteger o uso da Internet da coleta de dados, possivelmente também por parte de seu ISP.

Ok, você vai dizer que a maioria dos navegadores possui um modo que permite ao usuário visitar sites sem ser rastreado. Não há histórico ou mesmo cookies. Sim, mas você precisa saber que essa proteção é limitada. Os sites que você visita continuarão a receber o endereço IP do seu roteador e o seu provedor de Internet saberá quem você está visitando. E, se o seu provedor sabe, o governo também pode eventualmente descobrir. Se você usar as ferramentas certas elas podem acrescentar camadas de proteção no seu navegador.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

## 1 - Usar HTTPS em todos os lugares
A extensão do navegador HTTPS Everywhere, da Electronic Frontier Foundation, é uma das primeiras coisas que você deve instalar. Esta extensão requer que todas as conexões do site com o navegador ocorram usando criptografia SSL/TLS. Isso significa que o conteúdo do que você está visualizando será protegido da coleta passiva pelo seu provedor de acesso. Há apenas uma hipótese da extensão não conseguir forçar HTTPS:  quando o site ao qual você estiver se conectando não suportar o protocolo.

A extensão começa a funcionar assim que você a instala. Só não impede, entretanto, que o seu ISP para de ver os locais que você visita. Apenas protege o conteúdo da sua comunicação. Assim, seu ISP saberá que visitou o YouTube, mas não o que você assistiu enquanto estava lá, ou as páginas específicas visitadas.

A HTTPS Everywhere está disponível para Firefox (desktop e Android), Chrome e Opera.

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

## 2 - Usar uma rede privada virtual paga
O próximo passo é se inscrever em um serviço de VPN pago - não um serviço gratuito que colete seus dados e o venda a terceiros para fins de análise ou use anúncios para oferecer suporte a seu serviço gratuito, porque isso seria pior que deixar o seu provedor rastreá-lo. O custo de uma VPN para manter seus dados privados deve girar em torno de US $ 40 a US $ 60 por ano.

Uma VPN é como um túnel criptografado entre você e a Internet. Você se conecta diretamente à sua VPN (uma conexão que seu ISP vai ver) e, em seguida, toda a navegação na Internet passa pelos servidores da VPN e bloqueia o olhar de terceiros. Empresas configurarem suas próprias VPNs usando aplicações especiais de redes. Mas em seu dispositivo pessoal, você terá que optar por algum serviço comercial de VPN.

Algumas empresas de antivírus também oferecem serviços VPN, que podem funcionar como um meio-termo entre soluções gratuitas e as comerciais pagas, uma vez que os usuários conseguem negócios melhores caso também possuam uma licença de antivírus daquela companhia. Além disso, essas soluções de VPN já possuem configurações razoavelmente seguras, então os usuários não precisam se preocupar em configurá-las por conta própria.

Uma vez que você tenha escolhido um fornecedor confiável e configurado uma VPN, defina-a para iniciar automaticamente e passar todo o tráfego da Internet por lá.

Escolher uma VPN é um pouco complicado uma vez que você quer um provedor que colete e armazene uma quantidade mínima de dados sobre a sua navegação. A Freedome VPN promete não registrar seu tráfego e é executada pelo F-Secure, um nome respeitável na segurança da Internet.

Existem tecnologias diferentes de VPN com forças diferentes de criptografia. Por exemplo, o PPTP (Point-to-Point Tunneling Protocol) é rápido, mas muito menos seguro do que outros protocolos como o IPSec ou o OpenVPN, que usam SSL/TLS (Secure Sockets Layer/Transport Layer Security). Além disso, o tipo de algoritmo de criptografia e o tamanho da chave usados também são importantes nas VPNs baseadas em TLS.

Enquanto o OpenVPN suporta muitas combinações de cifras, protocolos de trocas de chaves e algoritmos de hashing, a implementação mais comum oferecida pelos provedores de serviços de VPN para conexões OpenVPN é a criptografia AES com troca de chaves RSA e assinaturas SHA. As configurações recomendadas são criptografia AES-256 com uma chave RSA que tenha pelo menos 2048 bits e a função criptográfica SHA-2 (SHA-256), em vez de SHA-1.

Vale notar que quanto mais forte a criptografia, maior será o impacto na velocidade de conexão. A escolha da tecnologia e da força da criptografia da VPN deve ser feita com base em cada caso, dependendo do tipo de dado que será passado por ela.

Tudo que você tem que fazer é esperar que seu ISP não obstrua ou estrangule seu tráfego sempre que você estiver usando uma VPN paga, ou qualquer outro tipo de proteção.

No mercado corporativo, a maioria das empresas depende muito da utilização da rede privada virtual (VPN) no endpoint, mas há várias formas de se proteger o tráfego da rede IP. A Cisco, por exemplo, acaba de anunciar o primeiro gateway seguro de internet (SIG, na sigla em inglês) em nuvem. Segundo a empresa, o Cisco Umbrella oferece proteção de dados dentro e fora da rede corporativa. Opera como uma plataforma em nuvem que, além de interromper ataques emergentes em todas as entradas e protocolos, também bloqueia o acesso a domínios, URLs e IPs antes que a conexão seja estabelecida ou um arquivo seja baixado.

Isso se torna crítico, porque a maioria das pessoas não trabalha de uma única localização. Muitos estão em casa, cafeterias, escritórios dos clientes, hotéis ou aeroportos e, independentemente de onde trabalhem, os dados precisam estar protegidos. Entre os recursos do Cisco Umbrella estão a visibilidade necessária para proteger o acesso à internet em todos os dispositivos da rede, escritórios e usuários remotos, não só de bisbilhoteiros, quanto de cibercriminosos.

As necessidades de segurança das empresas são diferentes das necessidades da maioria dos usuários, que normalmente só precisam se proteger contra ataques oportunistas que espionam o tráfego - a não ser que estejam preocupados com a vigilância em massa da NSA (Agência Nacional de Segurança dos EUA). Neste caso, uma criptografia muito forte é necessária.

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

## 3 - Ajustar seu DNS
Você também deve querer que a solução de VPN escolhida o proteja contra vazamentos de DNS. O Sistema de Nomes de Domínio é como o seu computador traduz um nome de site legível para humanos, como CIO.com.br, em um endereço numérico de Internet. É como a lista telefônica da Internet.

O problema é que o seu PC é geralmente configurado para usar o DNS do seu ISP, o que significa que seu ISP vê todos os pedidos do seu navegador. As VPN normalmente configuram o seu PC para usar seu DNS, e normalmente há um recurso de proteção contra vazamento de DNS que garante que seu PC não ignore a VPN e use suas configurações de DNS padrão.

No entanto, para ter certeza de que você não está usando o DNS do seu ISP, é uma boa ideia configurar seu PC para usar um provedor de DNS de terceiros, como OpenDNS.

Uma vez configurado, consulte o IPLeak.net e teste vazamentos de DNS (use o teste estendido) para se certificar de que você não está revelando nenhum dado que você não queira revelar.

Outras possibilidadesNo caso de webmail, uma solução possível para manter a privacidade pode ser o uso do add-in MaskMe. Com ele instalado no Firefox ou Chrome você pode clicar no campo para adicionar o seu endereço de e-mail e passar a usar um endereço aleatório e descartável.

A mensagem enviada para o endereço será redirecionada automaticamente para o seu e-mail real... pelo menos até que você diga ao MaskMe para parar com os envios.

![Ask Me](/assets/images/maskme.jpg)

Para manter uma navegação mais privada você pode, ainda, utilizar o navegador anônimo Tor. Esse browser especial sempre roda em modo privado. Ele envia o seu sinal por uma série de servidores para esconder de onde ele realmente vem. É o mais seguro que você consegue ficar na Internet.

<iframe width="1246" height="701" src="https://www.youtube.com/embed/UYFCql7ca_Y" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Por fim, tenha em mente que nenhuma dessas opções é infalível, mas se utilizá-las você terá dado uma série de passos importantes para a sua proteção e a dos funcionários da sua empresa.

Não há qualquer tipo de proteção 100% perfeita, que irá assegurar a sua privacidade por completo. A vulnerabilidade [Heartbleed](http://idgnow.com.br/busca/?sa=&cx=009797713746722025445%3Arcxwsh43g6g+&ie=UTF-8&q=heartbleed) deixou isso bem claro neste ano. Mas você pode "blindar" o seu acesso à Internet, tornando uma brecha de segurança menos provável.

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

Via [CIO](https://cio.com.br/tres-modos-de-impedir-que-o-provedor-de-acesso-monitore-a-sua-navegacao/)
