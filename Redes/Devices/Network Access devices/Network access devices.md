Network access devices (NADs) são dispositivos de rede que controlam, permitem ou negam o acesso de usuários e dispositivos à rede.
Eles atual como ponto de entrada fisico ou lógico a uma rede, especialmente em redes com controle de acesso baseado em autenticação, como 802.1x

### Função principal

- Receber solicitações de acesso à rede de dispositivos ([[Host]])
- Encaminhas essa solicitação para um servidor de autenticação (ex: RADIUS)
- permitir ou negar o acesso com base na resposta recebida



#### Exemplos de Network Access Devices

|Tipo de dispositivo|Descrição|
|---|---|
|**Switch de borda**|Recebe conexões de hosts via cabo (Ethernet)|
|**Access Point (AP)**|Recebe conexões sem fio (Wi-Fi)|
|**Controladora wireless**|Controla múltiplos APs, também pode ser NAD|
|**Porta 802.1X habilitada**|Qualquer porta de switch configurada para autenticação|


### Porque os NADs são importantes ?
- permitem controle centralizado de acesso à rede
- Aumentam a segurança, impedindo que qualquer dispositivo se conecte automaticamente.
- Permitem aplicar políticas baseadas em identidade
	- VLAN dinâmica
	- ACLs por usuário
	- Limitação de banda


> [!tip] Analogia
> Um Network access device é como um porteiro digital da sua rede.
> ele pede a identidade de quem está tentando entrar, consulta um banco de dados e só abre a porta se estiver autorizado.

