---
layout: post
title: "Lançado o Windows Terminal 0.9 com argumentos de linha de comando e muito mais"
categories: [ News ]
image: 'assets/images/news/Windows-Terminal.jpg'
---

A Microsoft lançou o Windows Terminal v0.9, que adiciona argumentos de linha de comando, criação automática de perfis do PowerShell e uma nova configuração que permite fechar todas as guias sem confirmação.

O Windows Terminal é um programa de console com várias guias que permite iniciar diferentes shells/consoles em diferentes guias. Por exemplo, uma guia pode ser o PowerShell, a outra o prompt de comando padrão do Windows 10 e a terceira um shell bash do WSL, como mostrado abaixo.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

![Windows Terminal](/assets/images/news/windows-terminal.jpg)

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

With the release of Windows Terminal V0.9, Microsoft has introduced a variety of new and helpful features which are outlined below.

# Novos argumentos de linha de comando para abrir guias

O Terminal do Windows pode ser iniciado a partir de um prompt de comando usando o comando `wt`. Com esta versão, agora você pode usar os seguintes argumentos de linha de comando como parte deste comando para abrir novas guias, especificar a pasta que deve ser aberta, abrir em painéis divididos e qual guia deve ser focada.

Esses comandos são:

- `-p`: Especifica o perfil do terminal do Windows que deve ser aberto. Exemplo: Para abrir um console WSL do Ubuntu, digite:
{% highlight bash %}
wt -p "Ubuntu-18.04"
{% endhighlight %}

- `-d`: Especifica a pasta que deve ser usada como o diretório inicial do console. Exemplo: Para abrir o Terminal do Windows e ter seu perfil padrão, abra a pasta `E: \`, digite:
{% highlight bash %}
wt -d e:\
{% endhighlight %}

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

- `new-tab`: Especifica que você deseja abrir uma nova guia. Isso é usado quando você deseja abrir várias guias ao mesmo tempo. Exemplo: Para abrir o perfil padrão do Terminal do Windows e também uma guia WSL do Ubuntu, insira:
{% highlight bash %}
wt; new-tab -p "Ubuntu-18.04"
{% endhighlight %}

![Windows Terminal](/assets/images/news/two-tabs.jpg)

- `split-pane`: Esse comando abrirá uma nova guia, mas em um painel dividido. Exemplo: Para abrir um painel dividido do perfil padrão na pasta `D: \` e o perfil 'cmd' na pasta `E: \`, insira.
{% highlight bash %}
wt -d d:\ ; split-pane -p "cmd" -d e:
{% endhighlight %}

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

![Windows Terminal](/assets/images/news/split-pane.jpg)

- `focus-tab`: Este comando permite especificar qual guia deve ganhar foco quando aberto. Exemplo: Para abrir o perfil padrão e um perfil WSL do Ubuntu, mas tornar a primeira guia focada, você deve inserir este comando.
{% highlight bash %}
wt ; new-tab -p "Ubuntu-18.04"; focus-tab -t0
{% endhighlight %}

Detalhes completos sobre como usar os argumentos da linha de comando podem ser encontrados [aqui](https://github.com/microsoft/terminal/blob/master/doc/user-docs/UsingCommandlineArguments.md).

# Arraste o arquivo para o console para copiar o caminho

Agora você pode arrastar um arquivo para uma janela aberta do console e o caminho para o arquivo será automaticamente colado no console.

![Windows Terminal](/assets/images/news/copy-path-by-dragging-file.jpg)

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

# Configuração de fechar todas as guias automaticamente

Ao fechar o Terminal do Windows, por padrão, você será perguntado se tem certeza se deseja fechar todas as guias.
![Fechar todas as guias](/assets/images/news/close-all-tabs.jpg)

Para remover esta caixa de diálogo de confirmação e fechar automaticamente todas as guias, você pode adicionar a configuração global "`confirmCloseAllTabs`" e defini-la como `false`, como mostrado abaixo.
![Windows Terminal](/assets/images/news/settings.jpg)

# Criar automaticamente perfis do PowerShell

Com esta versão, o Windows Terminal detectará todas as versões do PowerShell instaladas no Windows e criará automaticamente perfis para elas.

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

![Windows Terminal](/assets/images/news/powershell-profiles.jpg)

# Outras correções e melhorias

Abaixo está a lista completa de correções e melhorias no Windows Terminal v0.9.
Outras melhorias

- Acessibilidade: Agora você pode navegar palavra por palavra usando o [Narrator] ou o [NVDA]!
- Agora você pode arrastar e soltar um arquivo no Terminal e o caminho do arquivo será impresso!
- `Ctrl + Ins` e `Shift + Ins` são vinculados por padrão para copiar e colar, respectivamente!
- Agora você pode pressionar `Shift` e clicar para expandir sua seleção!
- As chaves do código VS usadas para ligações de teclas agora são suportadas (por exemplo, "`pgdn`" e "`pagedown`" são válidas)!

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

# Correções de bugs

- Acessibilidade: o terminal não falha quando o Narrator está em execução!
- O terminal não falha quando você fornece uma imagem de plano de fundo ou caminho de ícone inválido!
- Todos os nossos diálogos pop-up agora têm botões arredondados!
- A caixa de pesquisa agora funciona corretamente em alto contraste!
- Algumas ligaduras serão renderizadas mais corretamente!

Via [bleepingcomputer](https://www.bleepingcomputer.com/news/microsoft/windows-terminal-09-released-with-command-line-arguments-and-more/)
