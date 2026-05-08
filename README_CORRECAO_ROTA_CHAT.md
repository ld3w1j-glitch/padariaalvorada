# Correção aplicada

Corrigido erro ao iniciar o sistema:

`AssertionError: View function mapping is overwriting an existing endpoint function: limpar_conversa_chat`

Causa: a rota de envio de mensagem ficou acidentalmente apontando para a função de limpar conversa.

Ajuste realizado:

- `/comunicacao/grupos/<id>/limpar` agora aponta somente para `limpar_conversa_chat`.
- `/comunicacao/grupos/<id>/mensagem` agora aponta corretamente para `enviar_mensagem_chat`.

Depois de extrair este ZIP, execute novamente:

```powershell
C:/Python314/python.exe app.py
```
