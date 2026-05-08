# Filtro por linha no relatório de Estoque Geral

A aba **Relatórios > Estoque geral por linhas** agora tem um campo **Filtrar por linha**.

## O que mudou

- Adicionado seletor com todas as linhas existentes no estoque.
- Ao selecionar uma linha, os cards de resumo passam a calcular somente aquela linha.
- A tabela abaixo também exibe somente a linha filtrada.
- O botão **Limpar filtro** volta para a visualização de todas as linhas.
- A exportação em Excel respeita o filtro selecionado e registra a linha filtrada no arquivo.

## Arquivos alterados

- `controle_separacao/core.py`
- `templates/relatorios.html`
