Um Hub é um dispositivo de rede da Camada 1 do modelo OSI.
Ele recebe sinais elétricos de um dispositivo e os replica para todas as portas sem nenhum tipo de inteligência ou decisão lógica.

### Função principal
- Atua como um repetidor físico
- não entende endereços, não filtra dados e não direciona pacotes.
- Todos os dispositivos conectados recebem o mesmo sinal, oque gera muito tráfego desnecessário


### Como um Hub funciona ?
1. Um computador envia um sinal (quadro) para a rede via sua porta Ethernet.
2. O hub replica esse sinal para todas as outras portas, independentemente do destino.
3. Todos os dispositivos recebem o sinal, mas apenas o destinatário certo processa o dado. os outros descartam.

### Por que os Hubs foram abandonados ?
- Criam grande quantidade de colisões em redes Ethernet (Domínio de colisão único).
- Consomem largura de banda desnecessariamente
- Não são seguros. qualquer dispositivo conectado recebe os dados de todos.
- foram substituídos por [[Switch|Switches]], que operam na Camada 2 e encaminham quadros com base no [[Endereço MAC]]