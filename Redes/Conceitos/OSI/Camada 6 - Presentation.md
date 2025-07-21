A camada 6 - presentation é uma das 7 camadas do [[Modelo OSI]], a função dela é ser responsável por traduzir, formatar e preparar os dados para que possam ser compreendidos entre sistemas diferentes. Ela atua como um intérprete entre o que a aplicação entende e o que a rede pode transmitir.
Ela cuida de:
- Conversão de formatos de dados
- Serialização e desserialização de dados.
- Codificação e decodificação
- Criptografia e descriptografia
- Compressão e decompressão

> Em essência, a Layer 6 garante que a mensagem enviada por um sistema possa ser compreendida por outro, mesmo que eles usem formatos diferentes ou convenções diferentes internamente.

### Como funciona na prática ?
Vamos imaginar que estamos em um site utilizando Https com imagens e texto

1. O navegador (Na application layer) solicita dados do servidor.
2. A resposta vem criptografada e comprimida, quem lida com isso é a Presentation layer.
3. Ela descriptografa, descomprime, converte e entrega os dados prontos para o navegador mostrar.