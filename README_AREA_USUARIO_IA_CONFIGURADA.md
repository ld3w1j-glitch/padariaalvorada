# Área do usuário usando a IA configurada

Alteração aplicada:

- A área do usuário não obriga mais escolher uma IA offline separada.
- O botão de observação agora usa automaticamente a IA principal configurada em **Configurações**.
- Funciona com:
  - Google Gemini, quando salvo como IA principal;
  - OpenAI/ChatGPT, quando salvo como IA principal;
  - Ollama/LM Studio, caso o modelo local esteja habilitado nas Configurações.
- Se nenhuma IA estiver conectada, o sistema retorna aviso pedindo para configurar primeiro.

Arquivos alterados:

- `templates/area_usuario.html`
- `controle_separacao/core.py`

Fluxo novo:

Área do usuário → IA configurada criar observação → sistema consulta Configurações → chama Gemini, OpenAI ou modelo local habilitado.
