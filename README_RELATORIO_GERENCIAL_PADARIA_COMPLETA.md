# Ajuste no Relatório Gerencial - Padaria Completa

O relatório gerencial agora abre por padrão com a linha base **Padaria**, em vez de **Padaria - Industria CD**.

Com isso, o cálculo de valor em estoque, quantidade, itens zerados, estoque baixo, itens críticos e sublinhas passa a considerar todos os itens que contenham Padaria no caminho ERP/linha/descrição.

## Antes
- Filtro padrão: `Padaria - Industria CD`
- Pegava somente os itens dentro da sublinha de indústria.

## Agora
- Filtro padrão: `Padaria`
- Pega também lanchonete, confeitaria, rotisseria, embalagens, matérias-primas e outras linhas ligadas à Padaria.

O campo **Linha principal** continua editável, então ainda é possível digitar `Padaria - Industria CD` manualmente quando quiser voltar para esse recorte menor.
