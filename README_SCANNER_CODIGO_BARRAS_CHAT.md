# Scanner de código de barras no chat

Melhoria adicionada na tela **Chat/Tarefas**.

## O que mudou

- Foi adicionado um botão de câmera ao lado do ícone de anexar arquivo no campo de mensagem.
- Ao escanear um código de barras, o sistema consulta o estoque.
- Se o produto existir, o campo de texto do chat é preenchido com:
  - código;
  - código de barras;
  - descrição;
  - quantidade total existente no estoque.
- Se o produto não existir, o sistema cadastra automaticamente o código no estoque com quantidade `0` e descrição em branco, para ser preenchida posteriormente.
- Também existe entrada manual no modal, caso o navegador não consiga ler o código pela câmera.

## Observação importante

A leitura pela câmera usa a API nativa `BarcodeDetector` do navegador. Ela funciona melhor no Chrome/Edge atualizado em Android e exige HTTPS em produção ou localhost em teste.
