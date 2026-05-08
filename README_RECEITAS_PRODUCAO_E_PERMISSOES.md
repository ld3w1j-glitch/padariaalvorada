# Atualização: permissões, supervisor, receitas e ordem de produção

## Permissões

- Adicionado o cargo **Supervisor**.
- Os cargos **Gerente**, **Desenvolvedor** e **Supervisor** recebem acesso operacional amplo, parecido com admin.
- As áreas sensíveis continuam exclusivas do admin real:
  - Usuários
  - Configurações
  - Código fonte
  - Auditoria

## Nova aba: Receitas/Produção

A nova aba aparece no menu como **Receitas/Produção**.

### Criar receita

1. Informe o código do produto final já existente no estoque.
2. Salve a receita.
3. Em seguida, adicione ingredientes pelo código/código de barras já existente no estoque.
4. Informe a quantidade de cada ingrediente e a unidade: kg, g, litro, ml ou unidade.
5. Use o campo de observação para colocar modo de preparo.

### Criar ordem de produção

1. Escolha a loja/destino.
2. Escolha a receita.
3. Informe a quantidade total do pedido.
4. O sistema cria uma ordem de produção e calcula o total de ingredientes necessário.

### Conferência pelo padeiro

Na tela da ordem, o padeiro consegue registrar a quantidade produzida de cada item. Cada atualização fica salva no histórico da ordem.

### Exportação mensal

Na aba Receitas/Produção existe o botão **Exportar histórico CSV**, com filtros de data inicial e final. Esse arquivo pode ser usado como relatório mensal do que foi produzido.


## Remover ordens de produção

Na aba **Receitas/Produção**, cada ordem criada possui o botão **Remover**. Também é possível abrir a ordem e usar **Remover ordem** no topo da tela.

Ao remover uma ordem:

- a ordem deixa de aparecer na lista de ordens;
- seus itens e registros internos de conferência são apagados;
- a ordem removida deixa de sair no CSV de histórico mensal;
- um resumo da remoção fica salvo na auditoria com título, loja, status e itens principais.
