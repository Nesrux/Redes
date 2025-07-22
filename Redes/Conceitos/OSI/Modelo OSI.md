O modelo OSI foi criado pela ISO (international Organization for Standardization) por volta de 1984

### Por quê ?
Antes do modelo OSI, cada fabricante criava sua própria forma de comunicação, IBM, DEC, XEROX, e os sistemas não eram compatíveis entre sí.

> O Objetivo do OSI era padronizar a comunicação de redes, para qualquer sistema de qualquer fabricante pudesse se comunicar com outro, independente da arquitetura interna.

### Como foi criado ?
Um grupo da ISO, em colaboração com a UIT-T, estudou diversas arquiteturas de redes existentes e criou um modelo genérico modular com 7 Camadas.
Esse modelo não é um protocolo, mas uma referência para o design e entendimentos de protocolos.

### As 7 camadas do Modelo OSI
##### 1. Camada 7 -> **Application**
  Onde os usuários interagem com a rede (navegadores, emails, etc)
##### 2. Camada 6 -> **Presentation**
Tradução de dados: criptografia compressão, conversão de formatos
##### 3. Camada 5 -> **Session**
Gerencia conexões (sessões), abertura e encerramento entre aplicações
##### 4. Camada 4 -> **Transport**
Garante entrega confiável ou rápida de dados (TCP, UDP)
##### 5. Camada 3 -> **Network**
Roteamento dos pacotes pela rede (IP, ICMP)
##### 6. camada 2 -> **Data Link Layer**
Comunicação direta entre dispositivos na mesma redes (Ethernet, MAC)
##### 7. Camada 1 -> **Physical**
Transmissão elétrica/óptica/ radio de bits (Cabos, sinais, conectores)

### Por que o OSI é importante hoje?
- Ajuda a entender como os protocolos funcionam
- Serve como base para arquitetura TCP/IP
- Facilita o diagnóstico de problemas em redes
- é exigido em certificações como CCNA, CCNP, CompTIA