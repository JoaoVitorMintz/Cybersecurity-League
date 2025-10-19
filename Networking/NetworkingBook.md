**Referência:** KUROSE, J. F.; ROSS, K. W. Redes de computadores e a internet: uma abordagem top-down. 3. ed. São Paulo, SP: Pearson, 2005. E-book. Disponível em: https://plataforma.bvirtual.com.br. Acesso em: 09 out 2025.

## O que são comutadores de pacotes?

Equipamentos interconectados indiretamente por equipamentos intermediários conhecidos como **comutadores de pacotes** (encaminha a informação que está chegando em um de seus enlaces de comunicação de entrada para um de seus enlaces de comunicação de saída). Blocos de informação são comumente chamados de **pacote**. Há diversos tipos de comutadores de pacotes, sendo os dois mais comum na internet: **roteadores** e **comutadores de camada de enlace (switches)**. Esses comutadores encaminham pacotes a seus destinos finais.

A sequência de enlaces de comunicação e comutadores de pacotes que percorre desde o sistema final remetente até o sistema final receptor é conhecido como **rota** através da rede. A internet não provem de um caminho dedicado entre sistemas finais comunicantes mas utiliza de uma técnica chamada **comutação de pacotes** que permite que diversos sistemas finais comunicantes compartilhem ao mesmo tempo um caminho ou partes dele.

---

## O que são protocolos?

Os sistemas finais, os comutadores de pacotes e outras peças da Internet executam **protocolos** que controlam o envio e o recebimento de informação dentro da Internet. O **TCP** (Transmission Control Protocol) e o **IP** (Internet Protocol) São dois dos protocolos mais importantes da internet. O protocolo IP especifica o formado dos pacotes que são enviados e recebido entre roteadores e sistemas finais. Os principais protocolos da internet são conhecidos coletivamente como **TCP/IP**.

## Protocolo como analogia humana:
<div>
    <img style="display: block; margin: auto;" alt="ProtocolExample" height="640" width="950" src="/Networking/Images/Protocol.png">
</div>

Pela imagem, é visivel que o protocolo humano (boas maneiras) ordena que iniciemos uma comunicação primeiramente com um "oi" e um "oi" como resposta indicando que pode-se prosseguir na interação. No caso de uma resposta diferente do "oi" exemplificado pode indicar portanto incapacidade de comunicação. Após isso, é de protocolo humano requisitar algo, que no caso do exemplo, seria as horas. Esse exemplo mostra que deve-se garantir o protocolo para que as respostas batam e a interação seja realizada, sendo portanto válido também para redes para que entidades comunicantes executem o mesmo protocolo para que uma tarefa seja realizada.

## Em relação à protocolos de rede:

O protocolo de rede trabalha com a comunicação de hardware ou software de algum equipamento (computador, roteador ou outro equipamento habilitado para rede). **Protocolos implementados em hardware** nas placas de inteface de rede de dois computadores conectados fisicamente controlam o fluxo de bits do barramento entre as duas placas de interface de rede; **protocolos de controle** de congestionamento em sistemas finais controlam a taxa com que os pacotes são transmitidos entre a origem e o destino; **protocolos de roteadores** determinam o caminho de um pacote da fonte ao destino.

Um exemplo de protocolo de rede pode ser a requisição a um servidor Web ao digitar a URL de uma página Web no browser. Primeiramente o computador envia uma mensagem de requisição de conexão ao servidor Web e aguarda a resposta. Ao receber essa requisição, o servor retorna uma mensagem de resposta de conexão, sabendo que está tudo certo para requisitar o documento da Web, o computador envia o nome da página Web que quer buscar naquele servidor com uma mensagem GET e, por fim, o servidor retorna a página Web (arquivo) para o computador. Sendo portanto, definido o protocolo como: 

"*Um protocolo define o formato e a ordem das mensagens trocadas entre duas ou mais entidades comunicantes, bem como as ações realizadas na transmissão e/ou no recebimento de uma mensagem ou outro evento*" (F. KUROSE, James, 2005, p.7)

## O que são, de fato, os RFCs:

RFCs são documentos que definem padrões desenvolvidos pela IETF para protocolos. Inicialmente, os RFCs recebiam solicitações de comentários para resolver problemas de arquitetura que a a percursora da internet enfrentava, sendo um tipo de documentação muito técnica e detalhados. Definem protocolos como TCP, IP, HTTP e SMTP (Simple Mail Transfer Protocol). Existem mais de 3500 RFCs. Há também outros tipos de padrões especificados por outros órgãos como o IEEE que define, por exemplo, o IEEE 802 LAN/MAN que especifica os padrões de Ethernet e Wi-Fi sem fio.

---

## Exemplificando e explicando intranets:

A internet é um tipo de rede pública (rede global de redes) e rede privada são comumentes usadas em redes corporativas ou governamentais, cujos hospedeiros não podem trocar mensagens com hospedeiros que estão fora da rede privada (a menos que as mensagens passem por dispositivos denominados **firewall** que restringe o fluxo de mmensagens para dentro e para fora da rede). Essas redes privadas são frequentemente denominadas **intranets** por usarem o mesmo tipo de hospedeiros, roteadores, elaces e protocolos da inetnet pública.

---

## Sistemas finais, clientes e servidores:

Computadores conectados à internet são usualmente denominados **sistemas finais** pois estão na periferia da internet. Sistemas finais são, de forma geral: Commputadores de mesa, servidores, computadores móveis e, atualmente, equipamentos eletroeletrônicos como TVs, eletrodomésticos entre outro.

Sistemas finais também são denominados de **hosts** por hospedarem programas de aplicações como browser da Web, programa de servidor Web, leitor de e-mail e etc. Sistemas finais são ainda subdivididos em duas categorias: **clientes** e **servidores**. Normalmente, clientes são PCs de mesa ou móveis enquanto servidores costumam ser ser máquinas mais poderosas que armazenam e distribuem páginas Web, vídeo em tempo real e etc.

Um **programa cliente** é um programa que funciona em um sistema final, que solicita um serviço de um **programa servidor**, que funciona em um outro sistema final, sendo conhecido como modelo cliente-servidor. Aplicações cliente-servidor de Internet são, por definição, **aplicações distribuídas**, interagindo por envio de mensagens um para o outro pela Internet. Os roteadores, enlaces e outros componentes da Internet funcionam de forma similar a uma caixa-preta que transfere mensagem entre componentes distribuídos, comunicantes, de uma aplicação de Internet (Não confundir com logs que são os registros de eventos como conexões, erros e etc. que podem ajudar a entender comportamente interno dessa "caixa-preta").

Nem todos as aplicações da Internet atual trabalham com programas puramente clientes que interagem com programas puramente servidores. Exemplo: Aplicações P2P que funciona como um programa cliente e também como um programa servidor. Funciona como cliente para requisição de um arquivo de outro par e o programa funciona como um servidor quando envia um arquivo para outro par (sendo par a máquina de um usuário).

---

## Serviço não orientado para conexão (UDP) x serviço orientado para conexão (TCP):

 - **Serviço orientado para conexão (TCP):** O programa cliente e o programa servidor enviam pacotes entre si antes de enviar dados reais para estabelecer uma comunicação. Esse processo é chamado de apresentação e, ao ser concluído esse procedimento, é estabelecido uma conexão entre esses dois sistemas finais. Nesse tipo de conexão, apenas os sistemas finais sabem dessa conexão (comutadores de pacotes ficam alheios a ela). Este serviço vêm conjugados com diversos outros serviços, inclusive transferência de dados confiável (uma aplicação pode confiar que a conexão entregará todos os seus dados sem erro e na ordem certa), controle de fluxo (garante que nenhum dos lados de uma conexão sobrecarregue o outro enviando muitos pacotes rapidamente) e controle de congestionamento (ajuda evitar que a internet trave já que, os comutadores que armazenam em seus buffers os pacotes enviados, podem transbordar e perder pacotes. Portanto, internet forla que sistemas finais a reduzirem a velocidade em que enviam pacotes à rede durante períodos de congestionamento). O TCP vem de Transmission Control Protocol engloba os outros serviços anteriores mas também provê uma **abstração de corrente de bytes**, entregando uma corrente de bytes do remetente ao receptor.
  
  
 - **Serviço não orientado para conexão (UDP):** Não há apresentação mútua neste tipo de serviço, quando um lado de uma aplicação envia pacotes para o outro, o programa remetente apenas o envia, sem estabelecer a conexão de fato. Sem a apresentação, os dados podem ser entregues mais rápidos, sendo portanto um bom serviço para aplicações simples, porém, não há transferência confiável de dado, nem controle de fluxo, nem controle de congestionamento. O UDP vem de User Datagram Protocol.

## Onde cada tipo de serviço é usado?

Maioria das aplicações conhecidas da internet utilizam TCP, sendo elas (exemplos): Telnet, SMTP, FTP e HTTP. Entretanto, a UDP é comumente usado para aplicações de multimídia como telefone por internet e videoconferência.

---

## Núcleo da rede, comutação de circuitos e comutação de pacotes:

O **núcleo da rede** refere-se à malha de roteadores que interconecta os sistemas finais da Internet. Existem duas abordagens principais para a transmissão de dados nesse núcleo: a **comutação de circuitos** e a **comutação de pacotes**.

Na **comutação de circuitos**, todos os recursos necessários (como buffers e taxa de transmissão dos enlaces) são **reservados de forma dedicada** durante toda a sessão de comunicação. Isso significa que, antes de a comunicação começar, é estabelecido um **caminho fixo e exclusivo** entre origem e destino, garantindo uma taxa de transmissão constante. Essa abordagem é típica das redes telefônicas tradicionais, onde o circuito é estabelecido antes da conversa e mantido até o final da chamada.

Já na **comutação de pacotes**, esses recursos **não são reservados** antecipadamente. Em vez disso, os dados são divididos em pequenos pacotes que compartilham dinamicamente os recursos da rede (como os enlaces e buffers dos roteadores) com pacotes de outras transmissões. Assim, cada pacote pode até seguir caminhos diferentes até o destino. Isso **torna a rede mais eficiente e flexível, mas pode gerar atrasos variáveis (fila de espera nos roteadores) e perdas ocasionais de pacotes**.

"*Se quisermos ir ao restaurante que exige reserva (comutação de circuitos), teremos que passar pelo aborrecimento de telefonar antes de sair de casa. Mas, quando chegarmos lá, poderemos, em princípio, ser imediatamente atendidos e servidos. No restaurante que não exige reserva (comutação de pacotes), não precismamos nos dar ao trabalho de reservar mesa, porém, quando lá chegarmos, talvez tenhamos de esperar*" (F. KUROSE, James, 2005, p.11)

### Diferença na conexão tipos de conexão:
<div>
    <img style="display: block; margin: auto;" alt="TCP_e_CC" height="670" width="980" src="/Networking/Images/TCP_e_CC.png">
</div>

Portanto, principais diferenças são: Comutação de circuito reserva recursos reais (fios, banda, buffers) enquanto o TCP apenas simula uma conexão confiável sobre uma rede que usa comutação de pacotes (IP), isto é, TCP organiza, reenvia e garante ordem dos pacotes, mas os roteados não reservam nada para ele.

<div>
    <img style="display: block; margin: auto;" alt="analogiaTCP_e_CC" height="670" width="980" src="/Networking/Images/AnalogiaTCP_CC.png">
</div>

Nem todas as redes são classificadas como redes de comutação de circuitos puras ou redes de comutação de pacotes puras, porém, essa classificação auxilia na compreensão de redes de telecomunicação.