# Teste de aplicativo web — Urban Routes

Projeto da Sprint 3 do curso de QA Engineer da TripleTen: teste da interface web do **Urban Routes**, um serviço que cria rotas para vários tipos de transporte, com checklists, casos de teste e relatórios de bug no Jira.

## Objetivo

Verificar se o layout e a lógica do Urban Routes seguem os requisitos: tela inicial, modos de transporte, mapa, tarifas, método de pagamento, botão "Reservar" e reserva de carro.

## O que foi feito

- **Checklist do layout** (19 verificações), testado no Google Chrome (800x600) e no Firefox (1920x1080): estado inicial do formulário, modo Personal, mapa e tarifa Casual.
- **Checklist das janelas "Método de pagamento" e "Adicionar cartão"** (27 verificações): campos Número e Código, com classes de equivalência e valores limite (por exemplo: código 00, 01, 99 e 100; número com menos e mais de 12 dígitos).
- **Casos de teste para o botão "Reservar"** (5 casos): combinações com e sem carteira de motorista, cartão e endereços.
- **Casos de teste para a reserva do carro** (3 casos): reserva, cancelamento e não cancelamento.
- **22 relatórios de bug** registrados no Jira, ligados a cada verificação reprovada.

## Resultados

| Parte | Total | Aprovados | Reprovados | Bloqueados |
|---|---|---|---|---|
| Checklist do layout | 19 | 12 | 7 | 0 |
| Checklist de pagamento | 27 | 16 | 11 | 0 |
| Casos de teste do botão "Reservar" | 5 | 1 | 3 | 1 |
| Casos de teste da reserva | 3 | 1 | 1 | 1 |

### Exemplos de bugs encontrados

- Ao adicionar um cartão, a interface não mostra os últimos 4 dígitos do número.
- O campo Código aceita os valores inválidos 00 e 100.
- O campo Número aceita mais de 12 dígitos e símbolos fora dos requisitos.
- O botão "Adicionar" fica habilitado com número ou código inválido.
- O cancelamento da reserva não funciona.
- A rota não aparece no mapa com os nomes dos endereços "De" e "Para".

## Arquivos

- [`checklists-e-casos-de-teste-urban-routes.xlsx`](checklists-e-casos-de-teste-urban-routes.xlsx): planilha com quatro abas:
  1. Checklist do layout
  2. Checklist para "Método de pagamento" e "Adicionar cartão"
  3. Casos de teste para o botão "Reservar"
  4. Casos de teste para a locação (reserva do carro)

Cada item reprovado tem o link para o relatório de bug no Jira.

## O que aprendi

- **Teste de interface de usuário:** verificar layout e lógica da interface web em navegadores e resoluções diferentes, com checklists e casos de teste.
- **Rastreamento de bugs:** ligar cada verificação reprovada ao seu relatório de bug, com etapas para reprodução, resultado esperado e resultado real.
- **Jira:** registrar e organizar os 22 bugs encontrados.
- **Classes de equivalência e valores limite:** aplicar as técnicas de design de teste em campos reais, como número e código do cartão.
