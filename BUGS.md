# Relatórios de bug — Urban Routes (Sprint 3)

Os 22 bugs abaixo foram registrados no Jira durante o teste do app web Urban Routes. Como o Jira do projeto é privado, eles foram copiados para cá para que qualquer pessoa possa ler os relatórios.

Os IDs (S3-1 a S3-22) são os mesmos que aparecem na coluna "Link para o relatório de bug" da planilha.

## Resumo

| ID | Título | Área | Prioridade |
|---|---|---|---|
| [S3-1](#s3-1) | Não exibe os últimos dígitos do cartão. | Método de pagamento / Adicionar cartão | Média |
| [S3-2](#s3-2) | Não deixa adicionar o cartão. | Método de pagamento / Adicionar cartão | Média |
| [S3-3](#s3-3) | Não deixa adicionar o cartão. | Método de pagamento / Adicionar cartão | Média |
| [S3-4](#s3-4) | Os espaços não são inseridos automaticamente quando o usuário insere o número e clica fora do campo. | Método de pagamento / Adicionar cartão | Média |
| [S3-5](#s3-5) | É possível inserir mais de 12 símbolos | Método de pagamento / Adicionar cartão | Média |
| [S3-6](#s3-6) | O sistema permite inserir outros símbolos ou números que não estejam conforme os requisitos. | Método de pagamento / Adicionar cartão | Média |
| [S3-7](#s3-7) | É possível digitar 00 no código. | Método de pagamento / Adicionar cartão | Média |
| [S3-8](#s3-8) | É possível digitar 100 no código ou código com 3 dígitos. | Método de pagamento / Adicionar cartão | Média |
| [S3-9](#s3-9) | Ao digitar um valor inválido no campo número e código o botão adicionar é habilitado. | Método de pagamento / Adicionar cartão | Média |
| [S3-10](#s3-10) | Ao digitar um valor inválido no campo número e um valor válido no código o botão adicionar é habilitado. | Método de pagamento / Adicionar cartão | Média |
| [S3-11](#s3-11) | Ao digitar um valor válido no campo número e um valor inválido no código o botão adicionar é habilitado. | Método de pagamento / Adicionar cartão | Média |
| [S3-12](#s3-12) | Aparece carro reservado, espera gratuita | Botão "Reservar" | Média |
| [S3-13](#s3-13) | A janela "Carteira de motorista adicionada" não aparece. | Botão "Reservar" | Média |
| [S3-14](#s3-14) | É possível clicar no botão de reservar | Botão "Reservar" | Média |
| [S3-15](#s3-15) | Ao clicar no botão Cancelar ele não executa nenhuma ação. | Reserva do carro | Média |
| [S3-16](#s3-16) | A palavra PLATAFORMA está escrita de maneira incorreta. | Layout | Média |
| [S3-17](#s3-17) | Ao selecionar o modo Personal exibe a frase "Carsharing ~$x Duração : x min esta escrito incorreto | Layout | Média |
| [S3-18](#s3-18) | O botão reservar está menor de acordo com o FIGMA | Layout | Média |
| [S3-19](#s3-19) | Ao digitar os endereços DE e PARA é exibido no mapa a rota com o nome dos endereços DE e PARA incorretos | Layout | Média |
| [S3-20](#s3-20) | Ao selecionar a tarifa CASUAL não é exibido carrinhos azuis | Layout | Média |
| [S3-21](#s3-21) | Descrição de tempo e espera gratuita incorretos | Layout | Média |
| [S3-22](#s3-22) | Imagem do carro faltando acessórios | Layout | Média |

---

<a id="s3-1"></a>

## S3-1 — Não exibe os últimos dígitos do cartão.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código
8. Clicar no botão Adicionar

**Resultado esperado:** Deve exibir os 4 últimos dígitos do cartão.

**Resultado real:** Não exibe os últimos dígitos do cartão.

**Evidências no Jira:** Chrome.png, Figma.png

---

<a id="s3-2"></a>

## S3-2 — Não deixa adicionar o cartão.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar 0000
8. Clicar no botão Adicionar

**Resultado esperado:** Deve restringir o uso de 0000

**Resultado real:** Não deixa adicionar o cartão.

**Evidências no Jira:** Chrome 0000.png, Figma 2.png

---

<a id="s3-3"></a>

## S3-3 — Não deixa adicionar o cartão.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar 0000
8. Clicar no botão Adicionar

**Resultado esperado:** Deve restringir o uso de 9999

**Resultado real:** Não deixa adicionar o cartão.

**Evidências no Jira:** Chrome 9999.png, Figma 2.png

---

<a id="s3-4"></a>

## S3-4 — Os espaços não são inseridos automaticamente quando o usuário insere o número e clica fora do campo.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código
8. Clicar no botão Adicionar

**Resultado esperado:** Os espaços devem ser inseridos automaticamente quando o usuário insere o número e clica fora do campo

**Resultado real:** Os espaços não são inseridos automaticamente quando o usuário insere o número e clica fora do campo.

**Evidências no Jira:** Chrome .png, Figma.png

---

<a id="s3-5"></a>

## S3-5 — É possível inserir mais de 12 símbolos

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código
8. Clicar no botão Adicionar

**Resultado esperado:** É impossível inserir mais de 12 símbolos.

**Resultado real:** É possível inserir mais de 12 símbolos.

**Evidências no Jira:** Chrome.png

---

<a id="s3-6"></a>

## S3-6 — O sistema permite inserir outros símbolos ou números que não estejam conforme os requisitos.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código
8. Clicar no botão Adicionar

**Resultado esperado:** O sistema não permite inserir outros símbolos ou números que não estejam conforme os requisitos.

**Resultado real:** O sistema permite inserir outros símbolos ou números que não estejam conforme os requisitos.

**Evidências no Jira:** Chrome.png

---

<a id="s3-7"></a>

## S3-7 — É possível digitar 00 no código.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código 00
8. Clicar no botão Adicionar

**Resultado esperado:** Não é possível digitar 00 no código.

**Resultado real:** É possível digitar 00 no código.

**Evidências no Jira:** Chrome - 00.png

---

<a id="s3-8"></a>

## S3-8 — É possível digitar 100 no código ou código com 3 dígitos.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código com três dígitos.
8. Clicar no botão Adicionar

**Resultado esperado:** Não é possível digitar 100 no código ou código com 3 dígitos.

**Resultado real:** É possível digitar 100 no código ou código com 3 dígitos.

**Evidências no Jira:** Chrome -100.png

---

<a id="s3-9"></a>

## S3-9 — Ao digitar um valor inválido no campo número e código o botão adicionar é habilitado.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código
8. Clicar no botão Adicionar

**Resultado esperado:** Ao digitar um valor inválido no campo número e código o botão adicionar não é habilitado.

**Resultado real:** Ao digitar um valor inválido no campo número e código o botão adicionar é habilitado.

**Evidências no Jira:** Chrome.png

---

<a id="s3-10"></a>

## S3-10 — Ao digitar um valor inválido no campo número e um valor válido no código o botão adicionar é habilitado.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código
8. Clicar no botão Adicionar

**Resultado esperado:** Ao digitar um valor inválido no campo número e um valor válido no código o botão adicionar não é habilitado.

**Resultado real:** Ao digitar um valor inválido no campo número e um valor válido no código o botão adicionar é habilitado.

**Evidências no Jira:** Chrome -codigo.png

---

<a id="s3-11"></a>

## S3-11 — Ao digitar um valor válido no campo número e um valor inválido no código o botão adicionar é habilitado.

- **Área:** Método de pagamento / Adicionar cartão
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em método de Pagamento
6. Clicar em Adicionar cartão
7. Digitar número e código
8. Clicar no botão Adicionar

**Resultado esperado:** Ao digitar um valor válido no campo número e um valor inválido no código o botão adicionar não é habilitado.

**Resultado real:** Ao digitar um valor válido no campo número e um valor inválido no código o botão adicionar é habilitado.

**Evidências no Jira:** Chrome - codigo valido.png

---

<a id="s3-12"></a>

## S3-12 — Aparece carro reservado, espera gratuita

- **Área:** Botão "Reservar"
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em carteira de motorista
6. Clicar em reservar

**Resultado esperado:** A janela "Carteira de motorista adicionada" aparece.

**Resultado real:** Aparece carro reservado, espera gratuita.

**Evidências no Jira:** Captura de Tela 2026-03-22 às 23.30.07.png

---

<a id="s3-13"></a>

## S3-13 — A janela "Carteira de motorista adicionada" não aparece.

- **Área:** Botão "Reservar"
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em adicionar cartão
6. Clicar em reservar

**Resultado esperado:** A janela "Carteira de motorista adicionada" aparece.

**Resultado real:** A janela "Carteira de motorista adicionada" não aparece.

**Evidências no Jira:** Captura de Tela 2026-03-22 às 23.56.25.png

---

<a id="s3-14"></a>

## S3-14 — É possível clicar no botão de reservar

- **Área:** Botão "Reservar"
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em adicionar cartão
6. Clicar em reservar

**Resultado esperado:** Não é possível clicar no botão.

**Resultado real:** É possível clicar no botão.

**Evidências no Jira:** Captura de Tela 2026-03-23 às 19.53.59.png

---

<a id="s3-15"></a>

## S3-15 — Ao clicar no botão Cancelar ele não executa nenhuma ação.

- **Área:** Reserva do carro
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Clicar no botão reservar
5. Clicar em adicionar cartão
6. Clicar em reservar
7. Clicar em Cancelar

**Resultado esperado:** Ao clicar no botão Cancelar a corrida é cancelada.

**Resultado real:** Ao clicar no botão Cancelar ele não executa nenhuma ação.

**Evidências no Jira:** Captura de Tela 2026-03-23 às 21.04.17.png, Chrome.png

---

<a id="s3-16"></a>

## S3-16 — A palavra PLATAFORMA está escrita de maneira incorreta.

- **Área:** Layout
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600, Firefox 1920x1080

**Resultado esperado:** Deve exibir a palavra PLATAFORMA

**Resultado real:** Exibe a palavra PLATFORME

**Evidências no Jira:** Chrome.png, Figma.png, FireFox.png

---

<a id="s3-17"></a>

## S3-17 — Ao selecionar o modo Personal exibe a frase "Carsharing ~$x Duração : x min esta escrito incorreto

- **Área:** Layout
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600, Firefox 1920x1080

**Resultado esperado:** Ao selecionar o modo Personal exibe a frase "Carsharing ~$x Duração : x min

**Resultado real:** Ao selecionar o modo Personal exibe a frase "Carsharing ~$x Duração x min.

**Evidências no Jira:** Chrome.png, Figma.png, FireFox.png

---

<a id="s3-18"></a>

## S3-18 — O botão reservar está menor de acordo com o FIGMA

- **Área:** Layout
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600, Firefox 1920x1080

**Resultado esperado:** O botão reservar deve ser do mesmo tamanho de acordo com o Figma

**Resultado real:** O botão reservar aparece menor.

**Evidências no Jira:** Chrome.png, Figma.png, FireFox.png

---

<a id="s3-19"></a>

## S3-19 — Ao digitar os endereços DE e PARA é exibido no mapa a rota com o nome dos endereços DE e PARA incorretos

- **Área:** Layout
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600, Firefox 1920x1080

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal

**Resultado esperado:** Ao digitar os endereços DE e PARA é exibido no mapa a rota com o nome dos endereços DE e PARA

**Resultado real:** Ao digitar os endereços DE e PARA é exibido no mapa a rota com o nome dos endereços DE e PARA incorretos

**Evidências no Jira:** Chrome.png, Figma.png, FireFox.png

---

<a id="s3-20"></a>

## S3-20 — Ao selecionar a tarifa CASUAL não é exibido carrinhos azuis

- **Área:** Layout
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600, Firefox 1920x1080

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Selecionar tarifa CASUAL

**Resultado esperado:** Ao selecionar a tarifa CASUAL carrinhos azuis são exibidos.

**Resultado real:** Ao selecionar a tarifa CASUAL não é exibido carrinhos azuis.

**Evidências no Jira:** Chrome.png, Figma.png, FireFox.png

---

<a id="s3-21"></a>

## S3-21 — Descrição de tempo e espera gratuita incorretos

- **Área:** Layout
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600, Firefox 1920x1080

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Selecionar tarifa CASUAL

**Resultado esperado:** Descrição de tempo e espera gratuita corretos.

**Resultado real:** Descrição de tempo e espera gratuita incorretos.

**Evidências no Jira:** Chrome.png, Figma.png, FireFox.png

---

<a id="s3-22"></a>

## S3-22 — Imagem do carro faltando acessórios

- **Área:** Layout
- **Prioridade:** Média
- **Ambiente:** Google Chrome 800x600, Firefox 1920x1080

**Etapas para reprodução:**

1. Acessar Urban Routes
2. Digitar endereços DE e PARA
3. Selecionar modo Personal
4. Selecionar tarifa CASUAL

**Resultado esperado:** Imagem do carro com acessórios

**Resultado real:** Imagem do carro faltando acessórios

**Evidências no Jira:** Chrome.png, Figma.png, FireFox.png
