# Modelo offline nas Configurações e comando /agente

## O que foi adicionado

- Em **Configurações**, existe a área **Modelo offline do sistema**.
- O admin pode escanear modelos locais do **Ollama** e do **LM Studio**.
- O modelo escolhido pode ser salvo como IA principal do sistema.
- O chat passa a responder usando o modelo offline selecionado quando ele estiver ativo.
- Em qualquer campo de texto do sistema, digite `/agente sua pergunta` e envie o formulário. O sistema troca o texto pela resposta da IA antes de salvar/enviar.
- Também é possível usar `Ctrl + Enter` dentro do campo para gerar a resposta sem enviar o formulário.

## Como usar com Ollama

1. Instale e abra o Ollama.
2. Baixe um modelo, por exemplo:

```powershell
ollama pull llama3.1:8b
```

3. Abra o Sistema Alvorada.
4. Vá em **Configurações > Modelo offline do sistema**.
5. Clique em **Escanear novamente**.
6. Selecione o modelo.
7. Marque **Usar modelo offline como IA principal**.
8. Clique em **Salvar modelo offline**.
9. Clique em **Testar modelo offline**.

## Como usar no chat

Digite no chat:

```text
/agente crie uma orientação para conferir o estoque da loja 3 hoje
```

O sistema salva sua pergunta e coloca a resposta da IA na conversa.

## Como usar em qualquer campo

Em qualquer campo de texto, por exemplo observação, descrição ou anotação:

```text
/agente monte uma observação profissional para esta tarefa de balanço
```

Ao enviar o formulário, o sistema chama a IA local, substitui o texto pela resposta e depois salva.
