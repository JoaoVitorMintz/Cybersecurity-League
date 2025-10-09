**Referência:** Redes de computadores e a internet: uma abordagem top-down de James F. Kurose, Leitura realizada pela plataforma biblioteca virtual.

## O que são comutadores de pacotes?

Equipamentos interconectados indiretamente por equipamentos intermediários conhecidos como **comutadores de pacotes** (encaminha a informação que está chegando em um de seus enlaces de comunicação de entrada para um de seus enlaces de comunicação de saída). Blocos de informação são comumente chamados de **pacote**. Há diversos tipos de comutadores de pacotes, sendo os dois mais comum na internet: **roteadores** e **comutadores de camada de enlace (switches)**. Esses comutadores encaminham pacotes a seus destinos finais.

A sequência de enlaces de comunicação e comutadores de pacotes que percorre desde o sistema final remetente até o sistema final receptor é conhecido como **rota** através da rede. A internet não provem de um caminho dedicado entre sistemas finais comunicantes mas utiliza de uma técnica chamada **comutação de pacotes** que permite que diversos sistemas finais comunicantes compartilhem ao mesmo tempo um caminho ou partes dele.

## O que são protocolos?

Os sistemas finais, os comutadores de pacotes e outras peças da Internet executam **protocolos** que controlam o envio e o recebimento de informação dentro da Internet. O **TCP** (Transmission Control Protocol) e o **IP** (Internet Protocol) São dois dos protocolos mais importantes da internet. O protocolo IP especifica o formado dos pacotes que são enviados e recebido entre roteadores e sistemas finais. Os principais protocolos da internet são conhecidos coletivamente como **TCP/IP**.

## Protocolo como analogia humana:
<div>
    <img style="display: block; margin: auto;" alt="ProtocolExample" height="640" width="950" src="/Networking/Images/Protocol.png">
</div>

Pela imagem, é visivel que o protocolo humano (boas maneiras) ordena que iniciemos uma comunicação primeiramente com um "oi" e um "oi" como resposta indicando que pode-se prosseguir na interação. No caso de uma resposta diferente do "oi" exemplificado pode indicar portanto incapacidade de comunicação. Após isso, é de protocolo humano requisitar algo, que no caso do exemplo, seria as horas. Esse exemplo mostra que deve-se garantir o protocolo para que as respostas batam e a interação seja realizada, sendo portanto válido também para redes para que entidades comunicantes executem o mesmo protocolo para que uma tarefa seja realizada.

## O que são, de fato, os RFCs:

RFCs são documentos que definem padrões desenvolvidos pela IETF para protocolos. Inicialmente, os RFCs recebiam solicitações de comentários para resolver problemas de arquitetura que a a percursora da internet enfrentava, sendo um tipo de documentação muito técnica e detalhados. Definem protocolos como TCP, IP, HTTP e SMTP (Simple Mail Transfer Protocol). Existem mais de 3500 RFCs. Há também outros tipos de padrões especificados por outros órgãos como o IEEE que define, por exemplo, o IEEE 802 LAN/MAN que especifica os padrões de Ethernet e Wi-Fi sem fio.

## Exemplificando e explicando intranets:

A internet é um tipo de rede pública (rede global de redes) e rede privada são comumentes usadas em redes corporativas ou governamentais, cujos hospedeiros não podem trocar mensagens com hospedeiros que estão fora da rede privada (a menos que as mensagens passem por dispositivos denominados **firewall** que restringe o fluxo de mmensagens para dentro e para fora da rede). Essas redes privadas são frequentemente denominadas **intanets** por usarem o mesmo tipo de hospedeiros, roteadores, elaces e protocolos da inetnet pública.
