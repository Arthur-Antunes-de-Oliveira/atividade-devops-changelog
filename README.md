# Changelog e Release com GitHub Actions

Trabalho 1 de DevOps Avançado — UniALFA

## Integrantes

- SEU NOME COMPLETO (RA 000000)

## Sobre o projeto

Repositório que demonstra o uso de GitHub Actions para documentar alterações e publicar versões do projeto. Contém uma página HTML simples e duas automações independentes.

## Action de changelog (`changelog.yml`)

A cada push na branch `main`, a Action lê o histórico do Git (`git log`) e reescreve a seção de changelog deste README, listando cada commit com hash, mensagem, autor e data. A seção fica entre os marcadores `CHANGELOG:START` e `CHANGELOG:END`. Depois, a própria Action faz um commit com o README atualizado.

## Action de release (`release.yml`)

A cada push na branch `main`, a Action gera automaticamente um número de versão (`v1.0.N`, onde N é o número da execução), cria a tag no commit da alteração, empacota o projeto em um arquivo `pacote.zip` e publica a versão na seção Releases do GitHub, com notas de versão geradas automaticamente. Não é necessário criar tags manualmente: cada alteração enviada gera uma nova versão.

## Changelog

<!-- CHANGELOG:START -->
<!-- CHANGELOG:END -->
