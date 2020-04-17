---
layout: post
title: "Canonical muda o kernel do Ubuntu no Amazon AWS para modelo contínuo"
categories: [ News ]
image: 'assets/img/ubuntu-aws.png'
---

Em uma nova postagem no blog, Francis Ginther, gerente de engenharia da Canonical (fabricante do Ubuntu), anunciou a adoção de um modelo de kernel contínuo no Ubuntu 18.04 LTS Amazon Machine Image (AMI). Caso você não saiba, a Canonical já usa esse modelo em outros ambientes em nuvem para fornecer as mais recentes correções de bugs e melhorias de desempenho.

O kernel contínuo fará com que o kernel linux-aws padrão, que é baseado no 4.15, mude para um novo kernel baseado no 5.3 da versão intermediária. Como a próxima versão de longo prazo, o Ubuntu 20.04, deve ser lançada em 23 de abril, o Ubuntu 19.10 é atualmente uma versão intermediária com um kernel baseado em 5.3.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>


# Como obter um novo kernel?

A partir de agora, se você atualizar o kernel, passará para o kernel 5.3, atualmente disponível para visualização como o kernel linux-aws-edge. Portanto, você deve usá-lo em suas implantações que não são de produção.

Agora, para obter o kernel contínuo, você pode atualizar seu pacote ou iniciar a AMI mais recente que incluirá um kernel mais recente. Aqui, demonstrarei como instalar kernels rolantes no Ubuntu AWS existente.

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

Para começar, primeiro faça login na sua instância remota do Ubuntu na AWS e verifique a versão do kernel usando o comando:

`uname -r`

Em seguida, atualize os pacotes, instale o kernel linux-aws-edge e reinicie a instância do Ubuntu:

```sh
sudo apt update
sudo apt install -y linux-aws-edge
sudo reboot
```

Por fim, você pode verificar a versão do kernel que, esperançosamente, mostrará a v5.3 (se sua instalação for concluída com êxito):

`uname -r`

E se você não quiser ter um núcleo rotativo?

Se você deseja criar uma nova instância ou atualizar pacotes enquanto adere ao kernel 4.15, pode executar o seguinte comando:

```sh
sudo apt update
sudo apt install linux-aws-lts-18.04
```


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

Via: [FOSSBYTES](https://fossbytes.com/ubuntu-on-aws-rolling-kernel-model/)

