# Controle manual de permissões por usuário

Esta versão altera a tela de Usuários para que o cargo não marque permissões automaticamente.

## O que mudou

- O campo Cargo continua existindo para organização do usuário.
- As permissões de acesso agora obedecem ao que for marcado manualmente na tela.
- Gerente, Desenvolvedor e Supervisor podem receber acesso amplo, mas somente se o admin marcar os módulos desejados.
- Áreas sensíveis continuam exclusivas do cargo Admin:
  - Usuários
  - Configurações
  - Código fonte
  - Auditoria
- O cargo Admin continua recebendo acesso total automaticamente.

## Botões adicionados

Na criação e edição de usuários foram adicionados três botões auxiliares:

- **Aplicar padrão do cargo**: marca uma sugestão padrão para aquele cargo.
- **Marcar todos operacionais**: marca todos os módulos não sensíveis.
- **Limpar acessos**: desmarca todos os acessos operacionais.

Esses botões não são obrigatórios. Eles apenas ajudam a preencher mais rápido; depois você pode marcar ou desmarcar manualmente.
