# Como contribuir

## Branches
- `main`: somente versões entregues (baselines). Protegida.
- `develop`: integração. Protegida; merge por PR com 1 aprovação e CI verde.
- `feature/<US>-<descricao>`: sai de `develop` (ex.: `feature/US05-carrinho`).
- `release/<versao>`: preparação de entrega; merge em `main` + tag.
- `hotfix/<versao>`: correção urgente a partir de `main`; volta para `main` e `develop`.

## Commits (Conventional Commits)
`feat:` · `fix:` · `docs:` · `test:` · `refactor:` · `chore:` — cite a issue: `docs(requisitos): narrativa UC12 #10`.

## Fluxo de mudança
1. Toda mudança nasce de uma issue (história, bug ou solicitação de mudança).
2. Crie a branch a partir de `develop`.
3. Abra o PR usando o template; outro integrante revisa.
4. Após o merge, atualize o `CHANGELOG.md`.

## Versionamento
SemVer `MAJOR.MINOR.PATCH`. Documentação em `0.x` até o primeiro release do sistema (`1.0.0`).
