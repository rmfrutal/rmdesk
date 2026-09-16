# RMDesk

RMDesk é o programa de acesso remoto da **RM Informática**, usado para atender
os clientes da casa. Ele é uma versão modificada do
[RustDesk](https://github.com/rustdesk/rustdesk), distribuída sob a mesma
licença **AGPL-3.0**.

## O que muda em relação ao RustDesk

- O programa se chama RMDesk e usa o ícone da RM Informática.
- Ele fala apenas com o servidor próprio da casa (`rminf.com.br`), com a chave
  pública desse servidor já embutida — quem instala não configura nada.
- Os instaladores de Windows saem com o nome `rmdesk-<versão>-<arquitetura>`.

Todo o resto — a forma de conectar, a criptografia, a transferência de arquivos
— é o RustDesk, e o crédito é do projeto original.

## Como sai o instalador

A montagem é feita pelo próprio GitHub, pelo fluxo `Flutter Tag Build`
(`.github/workflows/flutter-tag.yml`): ao criar uma etiqueta de versão, ele
compila e publica os arquivos em *Releases*.

## Código-fonte

Este repositório é público porque a AGPL-3.0 exige que o código de uma versão
modificada fique disponível para quem usa o programa. O texto da licença está em
`LICENCE`.
