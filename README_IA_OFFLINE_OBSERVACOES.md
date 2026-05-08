# IA offline nas observações da Área do usuário

Esta versão adiciona, dentro do campo **Anotações relevantes**, os botões:

- **Escanear IA offline**: procura modelos locais no PC onde o Flask está rodando.
- **IA criar observação**: usa o título, meta, início e prazo da tarefa para gerar uma observação prática.

## Conexões suportadas

### Ollama
1. Instale/abra o Ollama no PC.
2. Baixe um modelo, por exemplo: `ollama pull llama3.1:8b`.
3. Deixe o Ollama rodando em `http://127.0.0.1:11434`.
4. No sistema, clique em **Escanear IA offline** e escolha o modelo.

### LM Studio
1. Abra o LM Studio.
2. Carregue um modelo local.
3. Ative o servidor local OpenAI Compatible em `http://127.0.0.1:1234`.
4. No sistema, clique em **Escanear IA offline** e escolha o modelo.

## Arquivos locais
O sistema também lista arquivos comuns de modelos, como `.gguf`, `.ggml`, `.bin` e `.safetensors`, nas pastas Downloads, Documents, Models/Modelos, LM Studio e cache do Hugging Face. Porém, para gerar texto, o modelo precisa estar carregado em um servidor local como Ollama ou LM Studio.

## Privacidade
A geração usa apenas endereços locais (`127.0.0.1`). O texto da tarefa não é enviado para API externa.
