# Relatório de todas as linhas do estoque

Foi adicionada na aba **Relatórios** uma visão geral que calcula todas as linhas existentes no estoque atual.

## O que aparece na tela

- Valor total estimado do estoque
- Quantidade total em estoque
- Quantidade de linhas encontradas
- Total de itens existentes
- Itens abaixo do estoque
- Itens zerados

## Tabela por linha

Para cada linha do estoque o sistema mostra:

- Linha do estoque
- Itens existentes
- Quantidade em estoque
- Quantidade abaixo do estoque
- Quantidade zerada
- Custo médio
- Valor estimado

## Exportação

Na aba **Relatórios** foi adicionado o botão **Exportar linhas Excel**.

Ele gera um arquivo `.xlsx` com o cálculo de todas as linhas do estoque.

## Observação

O cálculo usa os itens ativos da tabela `stock_items`. Quando existir `linha_caminho_erp`, ela é usada como nome da linha. Se não existir, o sistema usa `linha_erp`. Se o item não tiver linha, ele aparece como **Sem linha**.
