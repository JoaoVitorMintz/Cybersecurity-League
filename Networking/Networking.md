# O que é Networking?

Networking (ou Redes) é qualquer tipo de conexão, sendo mais específicamente para o computador, a conexão entre dois ou mais dispositivos técnológicos, permitindo que possam transferir dados entre si.


## O que é a Internet?

A internet é o que permite dispositivos diferentes se comunicarem. A internet é constituida de pequenas redes conectadas entre si, sendo essas pequenas redes chamadas de redes privadas (private network) e as redes que conectam as redes privadas chamada de rede pública (public network). Resumindo, se trata da rede de redes porque é formada literalmente por milhares de redes locais conectadas entre si.


<div>
    <img style="display: block; margin: auto;" alt="InternetLogic" height="570" width="844" src="/Networking/Images/Internet.png">
</div>

## Identificação de dispostivos na Rede:

Para manter a boa comunicação e a organização, os dispositivos devem ser capazes de se identificarem na rede, por isso, assim como seres humanos que são facilmente indentificados pelo nome e pelas digitais, a Rede utiliza dessa lógica, sendo eles respectivamente, o IP (Internet Protocol) e o MAC Address (Media Access Control).


## O que é o IP?

O IP é uma das formas de ser identificado o host da rede por um período de tempo, sendo esse IP podendo também ser associado à outros dispostivos sem que seja alterado. Um IP address é uma sequencia de números divididas em quatro octetos que, ao serem calculados pelo IP addressing & subnetting, devolve uma informação resumida de cada octeto que identifica o dispositivo. O IP pode ser alterado em cada dispositivo mas não pode estar ativo simultâneamente em mais de um dispositivo que esteja na mesma rede.


<div>
    <img style="display: block; margin: auto;" alt="IPLogic" height="316" width="754" src="/Networking/Images/IP1.png">
</div>


Os IPs seguem um padrão conhecidos como protocolos que controla a Rede e força os dispositivos a se comunicarem em uma mesma linguagem. Relembrando que os dispositivos podem ser tanto privados quanto públicos, dependendo do tipo, determina o tipo de IP address (public ou private IP address).


### Exemplo de dispositivos privados e publicos na rede:

<div>
    <img style="display: block; margin: auto;" alt="IPExample" height="316" width="754" src="/Networking/Images/IP2.png">
</div>


Pela imagem, é visível que há dois dispositivos, sendo que cada um possui o IP público e privado. Estes dispositivos utilizam o IP privado para se comunicarem entre si na rede que compartilham (rede local, também conhecida como LAN) enquanto, para qualquer dado enviado pela internet para cada dispositivo, eles utilizam o IP publico (endereço visível na internet, conhecido como WAN). O IP publico é fornecido pela Internet Service Provider (ISP) ou, em português, provedor de internet.

Até agora, todos esses exemplos de IP citados anteriormente foi relacionado ao esquema conhecido como IPv4, que usa um sistema de numeração de 2^32 IP addresses (cerca de 4.29 bilhões) o que é considerado poucas possibilidades de IP possíveis.


Para resolver esse problema, surgiu-se um novo esquema de IP addressing chamado IPv6 que possibilitado os seguintes beneficios:
 - Suporta até 2^128 IP addresses (cerca de 340 trilhões-mais).
 - Mais eficiente por seguir uma metodologia nova.

A seguir, uma breve comparação entre o IPv6 e o IPv4:

<div>
    <img style="display: block; margin: auto;" alt="IPExample" height="185" width="730" src="/Networking/Images/IP3.png">
</div>


## O que é o MAC Address:


Cada dispositivo que é capaz de se conectar à rede possui um microchip na placa mãe chamado de Network Interface, sendo atribuído a cada um desses microchips um unico address de fábrica chamado MAC address. Este MAC address é consituido de doze carácteres em hexadecimal, dividio de dois em dois e separados por dois pontos ( : ). Os primeiros 6 carácteres representam a empresa que criou o Network Interface enquanto os outros 6 representam números únicos de cada interface. Representação na imagem a seguir:


<div>
    <img style="display: block; margin: auto;" alt="MACLogic" height="390" width="754" src="/Networking/Images/MacAddress.png">
</div>

O MAC address pode ser falsificado ou "spoofed" em um processo chamado spoofing no qual um dispositivo conectado à rede finge se identificar como outro dispositivo usando seu MAC address, o que pode levar à sistemas com um design de segurança mal-feito a quebrarem, já que enxergam o dispositivo como seguro. Lugares como cafeterias e hoteis comumente usam controle de MAC address para configurar o WI-FI chamando-o de "Guest" ou "Public".

## O que são Redes locais?

São redes simples, que podem ser de apenas dois computadores até que conecta milhões de dispositivos instaladas a pequenos escritórios ou residências. Esses tipos de redes são chamados de redes SOHO e compartilham recursos como: impressoras, documentos, fotos e músicas, entre outros computadores locais.

## Tipos de dados:
 - Dados Voluntários: Todo tipo de dado que um usuário transmite, por exemplo, por meio das redes sociais ao compartilhar video, imagem ou responder pesquisas, pesquisar certas informações e etc.
 - Dados Inferidos: Dados retirados, por exemplo, de cartão de crédito que armazena informação como tipo de lugar que frequenta, score de crédito, preferências e etc, pode ter base na análise de dados voluntários e observados, porém, não necessáriamente foi fornecido por boa vontade do usuário.
 - Dados Observados: Dados obtidos a partir das ações dos indivíduos como localização enquanto usa o smartphone e etc.

## Métodos comuns de transmissão de dados:

Todos os dados, após serem transformados em uma série de bits, podem ser transmitidos de algumas formas, sendo as mais comuns: Sinais elétricos (Transmissão obtidida pela representação dos dados como pulsos elétricos em fiosd e cobre), Sinais ópticos (Transmissão obtida ple aconversão dos sinais elétricos em pulsos de luz) e Sinais sem fio (Transmissão obtida pelo uso de infravermelhos, micro-ondas ou ondas de rádio pelo ar). Na maioria das vezes, as transmissões são feitas por fios de cobre ou sem fio (WI-FI), sendo os cabos de fibra óticas mais confiáveis para sinais em longas distância (Internet).

## O que é a Largura de Banda?

Meio físico pode suportar a transferência de bits em velocidades diferentes, sendo a largura de banda a capacidade de um meio de transportar dados, medindo a quantidade de dados que podem fluir de um lugar para outro em determinado tempo. Exemplo: Kbps ~ Milhares de bits por segundo; Mbps ~ Milhões de bits por segundo e etc.

## O que é a Taxa de transferência?

Taxa de transferência, assim como a largura de banda, é a medida de transferência de bits através do meio físico durante um determinado período, entretanto, diversos fatores fazem com que a taxa de transferência não corresponda à largura de banda pelo fato da largura de banda ser um valor teóricamente alcançavel, porém, a taxa de transferência se trata justamente dos valores "reais", sendo exemplos de fatores que influenciam:

 - A quantidade de dados enviados e recebidos pela conexão
 - Os tipos de dados transmitidos
 - A latência criada pelo número de de dispositivos encontrados entre a origem e o destino

A **latência** anteriormente citada se refere ao tempo necessário apra os dados viajarem de um ponto ao outro, incluindo os atrasos.

Taxa de transferência não leva em consideração a validade ou a utilidade dos bits transmitidos/recebidos. Muitas mensagens recebidas pela rede não são destinadas a aplicativos específicos de usuário como mensagens de controle de rede que regulam o tráfego e corrigem erros.

Em uma inter-rede (rede com vários segmentos), a traxa de transferência não pode ser mais rápida do que o link mais lento do caminho entre o dispositivo emissor e o dispositivo receptor. Mesmo que todos os segmentos tenham banda alta, basta um segmento com largura de banda baixa no caminho para causar lentidão no rendimento da rede inteira.

## O que é o Throughput? 

É a quantidade de dados enviados/recebidos em uma conexão, considerandos os possíveis delays no envio/recebimento. Thourhput é visto normalmente como velocidade de download (recebimento) e velocidade de upload (envio).
