A Camada 4 é uma das 7 camadas do [[Modelo OSI]], ela é responsável por garantir que os dados sejam entregues de forma confiável e ordenada entre dois dispositivos em uma rede. Ela também gerencia o controle de fluxo, detecção de erros, e até mesmo a recuperação de dados perdidos, dependendo do tipo de protocolo usado.
As principais responsabilidade da Transport layer incluem:
- **Segmentação e remontagem dos dados**: divide dados grandes em partes menores (segmentos) para envio e depois reagrupa na recepção
- **Entrega confiável ou não confiável**: dependendo do protocolo, pode garantir que os dados cheguem intactos e na ordem correta (como no TCP), ou apenas enviá-los sem garantia (como no UDP).
- **Controle de fluxo**: evita que o remetente envia dados mais rápido do que o receptor consegue processar.
- **Controle de erros**: Detecta e pode corrigir erros nos dados transmitidos.
- **Multiplexação**: Permite que vários aplicativos usem a rede simultaneamente sem confusão, usando portas 

### Como funciona na prática ?
imagine que você está assistindo a um vídeo no Youtube
- A Transport layer do servidor divide o vídeo em segmentos e os envia pela rede.
- A transport layer do seu computador reagrupa os segmentos na ordem correta.
- Se algum segmento se perder ou chegar com erro, ela pode pedir o reenvio
- Também garante que você receba dados numa taxa que seu dispositivo consiga processar

Esse processo ocorre transparente para o usuário, tudo acontece nos bastidores.


### Relação com outras camadas
- Recebe dados da session layer, e os transforma em segmentos
- Envia os segmentos para a network layer, que cuida do endereçamento IP
- Atua como ponte entre a lógica de sessão e o roteamento físico dos dados.
