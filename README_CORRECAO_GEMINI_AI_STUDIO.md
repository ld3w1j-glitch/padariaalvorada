# Correção Google AI Studio / Gemini

Esta versão corrige o erro:

`models/gemini-1.5-flash is not found for API version v1beta, or is not supported for generateContent`

## O que mudou

- Adicionada seção **Configurações > Conectar Gemini**.
- Modelo padrão atualizado para `gemini-2.5-flash`.
- O sistema agora consulta `GET /v1beta/models` para listar modelos compatíveis com `generateContent`.
- Se o modelo salvo estiver indisponível, o sistema tenta escolher automaticamente outro modelo compatível.
- Botão **Listar modelos Gemini** para conferir quais modelos sua chave realmente pode usar.
- Botão **Testar Gemini**.
- O Gemini pode ser salvo como IA principal do sistema quando nenhum modelo offline estiver ativo.

## Como usar

1. Entre como admin.
2. Abra **Configurações**.
3. Vá até **Google AI Studio > Conectar Gemini**.
4. Cole sua chave do Google AI Studio.
5. Use o modelo `gemini-2.5-flash` ou clique em **Listar modelos Gemini**.
6. Clique em **Salvar Gemini como IA principal**.
7. Clique em **Testar Gemini**.

Se o modelo offline estiver ativado, ele continua tendo prioridade sobre Gemini/OpenAI.
