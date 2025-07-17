MAC é um tipo de elemento: identificador único ( também chamado de endereço físico ou hardware address).
Ele é uma identificação única gravada fisicamente em cada interface de rede ( placa de rede Ethernet ou WI-fi). 


### MAC = Media Access Control

Ele tem um formato muito característico, um endereço MAC tem 48 bits (6 bytes ), geralmente escrito em hexadecimal.

``` Exemplo
00:1A:2B:3C:4D:5E
```

Ele é dividido em duas partes: 

 - **OUI** (Organizationally unique identifier) - 3 primeiros bytes -> fabricante.
 - **NIC-specific** 3 últimos bytes -> número único da placa.

#### Onde fica o endereço MAC ?
- Gravado na memória ROM da placa de rede ( NIC )
- Cada interface de rede tem seu próprio MAC. em PC com WI-fi e Ethernet tem dois MACs distintos. 

#### Para que serve o endereço MAC ?
O Mac é usado para identificar dispositivos em uma rede local ( LAN ) de forma unica.

Em uma rede com switch, quando um  PC envia dados, o [[Switch]] lê o endereço MAC de destino para saber em qual porta de vê enviar o pacote.

### Papel na comunicação

#### 1. Comunicação local (LAN)
 -  um computador envia um quadro com o MAC de destino.
 - O switch usa sua tabela MAC para enviar o quadro diretamente ao dispositivo certo.

#### 2. ARP ( Address Resolution Protocol)
 - Quando um dispositivo conhece o IP de destino, mas não o MAC, ele usa o Protocolo ARP para descobrir.



> [!tip] analogia
> Se o endereço IP é como o CEP de uma casa, o endereço MAC é como o número de série da caixa de correio, único e fixo, usado internamente no prédio (LAN) para encontrar o destino certo.

