# Ajuste no balanço: itens sem cadastro e edição de contagem

Implementações feitas:

- Ao registrar/escancear um código no balanço que ainda não existe no estoque, o sistema agora adiciona o item mesmo assim ao histórico da contagem.
- O item aparece marcado como **Não cadastrado** no relatório de comparação.
- No próprio histórico do balanço, o usuário com permissão de cadastro no estoque pode preencher a descrição e clicar em **Registrar**.
- Após registrar, o produto passa a existir no estoque e pode receber os demais ajustes pela aba **Estoque**.
- A quantidade contada no histórico do balanço agora pode ser editada diretamente na linha do item, para corrigir erro de contagem.
- A confirmação do balanço bloqueia caso ainda existam itens marcados como **Não cadastrado**, evitando atualização incorreta do estoque.

Arquivos principais alterados:

- `controle_separacao/core.py`
- `templates/balanco_detalhe.html`
