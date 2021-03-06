---
layout: post
title: "Falha no Linux abre portas para ataques via Wi-Fi"
categories: [ News ]
image: 'assets/images/linux-wi-fi.png'
---

Uma vulnerabilidade grave no Linux pode deixar computadores com o sistema operacional vulneráveis a travamentos e explorações remotas a partir do Wi-Fi. O problema está localizado em um driver que permite o funcionamento da rede sem fio a partir de chips da Realtek e pode ser utilizado por criminosos nas proximidades para travar computadores ou ganhar acesso remoto completo a eles.

Não são necessárias interações do usuário, bastando que ele esteja ao alcance de uma rede comprometida. O problema começa em uma funcionalidade de economia de energia chamada Notificação de Ausência, que interrompe temporariamente a conexão em caso de ociosidade, mas mantém os dispositivos ligados para retorno rápido em caso de novo uso. A vulnerabilidade pode ser explorada com a alteração de elementos dessa ligação, causando uma sobrecarga no buffer do Linux.

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

Como os chips da Realtek são bastante populares, a maioria dos computadores deve ser suscetível à brecha, apesar de ser difícil chegar a um número exato. Da mesma forma, como se trata de uma brecha disponível em hardware, não existem distribuições mais ou menos seguras contra a vulnerabilidade.

A falha está presente, pelo menos, desde 2013, e pode ser explorada diretamente, bastando apenas proximidade a um atacante. Nico Waisman, engenheiro de segurança do Github e um dos responsáveis por descobrir a falha, porém, afirma que uma exploração direta da máquina, para obtenção de controle remoto, pode ser complexa, apesar de possível. Estamos falando de ataques direcionados, algo que reduz ainda mais o escopo da vulnerabilidade, mas não a torna menos perigosa.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

Segundo ele, a brecha no buffer permite o controle remoto do computador em teoria, mas Waisman não desenvolveu ainda uma prova de conceito para testar essa ideia na prática. O especialista, por outro lado, confirma a possibilidade de ataques de negação de serviço, travando máquinas completamente e interrompendo trabalhos, algo que pode ser bastante danoso no caso de servidores, data centers ou um ambiente empresarial, por exemplo.

O pesquisador aponta ainda para a existência da brecha, também, nos sistemas de chips da Realtek que foram usados em celulares Android. A plataforma da Google, entretanto, possui proteções adicionais contra sobrecarga de buffer e, por mais que seu hardware esteja supostamente suscetível à exploração, outros sistemas de segurança impedem que essa abertura seja explorada.

Ao mesmo tempo, devido à própria complexidade da brecha, não existem relatos de quea mesma tenha sido aproveitada por cibercriminosos. A equipe de desenvolvimento do Linux propôs, nessa semana, uma solução que já está sendo produzida e deve ser liberada nas próximas semanas, para que os responsáveis pelas diferentes distribuições também possam a implementá-la em suas versões.

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

Via [Ars Technica](https://arstechnica.com/information-technology/2019/10/unpatched-linux-flaw-may-let-attackers-crash-or-compromise-nearby-devices/)
