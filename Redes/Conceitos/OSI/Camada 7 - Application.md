A camada 7 faz parte do [[Modelo OSI]], a função é ser a camada mais próxima do usuário final. Ela fornece os serviços de rede diretamente às aplicações do sistema operacional, como navegadores, clientes de e-mail, FTPs, etc.

### Oque essa camada faz ?
A Camada de application: 
- Permite que os programas de usuário usem a rede para se comunicar
- não é a aplicação em sí, mas os serviços de rede que ela acessa.
- Garante que haja interface, autenticação e compatibilidade entre o software do usuário e a rede.
- ou seja: é a onde a comunicação começa e termina no lado do usuário.

### Protocolos que operam na camada 7
- Http/Https -> Navegação web
- FTP/SFTP -> transferencia de arquivos
- SMTP -> Envio de e-mails
- SSH -> Acesso remoto seguro
- DNS -> tradução de nomes para IPS

### Como funciona a comunicação na prática ?
Imagine que você digite ``www.exemplo.com`` no seu navegador:
1. A aplicação (navegador) solicita uma página via HTTP
2. Essa solicitação passa pela camada de application, que embala a requisição no formato correto
3. Depois, ela desce pelas outras camadas e sai pela rede
4. no destino (servidor), a Camada 7 entende que é uma requisição HTTP, e responde com a página solicitada.