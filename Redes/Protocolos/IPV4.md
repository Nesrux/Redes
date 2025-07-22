IPV4 (Internet protocol version 4) é a quarta versão do [[Internet Protocol (IP)|Protocolo IP]], definida na RFC 791 (1981), e é a mais utilizada atualmente em redes privadas e grande parte da internet.

### Como funciona  o IPV4
- Usa endereços de 32 bits (quatro bytes)
- Representados em decimal com pontos
	- Exemplo : `192.168.1.10`


Cada endereço IPV4 tem duas partes:

|Parte|Função|
|---|---|
|**Rede**|Identifica a rede à qual o host pertence|
|**Host**|Identifica o dispositivo dentro da rede|
#### Formato de endereço IPv4
``` IPv4
[ 8 bits ] . [ 8 bits ] . [ 8 bits ] . [ 8 bits ]
Exemplo: 192      .  168     .   1     .   10
```

### Componentes importantes do IPv4
- Endereço do IP : Identifica um host
- Máscara de sub-rede: define qual parte do IP é rede e qual é host
- Gateway padrão: [[roteador]] para fora da rede
- Broadcast: envia para todos os hosts da rede
- NAT: permite acesso à internet com Ips privados.