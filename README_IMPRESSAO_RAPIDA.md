# Impressão rápida com Base.xlsx

Foi adicionada a seção **Impressão rápida** no menu do sistema.

## O que faz

- Usa o modelo `templates_impressao/Base.xlsx` enviado pelo usuário.
- Permite pesquisar um item já existente no estoque por código, código de barras ou descrição.
- Preenche automaticamente o produto e a embalagem quando um item do estoque é selecionado.
- Permite editar manualmente produto, código, peso/embalagem, produção, validade, etiqueta e quantidade de pacotes antes de imprimir.
- Permite baixar a planilha preenchida em Excel.
- Permite tentar imprimir direto na impressora configurada no computador/servidor.

## Impressoras

A busca de impressoras usa o sistema operacional onde o Flask está rodando:

- Windows: tenta `pywin32`, PowerShell ou WMIC.
- Linux/macOS: tenta CUPS/`lpstat`.

No navegador não é possível parear Bluetooth/USB diretamente por segurança. Primeiro conecte ou instale a impressora no Windows ou no servidor; depois clique em **Procurar novamente** na seção de configuração.

## Impressão automática

No Windows, a impressão usa o aplicativo associado ao `.xlsx`, normalmente o Excel ou LibreOffice. Se a máquina não tiver aplicativo associado para imprimir `.xlsx`, use o botão **Baixar Excel preenchido** e imprima manualmente.

## Arquivos alterados

- `controle_separacao/core.py`
- `templates/impressao_rapida.html`
- `templates/partials/_topbar.html`
- `static/css/app.css`
- `templates_impressao/Base.xlsx`
