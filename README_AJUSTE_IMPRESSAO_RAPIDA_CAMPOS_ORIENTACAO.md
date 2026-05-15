# Ajuste na Impressão Rápida

Melhorias aplicadas:

1. Campos maiores na tela de **Impressão rápida pela Base.xlsx**
   - Corrigido o problema dos campos de código/etiqueta ficarem pequenos por causa do botão de câmera.
   - O campo Produto, Código, Etiqueta e os demais campos agora ficam mais largos e legíveis.
   - No celular, os campos continuam responsivos.

2. Escolha de orientação ao imprimir
   - Ao clicar em **Imprimir agora**, abre uma janela perguntando a orientação:
     - Retrato / Vertical
     - Paisagem / Horizontal
   - A orientação escolhida é aplicada na planilha antes de enviar para impressão.

Arquivos alterados:
- `templates/impressao_rapida.html`
- `static/css/app.css`
- `controle_separacao/core.py`
