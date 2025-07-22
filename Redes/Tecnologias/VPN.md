VPN significa **Virtual Private network**. É uma tecnologia que permite criar uma conexão segura e criptografada entre dois pontos através de uma rede pública, geralmente a internet.

### Para que serve uma VPN ?
uma VPN tem vários usos práticos, mas todos envolvem segurança e privacidade de dados. Ela serve para
1. **Acesso remoto seguro**
	  - Ex: Um funcionário acessa o sistema da empresa de casa como se estivesse no escritório.
2. **Conexão entre filiais**
	 - Empresas podem interligar escritórios geograficamente distantes como se estivessem na mesma [[LAN]].
3. Privacidade na internet
	- O tráfego é criptografado, ninguém (nem seu provedor de internet) pode ver oque você acessa.
4. Acesso a conteúdo com restrição geográfica
	- Uma VPN pode fazer você "Parecer" que está em outro pais.
5. Evitar censura e bloqueios
	- Em países com internet restrita, VPNs são usadas para driblar bloqueios.


### Como funciona uma VPN ?
#### 1.Criação de túnel virtual (tunelamento)
A VPN cria um "Túnel lógico", entre seu dispositivo e o destino. Esse túnel é como um canal privado dentro da internet pública.

#### 2.Criptografia de ponta a ponta
Tudo que você envia ou recebe é criptografado dentro desse túnel, impedindo que alguém intercepte e entenda os dados.

#### 3.Autenticação
O Acesso à VPN exige autenticação (Usuário e senha, certificado etc), garantindo que só pessoas autorizadas possam usá-la.

#### 4. Encapsulamento de pacotes [[Internet Protocol (IP)|IP]]
Os dados originais são encapsulados dentro de novos pacotes para poderem circular pela internet e, no outro lado da VPN, são "Desempacotados".

### Tipos de VPN
1. VPN site-to-site
	- Liga duas redes inteiras
	- Usada por empresas
2. VPN client-to-site (ou remote access)
	- Um único usuário remoto se conecta a uma rede corporativa.
3. VPN comercial (ou pessoal)
	- Usada por usuários comuns para privacidade onlline

### Protocolos usados em VPNs
- **IpSec**: Muito seguro. Usado em VPNs corporativas
- **SSL/TLS**: Usado em VPNs de acesso remoto, via navegador.
- **OpenVPN**: Muito usado em soluções modernas
- **L2TP/IPSEC, IKEV2, WireGuard**: outras opções populares