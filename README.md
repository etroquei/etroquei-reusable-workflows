# Workflows Reutilizáveis

Este repositório contém workflows GitHub Actions reutilizáveis para facilitar processos comuns de integração contínua (CI), build, deploy, criação de pull requests e releases automatizadas.

## Conteúdo

* CI: Workflows para validação de código, testes automatizados e cobertura de código.

* Build: Workflows que automatizam a criação e empacotamento de aplicações.

* Deploy: Workflows que realizam deploy automático para diferentes ambientes (desenvolvimento, staging e produção).

* Pull Requests: Workflows que automatizam a criação e gerenciamento de pull requests.

* Releases: Workflows para criação e publicação automatizada de releases.

## Como Usar

Para utilizar os workflows deste repositório, importe-os no seu projeto GitHub Actions com a sintaxe:

```yaml
jobs:
  ci:
    uses: etroquei/github-workflows/.github/workflows/ci-workflow.yml@main # ou @v1.0.0
    with:
      node-version: '18.x'
      fetch-depth: 1
      use-cache: true
```

## Estrutura

```bash
.github/
└── workflows/
    ├── ci-workflow.yml
    ├── build-workflow.yml
    ├── deploy-workflow.yml
    ├── open-pr-workflow.yml
    └── release-workflow.yml
```

## Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork deste repositório.
2. Crie uma nova branch (git checkout -b feature/nome-da-feature).
3. Faça suas alterações e commit (git commit -m 'feat: descrição da feature').
4. Envie suas alterações (git push origin nome-da-feature).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo LICENSE para mais detalhes.
