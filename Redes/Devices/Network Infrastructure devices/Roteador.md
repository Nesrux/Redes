Um Roteador ( Router ) é um dispositivo de rede que conecta diferentes redes entre si e encaminha pacotes com base em endereços [[Internet Protocol (IP)|IP]].

## Função principal
- Encaminhar pacotes entre redes diferentes com base nos endereços IP de origem e destino.
- Atua na Camada 3 ( Rede ) do [[modelo OSI]].
- É o responsável pelo roteamento, ou seja, decidir o melhor caminho que os dados devem seguir até chegar ao destino.

### Exemplo no mundo real
Em uma casa, o roteador

- Conecta a rede local ( [[LAN]]) à internet ([[WAN]]).
- Atribui IPS locais (VIA DHCP)
- Traduz os IPs internos para IP público (Via NAT).
- Atua como Firewall básico.

### O que um roteador faz ?

| Função                                |Explicação|
|---|---|
| **Roteamento IP**                     |Encaminha pacotes com base em endereços IP.|
| **NAT (Network Address Translation)** |Traduz IPs privados para IP público (em casa ou empresas pequenas).|
| **DHCP**                              |Pode fornecer endereços IP automaticamente.|
| **Firewall**                          |Pode bloquear tráfego indesejado com regras.|
| **QoS, ACL, [[VPN]]**                 |Em modelos mais avançados, gerencia tráfego e segurança.|


> [!tip] Analogia
> Um roteador é como um chefe dos Correios.
> ele lê o CEP (Endereço IP de destino) de cada carta (pacote) e decide a melhor rota para entregá-la.
