# Importação de PDF multiloja

A tela **Importar PDF** agora também lê o modelo `LISTA DE REABASTECIMENTO` que vem com uma loja por página.

## O que o sistema identifica

- Código da loja pelo cabeçalho `MR01`, `MR02`, ..., `MR20`.
- Número do pedido quando o PDF traz o campo `NÚMERO` ou o padrão `1429384/26` no cabeçalho.
- Itens com colunas parecidas com:
  - Código
  - Código de barras
  - Descrição
  - Endereço
  - Estoque
  - Qtd. pedido
  - Embalagem
  - Fator da embalagem

## Como ele cria a separação

Quando o PDF tem várias lojas, o sistema agrupa os itens por loja detectada e cria uma separação para cada loja no mesmo lote.

A quantidade fica aberta para edição direta. Os demais campos continuam pedindo confirmação antes de alterar.

## Observação

O PDF precisa ser textual. Se ele for imagem/escaneado, será necessário adicionar OCR em uma próxima etapa.
