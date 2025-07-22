A camada 2 é uma das 7 camadas do [[Modelo OSI]], é responsável por estabelecer uma conexão direta entre dois dispositivos na mesma rede física, garantindo que os dados possam ser entregues com confiabilidade dentro dessa rede local.
Principais funções:

- **Endereçamento físico** com o uso de endereços [[Endereço MAC|MAC]]
- **Encapsulamento em quadros**: transforma os pacotes da Layer 3 em unidades chamadas frames.
- **Detecção e Correção de erros** nos dados transmitidos.
- **Controle de acesso ao meio (MAC sublayer)**: decide quem pode usar o meio de transmissão (por exemplo, quando dois dispositivos compartilham o mesmo cabo).
- **Sincronização de quadros** Garante que o receptor saiba onde os dados começam e terminam
- **Reconhecimento de entrega local**: Confirma se o dado foi recebido corretamente pelo destino local.

A Layer 2 não se importa com IP ou com destino final dos dados; ela só se preocupa em garantir que os dados cheguem até o próximo nó da rede com integridade.

### Subcamadas da Layer 2
A Data Link é dividida em duas subcamadas:

#### 1. Logical Link Control (LLC)
- Comunica com a [[Camada 3 - Network|Layer 3]].
- Lida com controle de fluxo e erros.
- identifica qual protocolo da camada superior está sendo usado (IP, PX)

#### 2. Media access Control
- Define como os dispositivos acessam o meio físico
- Usa endereços MAC
- Atua fortemente em tecnologia como Ethernet e wi-fi

### Como funciona na prática ?
Imagine dois computadores na mesma rede doméstica trocando arquivos.

- O computador ``A`` Encapsula os dados em um frame e coloca o endereço MAC de destino (``Computador B``)
- Esse frame é transmitido pela rede.
- o [[Switch]] lê o endereço MAC e encaminha o frame para o dispositivo certo.
- o computador ``B`` recebe, verifica erros, confirma que o frame é para ele, e entrega os dados para camada superior.

Tudo isso ocorre sem usar roteamento ou IPS, apenas endereços MAC e regras locais.

### Resumo direto
- A Data link layer entrega dados entre dispositivos locais, na mesma rede física.
- Usa endereços MAC e encapsula os dados em frames.
- Detecta erros, controla acesso ao mesmo e sincroniza os dados.
- Não se preocupa com IPS ou roteamento
- Atua diretamente com dispositivos como switches e NICs