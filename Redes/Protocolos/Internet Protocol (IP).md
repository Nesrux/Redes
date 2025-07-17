O IP é um protocolo de rede usado para endereçar, identificar e encaminhar pacotes de dados entre dispositivos em redes interconectadas.

### Funções principais do protocolo IP

##### 1. Identificação
Cada dispositivo em uma rede IP recebe um endereço único chamado endereço IP. esse endereço identifica o dispositivo na rede.

##### 2. Encaminhamento de pacotes (roteamento)
O IP permite que os dados sejam enviados de uma rede de origem até uma rede de destino, mesmo que passe por diversas redes intermediárias.

##### 3. Fragmentação e remontagem
se os dados forem muito grandes para uma rede intermediária, o IP pode fragmentar os pacotes depois reconstruí-los no destino.

### Como o protocolo IP funciona ?
- O IP trata os dados como pacotes independentes.
- Cada pacote contém
	- Endereço de origem
	- Endereço de destino
- O protocolo IP não estabelece conexão nem garante entrega.
	- Por isso é chamado de não confiável e sem conexão
	- se o pacote se perder, o IP tenta reenviar.

**Protocolos como TCP ou UDP** trabalham junto com o IP para adicionar funcionalidades como controle de erros ou velocidade.


### Estrutura básica de um pacote IP
``` simplificado

[ Cabeçalho IP ] [ Dados do protocolo superior (ex: TCP/UDP) ]

```
O cabeçalho IP inclui
 - Endereço de origem
 - Endereço de destino
 - Tamanho do pacote
 - TTL (Time to live )
 - identificador de protocolo (TCP, UDP, ICMP, etc.)

#### Importante
IP é um protocolo de entrega lógica, não física
- Ele não usa endereços físicos [[Endereço MAC|MAC]] diretamente;
- Ele confia na camada de enlace para transportar o pacote dentro de cada rede.
- o IP encaminha pacotes entre redes diferentes, enquanto a camada 2 transmite pacotes dentro da mesma rede.


> [!tip] Analogia
> O protocolo IP é como serviço postal de um país
> - Ele não se importa com o conteúdo da carta (dados)
> - só lê o remetente e destinatário (endereços IP) e decide o caminho que a carta deve seguir.
