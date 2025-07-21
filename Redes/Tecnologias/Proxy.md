O Proxy é um dispositivo ou serviço intermediário que fica entre um cliente ( como um navegador ) e o servidor final (como um site ).
Ele recebe as requisições dos clientes, decide o que fazer com elas ( enviar, negar, filtrar, armazenar etc) e as repassa ao destino ou responde diretamente.


### Para que serve um Proxy
Um proxy tem várias finalidades, dependendo de como é configurado. As principais são

#### 1. Controle de acesso à internet
- Filtrar sites proibidos,  bloquear categorias ( redes sociais, streaming jogos)
- implementar políticas de uso da internet por horário ou usuário.

#### 2. Segurança
- Esconde o [[Internet Protocol (IP)|Endereço IP]] real dos dispositivos internos
- pode analisar conteúdo malicioso antes de permitir acesso
- Atua como uma barreira extra entre a rede interna e a internet

#### 3. Cache (desempenho)
- Armazena relatórios detalhados de uso da internet, como sites acessados, tempo de navegação, volume de dados.

#### 4. monitoramento
- Gera relatórios detalhados de uso da internet, como sites acessados, tempo de navegação, volume de dados

### Como o Proxy funciona ?
**Passo a passo básico**:
1. um usuário tenta acessar um site
2. a requisição vai primeiro para o proxy, não diretamente para a internet
3. O Proxy
	- verifica se pode ou não permitir esse acesso
	- se estiver permitido, repassa a requisição ao site
	- Pode guardar uma cópia ( cache ) do conteúdo
4. o site responde -> o proxy recebe a resposta -> entrega ao usuário

### Tipos de Proxy
1. Proxy direto ( ou explicito )
	- O navegador ou sistema é configurado manualmente para usar o proxy
2. Proxy transparente
	- O proxy é colocado na rede de forma invisível para o usuário, interceptando as conexões automaticamente.
3. [[Proxy reverso]]
	- Fica na frente de servidores recebendo requisições externas e redirecionando para os servidores reais (muito usado em sites, balanceamento de cargam segurança)

### Proxy é a mesma coisa que [[Firewalls|firewall]] ?
Não. o firewall filtra pacotes com base em regras de rede ( endereços [[Internet Protocol (IP)|IP]], portas, protocolos).
O proxy atua em nível de aplicação (HTTP, HTTPS, FTP), entendendo o conteúdo das mensagens e podendo tornar decisões mais refinadas.

### Exemplo prático
Em uma empresa, os funcionários usam um navegador configurado para o proxy ``proxy.empresa.local:3128``. Quando tentam acessar o Youtube, o proxy bloqueia com  uma mensagem como 

> “Este site está bloqueado pela política de segurança da empresa.”


Se acessarem um site permitido, o proxy pode servir a página rapidamente, **sem acessar a Internet**, caso ela esteja em cache.



> [!tip] Analogia
> Pense no proxy como o porteiro de um prédio corporativo
> - Os funcionários (usuarios) querem sair do pŕedio (Acessar sites).
> - Antes de deixa-los sair, o porteiro verifica:
> 	- Se eles têm permissão para sair naquele horário.
> 	- Se o destino é permitido 
> 	- Se já foi ontem e trouxe folhetos (cache), ele ja tem uma cópia do que pegou.
> - Às vezes, o porteiro nem deixa sair. Diz "A empresa não permite esse tipo de passeio"




