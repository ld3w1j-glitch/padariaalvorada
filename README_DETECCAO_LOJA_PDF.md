# Detecção automática de loja no PDF

Esta versão adiciona a identificação automática da loja na importação de PDF.

## O que foi alterado

- A tela **Importar PDF** agora tenta identificar a loja pelo CNPJ ou pela razão social/apelido encontrado no cabeçalho do PDF.
- Exemplo: `MAGLIONI RIBEIRO & CIA LTDA (COM.)` é reconhecido como **Loja 1**.
- Quando a loja é reconhecida, ela já aparece marcada automaticamente na lista de lojas da separação.
- O banco inicial agora garante as lojas **Loja 1** até **Loja 20**, além do **CD**.
- Bancos antigos que tinham apenas as 5 primeiras lojas são completados automaticamente na próxima abertura do sistema.

## Relação usada para detectar a loja

A detecção usa duas bases:

1. CNPJ sem pontuação.
2. Nome/apelido da razão social, como `COM`, `MACHADO`, `GUARDA`, `CESARIO`, `GETULIO`, `ALAGOAS`, `IMIGRANTES`, entre outros.

Se o PDF não tiver nenhuma correspondência, o sistema mantém a importação normal e permite marcar a loja manualmente.
