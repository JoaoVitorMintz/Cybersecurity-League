# O que é Networking?

<p style="text-indent: 30px;">
Networking (ou Redes) é qualquer tipo de conexão, sendo mais específicamente para o computador, a conexão entre dois ou mais dispositivos técnológicos, permitindo que possam transferir dados entre si.
</p>

## O que é a Internet?

<p style="text-indent: 30px;">
A internet é o que permite dispositivos diferentes se comunicarem. A internet é constituida de pequenas redes conectadas entre si, sendo essas pequenas redes chamadas de redes privadas (private network) e as redes que conectam as redes privadas chamada de rede pública (public network). Resumindo, se trata da rede de redes porque é formada literalmente por milhares de redes locais conectadas entre si.
</p>

<div>
    <img style="display: block; margin: auto;" alt="InternetLogic" height="570" width="844" src="/Networking/Images/Internet.png">
</div>

## Identificação de dispostivos na Rede:

<p style="text-indent: 30px;">
Para manter a boa comunicação e a organização, os dispositivos devem ser capazes de se identificarem na rede, por isso, assim como seres humanos que são facilmente indentificados pelo nome e pelas digitais, a Rede utiliza dessa lógica, sendo eles respectivamente, o IP (Internet Protocol) e o MAC Address (Media Access Control).
</p>

## O que é o IP?

<p style="text-indent: 30px;">
O IP é uma das formas de ser identificado o host da rede por um período de tempo, sendo esse IP podendo também ser associado à outros dispostivos sem que seja alterado. Um IP address é uma sequencia de números divididas em quatro octetos que, ao serem calculados pelo IP addressing & subnetting, devolve uma informação resumida de cada octeto que identifica o dispositivo. O IP pode ser alterado em cada dispositivo mas não pode estar ativo simultâneamente em mais de um dispositivo que esteja na mesma rede.
</p>

<div>
    <img style="display: block; margin: auto;" alt="IPLogic" height="316" width="754" src="/Networking/Images/IP1.png">
</div>

<p style="text-indent: 30px;">
Os IPs seguem um padrão conhecidos como protocolos que controla a Rede e força os dispositivos a se comunicarem em uma mesma linguagem. Relembrando que os dispositivos podem ser tanto privados quanto públicos, dependendo do tipo, determina o tipo de IP address (public ou private IP address).
</p>

### Exemplo de dispositivos privados e publicos na rede:

<div>
    <img style="display: block; margin: auto;" alt="IPExample" height="316" width="754" src="/Networking/Images/IP2.png">
</div>

<p style="text-indent: 30px;">
Pela imagem, é visível que há dois dispositivos, sendo que cada um possui o IP público e privado. Estes dispositivos utilizam o IP privado para se comunicarem entre si na rede que compartilham (rede local, também conhecida como LAN) enquanto, para qualquer dado enviado pela internet para cada dispositivo, eles utilizam o IP publico (endereço visível na internet, conhecido como WAN). O IP publico é fornecido pela Internet Service Provider (ISP) ou, em português, provedor de internet.
</p>
<p style="text-indent: 30px;">
Até agora, todos esses exemplos de IP citados anteriormente foi relacionado ao esquema conhecido como IPv4, que usa um sistema de numeração de 2^32 IP addresses (cerca de 4.29 bilhões) o que é considerado poucas possibilidades de IP possíveis.
</p>

Para resolver esse problema, surgiu-se um novo esquema de IP addressing chamado IPv6 que possibilitado os seguintes beneficios:
 - Suporta até 2^128 IP addresses (cerca de 340 trilhões-mais).
 - Mais eficiente por seguir uma metodologia nova.

A seguir, uma breve comparação entre o IPv6 e o IPv4:

<div>
    <img style="display: block; margin: auto;" alt="IPExample" height="185" width="730" src="/Networking/Images/IP3.png">
</div>


## O que é o MAC Address:

<p style="text-indent: 30px;">
Cada dispositivo que é capaz de se conectar à rede possui um microchip na placa mãe chamado de Network Interface, sendo atribuído a cada um desses microchips um unico address de fábrica chamado MAC address. Este MAC address é consituido de doze carácteres em hexadecimal, dividio de dois em dois e separados por dois pontos (:). Os primeiros 6 carácteres representam a empresa que criou o Network Interface enquanto os outros 6 representam números únicos de cada interface. Representação na imagem a seguir:
</p>

<div>
    <img style="display: block; margin: auto;" alt="MACLogic" height="390" width="754" src="/Networking/Images/MacAddress.png">
</div>

<p style="text-indent: 30px;">
O MAC address pode ser falsificado ou "spoofed" em um processo chamado spoofing no qual um dispositivo conectado à rede finge se identificar como outro dispositivo usando seu MAC address, o que pode levar à sistemas com um design de segurança mal-feito a quebrarem, já que enxergam o dispositivo como seguro. Lugares como cafeterias e hoteis comumente usam controle de MAC address para configurar o WI-FI chamando-o de "Guest" ou "Public".
</p>

## O que são Redes locais?

<p style="text-indent: 30px;">
São redes simples, que podem ser de apenas dois computadores até que conecta milhões de dispositivos instaladas a pequenos escritórios ou residências. Esses tipos de redes são chamados de redes SOHO e compartilham recursos como: impressoras, documentos, fotos e músicas, entre outros computadores locais.
</p>

<p style="text-indent: 30px;">
</p>