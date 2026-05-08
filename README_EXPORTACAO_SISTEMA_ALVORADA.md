# Exportação sistema_alvorada.db após finalizar separação

Esta versão gera um arquivo `.db` no padrão do banco `sistema_alvorada` usado pela automação externa.

## Onde aparece

### Na tela da separação
Quando a separação estiver pronta para finalizar, aparecem dois botões:

- **Finalizar separação / Finalizar direto**: finaliza normalmente.
- **Finalizar e baixar sistema_alvorada**: finaliza e já baixa o arquivo `.db`.

Depois que a separação já estiver finalizada, também aparece:

- **Exportar sistema_alvorada.db**

### No histórico do lote
Na tela de histórico do lote, aparece o botão:

- **Exportar sistema_alvorada.db**

Esse botão gera um único arquivo com todas as lojas finalizadas do lote.

## Estrutura gerada no arquivo `.db`

O arquivo contém as tabelas no padrão informado:

- `pedidos_suspensos`
- `produtos`
- `produtos_editados`
- `produtos_removidos`
- `execucoes_lote`
- `execucoes_lote_lojas`
- `agendamentos_automacao`

## Regra usada nos itens

Para cada item da separação:

- `loja`: pega o número do nome da loja, por exemplo `Loja 8` vira `8`.
- `produto`: usa o código do item.
- `nome_produto`: usa a descrição.
- `qtd`: usa a quantidade separada. Se estiver zerada, usa a quantidade pedida.
- `status`: entra como `PENDENTE`, para a automação lançar depois.
- `data_lancamento`: usa o nome do lote.

## Observação importante

Para o outro programa reconhecer corretamente as lojas, cadastre as lojas com número no nome, por exemplo:

- Loja 8
- Loja 9
- Loja 10

Se o nome da loja não tiver número, o sistema usa o ID interno da loja como alternativa.
