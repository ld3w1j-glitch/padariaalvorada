# Importação de PDF padrão

Esta versão adiciona a seção **Importar PDF** no menu do sistema.

## O que foi implementado

- Upload de arquivo `.pdf` textual.
- Leitura automática do texto do PDF usando `pypdf`.
- Tentativa de identificação de campos como Pedido, Loja/Cliente e Data.
- Detecção automática de itens em linhas no padrão: código + descrição + quantidade.
- Tela de prévia com campos editáveis.
- Confirmação ao clicar em um campo: 👍 para liberar edição, 👎 para cancelar.
- Botão para adicionar/remover itens manualmente.
- Exportação da prévia para Excel.
- Criação de separação/lote a partir dos itens revisados.

## Dependência nova

Foi adicionada ao `requirements.txt`:

```txt
pypdf>=4,<6
```

Depois de atualizar o projeto, rode:

```bash
pip install -r requirements.txt
```

## Observação importante

Se o PDF for escaneado como imagem, sem texto selecionável, o sistema não conseguirá ler os campos automaticamente. Nesse caso, será necessário usar um PDF textual ou adicionar OCR no futuro.
