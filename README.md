# Changelog e Release com GitHub Actions

**Trabalho 1 de DevOps Avançado — UniALFA**

## Integrante
- Arthur Antunes de Oliveira — RA: 250314

## Sobre o projeto
Esse projeto mostra como usar o GitHub Actions para registrar mudanças e criar versões automaticamente. Ele tem uma página HTML simples e duas automações.

## Action de Changelog (`changelog.yml`)
Sempre que tem um push na branch `main`, a Action pega os commits do Git e atualiza o changelog deste README, mostrando o hash, a mensagem, o autor e a data de cada alteração.

Depois, ela salva a atualização do README com um novo commit.

## Action de Release (`release.yml`)
A cada push na branch `main`, a Action cria uma nova versão no formato `v1.0.N`, gera uma tag, compacta o projeto em `pacote.zip` e publica tudo na área de Releases do GitHub, com notas automáticas.

Assim, não precisa criar as versões manualmente.

## Changelog

<!-- CHANGELOG:START -->
<!-- CHANGELOG:END -->