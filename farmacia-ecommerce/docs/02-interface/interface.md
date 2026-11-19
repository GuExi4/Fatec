# Etapa 2 – Interface

Protótipo navegável (11 telas, botão Play): https://claude.ai/artifact/ULhhFXxL87yh7Xgs5MimDk
Fontes das telas (formato do canvas Claude Design): [prototipo/](prototipo/). Todas as telas exibem o nome FarmaOn e a marca do Grupo Wise.

| Tela | Objetivo | Casos de uso |
|---|---|---|
| T1 Início | Busca, banner de receita, categorias, recompra | UC01, UC10 |
| T2 Resultado da busca | Filtros e selos de receita | UC01 |
| T3 Detalhe do produto | Preço, ANVISA, quantidade, aviso de receita, chat | UC01, UC04, UC13 |
| T4 Carrinho | Itens, remover com desfazer, CEP | UC04, UC06 |
| T5 Entrar | E-mail e senha, recuperação, bloqueio após 5 tentativas | UC03 |
| T6 Criar conta | Validação em linha (CPF), aceite LGPD, idade mínima | UC02 |
| T7 Entrega e pagamento | Endereço, frete, PIX/cartão, cupom | UC05–UC07, UC09 |
| T8 Receita médica | Upload e checklist | UC08 |
| T9 Pedido realizado | Número e próximos passos | UC05 |
| T10 Acompanhar pedido | Linha do tempo, parecer, cancelar | UC10, UC11 |
| T11 Validação de receitas | Fila, checklist, aprovar/rejeitar | UC12 |

Navegação: T1 → T2 → T3 → T4 → T5 (ou T6) → T7 → T8 → T9 → T10; barra inferior (Início, Busca, Carrinho, Pedidos) nas telas de navegação; checkout com indicador de 4 etapas.

## Heurísticas de Nielsen
1. Visibilidade do status: indicador de etapas, linha do tempo, contador do carrinho.
2. Mundo real: genérico, tarja, princípio ativo, bula, receita.
3. Controle e liberdade: Desfazer, Voltar, cancelar pedido.
4. Consistência: mesma barra, mesma cor de ação, mesmos selos.
5. Prevenção de erros: selo “Exige receita”, controlados sem botão Comprar, limite de estoque, “Criar conta” só após aceite LGPD.
6. Reconhecer em vez de lembrar: endereço, cartão e receitas salvos; recompra.
7. Flexibilidade: busca por nome, princípio ativo ou marca; filtros rápidos.
8. Minimalismo: uma ação primária por tela.
9. Recuperação de erros: validação de CPF em linha no cadastro, mensagens no upload, parecer da receita.
10. Ajuda: checklist de foto, chat com farmacêutico, próximos passos.
