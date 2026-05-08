# Resetar sistema mantendo apenas o admin

Foi adicionada em **Configurações** uma área chamada **Resetar sistema**.

## O que faz

Ao confirmar com a senha do admin e digitando `RESETAR`, o sistema:

- limpa estoque, movimentações, separações, balanços, recebimentos, receitas, ordens de produção, chats, tarefas, anotações e históricos operacionais;
- remove todos os usuários comuns;
- mantém apenas o admin atual ativo;
- recria as configurações básicas do sistema;
- recria as lojas padrão `Loja 1` até `Loja 20` e `CD` para o sistema continuar funcional;
- desconecta o usuário para entrar novamente com o admin.

## Segurança

A ação só aparece/funciona para admin e exige:

1. senha atual do admin;
2. confirmação escrita `RESETAR`;
3. confirmação do navegador antes de enviar.

Esta ação não pode ser desfeita sem backup do banco `dados.db`.
