A camada 3 é uma das 7 camadas do [[Modelo OSI]], ela é responsável por enviar os dados de um dispositivo em uma rede para outro em uma rede diferente, ou seja, ela faz o roteamento dos pacotes.
Suas principais funções são:
- **Endereçamento lógico**: Atribui e usa [[Internet Protocol (IP)|Endereços IP]] para identificar de onde os dados vêm e para onde vão.
- **Encapsulamento em pacotes**: Os dados vindos da camada de transporte são colocados em pacotes, com informações de origem e destino.
- **Roteamento**: Escolhe o melhor caminho na rede (ou entre redes) para que os pacotes cheguem ao destino, mesmo que passem por vários dispositivos.
- **Fragmentação**: se o pacote for maior que a rede intermediária suporta, ele pode ser dividido em fragmentos menos.
- **Controle de congestionamento e erros simples**: Ajuda a evitar sobrecarga da rede (em protocolos mais complexos).

Ou seja, a camada de network é a mente que toma decisões de caminho. Ela não se importa com o conteúdo, mas com para onde os dados devem ir e como chegar lá.

### Como ela funciona na prática ?
Imagine que você está em uma rede doméstica e acessa o site ``www.cisco.com``:
1. seu dispositivo gera um pacote com os dados da requisição
2. A Network layer coloca o endereço Ip do seu computador com origem e o IP do servidor da cisco como destino.
3. Um roteador (device) analisa esse endereço e decide por onde enviar esse pacote.
4. o pacote pode atravessar vários roteadores e redes até chegar ao servidor da Cisco.
5. quando o servidor responde, o processo se inverte.

### Relação com as outras camdas
- Recebe segmentos da Transport Layer e os encapsula em pacotes.
- Envia esses pacotes para a Data link layer, que cuida da entrega local.
- Usa o endereçamento lógico, ao contrario da layer 2, que usa o endereçamento físico (MAC)