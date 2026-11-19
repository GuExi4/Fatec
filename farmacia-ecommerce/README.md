<p align="center"><img src="assets/logo/grupo-wise-logo.svg" alt="Grupo Wise" width="360"></p>

# FarmaOn – E-commerce de farmácia (Exercício 12)

Trabalho do **Grupo Wise**. Modelagem completa de um e-commerce para farmácia com loja física: requisitos, interface, gestão de configuração, Scrum, projeto (UML) e teste.

**Equipe (Grupo Wise):** [Integrante 1 – PO] · [Integrante 2 – Scrum Master] · [Integrante 3 – Dev back-end] · [Integrante 4 – Dev front-end]
**Entrega:** 19/11/2026 · **Professor (acesso de leitura):** AndersonLuizBarbosa

## Navegação

| Etapa | Conteúdo | Onde |
|---|---|---|
| 1 – Requisitos | Atores, RF, RNF, regras de negócio, diagrama e narrativas de casos de uso | [docs/01-requisitos](docs/01-requisitos/requisitos.md) · [diagrama](diagramas/img/casos-de-uso.png) |
| 2 – Interface | 11 telas navegáveis + heurísticas de Nielsen | [docs/02-interface](docs/02-interface/interface.md) · [fontes do protótipo](docs/02-interface/prototipo) |
| 3 – GCS | Estrutura, branches, convenções, baselines | [docs/03-gcs](docs/03-gcs/plano-gcs.md) · [CONTRIBUTING](CONTRIBUTING.md) |
| 4 – Scrum | Backlog, sprint 1, execução simulada, burndown | [planilha](docs/04-scrum/FarmaOn_Scrum_Backlog_Sprint1_Burndown.xlsx) · [burndown](diagramas/img/burndown-sprint1.png) |
| 5 – Projeto | Classes, sequência (checkout), máquina de estados (pedido) | [docs/05-projeto](docs/05-projeto/projeto.md) · [diagramas/img](diagramas/img) |
| 6 – Teste | Plano de teste, 40 casos, rastreabilidade | [planilha](docs/06-teste/FarmaOn_Plano_e_Casos_de_Teste.xlsx) |
| Apresentação | 16 slides, 15 minutos | [docs/07-apresentacao](docs/07-apresentacao) |

**Documento consolidado:** [Word](docs/Exercicio12_FarmaOn.docx) · [PDF](docs/Exercicio12_FarmaOn.pdf)

Versões on-line (privadas até serem compartilhadas pela equipe):
- Documento: https://claude.ai/artifact/9RNvYwqN1vqNuazWnVCgSN
- Protótipo: https://claude.ai/artifact/ULhhFXxL87yh7Xgs5MimDk
- Apresentação: https://claude.ai/artifact/KbBbctJWHG8PsnpAARe3QR

## Diagramas

As fontes estão em `diagramas/src/*.puml` (PlantUML). Para regerar:

```bash
java -jar plantuml.jar -tpng -o ../img diagramas/src/*.puml
```

No Draw.io: Organizar › Inserir › Avançado › PlantUML e cole o conteúdo do `.puml`.

## Publicar este repositório

```bash
cd farmacia-ecommerce
git init -b main
git add .
git commit -m "docs: modelagem inicial do FarmaOn (etapas 1 a 6)"
gh repo create farmacia-ecommerce --private --source=. --push
git checkout -b develop && git push -u origin develop
for t in v0.1.0 v0.2.0 v0.3.0 v0.4.0 v0.5.0 v0.6.0 v0.6.1; do git tag -a $t -m "Baseline $t"; done
git push origin --tags
gh api -X PUT repos/{owner}/farmacia-ecommerce/collaborators/AndersonLuizBarbosa -f permission=pull
```

Sem o `gh`: crie o repositório em github.com/new, faça `git remote add origin <url>` e `git push -u origin main`, e adicione o professor em Settings › Collaborators › Add people.
