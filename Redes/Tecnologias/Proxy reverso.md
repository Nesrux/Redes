Um proxy reverso é um servidor intermediário que fica na frente de um ou mais servidores web e recebe requisições do cliente externo (como navegadores).
Ao contrario do [[Proxy]] tradicional, que protege o cliente, o proxy reverso protege e gerencia o lado do servidor. 

### Para que serve um proxy Reverso ?
1. Distribuição de carga (load balancing)
	- Divide o tráfego entre vários servidores para evitar sobrecarga.
2. Segurança e anonimato dos servidores reais
	- Os usuários acessam apenas o proxy reverso, que esconde os servidores reais atrás dele.
3. Cache de conteúdo
	- Pode armazenar respostas de páginas e entregar rapidamente sem precisar consultar os servidores reais.
4. Criptografia SSL/TLS (offload)
	- O proxy pode cuidar da criptografia, avaliando os servidores web dessa tarefa.
5. Compressão e otimização de dados
	- Reduz o tempo de resposta e o uso de banda.
6. Firewall de aplicações (WAF)
	- Pode analisar o tráfego web para detectar e bloquear ataques (SQL injection, XSS, ETC)

### Como funciona o fluxo de um proxy reverso ?
##### Exemplo de fluxo: 

1. Um usuário acessa ``Https://www.site.com
2. a requisição vai para o proxy reverso, que esta configurado no [[DNS]] como ``www.site.com``
3. o Proxy
	- verifica se pode entregar algo em cache
	- ou escolhe um dos servidores reais para encaminhar a requisição (ex : ``10.0.0.10``)
	- Recebe a resposta e repassa para o usuário
4. o usuário nunca vê o [[Internet Protocol (IP)|IP]] ou nome real do servidor interno

### Diferença entre proxy tradicional e proxy reverso
|Característica|Proxy Tradicional|Proxy Reverso|
|---|---|---|
|Protege|O cliente|O servidor|
|Fica entre|Cliente e Internet|Internet e Servidores Internos|
|Caso de uso típico|Filtrar acesso à web|Balancear e proteger servidores|
|Visto em|LANs de empresas/escolas|Sites, data centers, nuvem|
