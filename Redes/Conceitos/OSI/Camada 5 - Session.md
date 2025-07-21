A Session layer é uma das 7 camadas do [[Modelo OSI]] responsável por iniciar, manter e encerrar sessões de comunicação entre dos dispositivos de rede.
Ela cuida de:
- **Estabelecer uma sessão**: Cria um canal de comunicação lógico entre duas aplicações.
- **Gerenciar a sessão**: mantém a comunicação ativa, controla quem fala quando.
- **Encerrar a sessão**: Fecha a conexão de forma ordenada e limpa.
- **Sincronização e controle**: Permite pausar e retomar uma sessão,  ou dividir em "Pontos de restauração" (checkpoints), úteis em transferências longas.

Essa camada garante que uma conversa entre dois sistemas possa começar, continuar e terminar de forma ordenada e correta, mesmo que a conexão sofra interrupções.


### como ela funciona na pratica ?
Imagine uma videoconferência entre dois usuários:
1. Quando um usuário entra na camada, a Session layer estabelece a sessão.
2. Durante a conversa, ela mantém a conexão estável, mesmo que o vídeo pause temporariamente ou a conexão sofra uma instabilidade
3. Se o usuário sair da chamada, essa camada garante que tudo seja encerrado corretamente, liberando os recursos da redes.