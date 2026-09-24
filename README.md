# oya-cell-sistema-gestao
Projeto acadêmico de modelagem de um sistema de gestão de informações para a Oya Cell, com foco na organização de pedidos, clientes, produtos e controle de estoque.

---

## Metadados

- **Nome dos alunos e RGM:**
  - Leonardo Oliveira Rodrigues — 47569590 
  - Lucas Gabriel Roman Martins  - 46847618
  - Gabriel Arnaldo Da Silva - 47480441
  - Emily Mayara Matos Moreira - 47323523
  - Kauã Gomes da Silva - 47262265

---

## 1. Caracterização da Organização

### Nome e natureza da organização

A Oya Cell é uma empresa fornecedora de acessórios e componentes para celulares, atendendo principalmente outras empresas. Entre os produtos comercializados estão telas, displays, placas-mãe, carcaças, tampas traseiras, capinhas, películas, fones e carregadores.

### Contexto e porte

A organização possui aproximadamente 7 funcionários e realiza uma média de 25 atendimentos por dia. Os clientes podem realizar pedidos presencialmente no balcão, por telefone ou pelo WhatsApp.

### Problemas e necessidades identificados

Durante o levantamento de informações foram identificadas dificuldades relacionadas principalmente à organização dos pedidos e ao controle de estoque.

Atualmente, a empresa não possui um processo totalmente estruturado para o cadastro e controle dos produtos. Em algumas situações, a quantidade disponível de determinado produto é verificada por meio de contagem informal no momento do atendimento.

Também foi identificada a necessidade de melhorar o registro das entradas e saídas de produtos, permitindo maior controle sobre a quantidade disponível em estoque.

### Justificativa da escolha

A Oya Cell foi escolhida devido à facilidade de acesso do grupo à organização e aos responsáveis pelo estabelecimento. Essa proximidade possibilita a realização de pesquisa de campo, entrevistas e coleta de informações sobre os processos reais da empresa.

Além disso, os problemas relacionados à organização dos pedidos e ao controle de estoque tornam a empresa um caso adequado para o desenvolvimento de um modelo de sistema de gestão de informações.

### Evidências da organização

- **Endereço:** Rua Barão de Duplat, 389
- **Contato:** (11) 98387-1006
- **Data da entrevista:** 19/09
- **Nome e função do responsável entrevistado:** A preencher

#### Registro da visita de campo

A imagem abaixo registra a visita realizada pelo grupo à Oya Cell durante o levantamento de informações para o projeto.

![Visita de campo à Oya Cell](Evidencias/visita_oya_cell.jpg)

---

## 2. Processos de Negócio

### Principais processos mapeados

A partir da pesquisa de campo realizada na Oya Cell, foram identificados como processos relevantes para a modelagem do sistema o processamento de pedidos, o controle de estoque e o tratamento de cancelamentos.

#### Processo de Pedido

O processo inicia quando o cliente solicita produtos pelo balcão, telefone ou WhatsApp. O atendente recebe a solicitação, identifica os produtos e suas respectivas quantidades e registra o pedido. Após a definição dos itens e do valor total, é realizado o pagamento. Com o pagamento confirmado, os produtos são separados e o pedido segue para retirada no balcão ou entrega.

#### Processo de Estoque

O controle de estoque envolve entradas e saídas de produtos. As entradas ocorrem com o recebimento de novas mercadorias, enquanto as saídas estão relacionadas principalmente aos produtos vendidos nos pedidos. O sistema proposto deverá registrar essas movimentações para permitir maior controle da quantidade disponível.

#### Processo de Cancelamento

O processo de cancelamento verifica inicialmente a situação do pagamento e o estágio em que o pedido se encontra. As condições de cancelamento e estorno são aplicadas de acordo com as regras operacionais definidas pela organização.

### Fluxogramas

Os fluxogramas dos processos mapeados encontram-se na pasta `Fluxogramas` deste repositório. 

### Fluxograma do Processo de Estoque

O fluxograma representa o processo proposto para controle das entradas e saídas de produtos da Oya Cell. O processo foi modelado considerando as dificuldades identificadas durante a pesquisa de campo, principalmente a ausência de um registro estruturado da entrada de mercadorias e a utilização de contagem informal para verificar determinadas quantidades disponíveis.

![Fluxograma do Processo de Estoque](Fluxogramas/Fluxograma_Estoque_Oya_Cell.png)

---

## 3. Requisitos do Sistema

### 3.1 Requisitos Funcionais

- **RF01 — Cadastrar clientes:** O sistema deve permitir cadastrar clientes com suas informações de identificação e contato.

- **RF02 — Cadastrar produtos:** O sistema deve permitir cadastrar produtos contendo código, descrição, categoria, preço e quantidade disponível.

- **RF03 — Registrar pedidos:** O sistema deve permitir registrar pedidos realizados pelos clientes.

- **RF04 — Adicionar produtos ao pedido:** O sistema deve permitir adicionar um ou vários produtos a um pedido, informando a quantidade de cada item.

- **RF05 — Calcular valor do pedido:** O sistema deve calcular o valor total do pedido com base nos produtos e quantidades informados.

- **RF06 — Registrar pagamentos:** O sistema deve permitir registrar pagamentos associados aos pedidos.

- **RF07 — Registrar forma de pagamento:** O sistema deve permitir identificar a forma de pagamento utilizada, como PIX, cartão de débito, cartão de crédito ou boleto.

- **RF08 — Controlar status do pedido:** O sistema deve permitir atualizar e consultar o status de cada pedido.

- **RF09 — Controlar estoque:** O sistema deve atualizar a quantidade disponível dos produtos de acordo com suas entradas e saídas.

- **RF10 — Registrar entrada de mercadorias:** O sistema deve permitir registrar a entrada de novas unidades de produtos no estoque.

- **RF11 — Registrar saída de produtos:** O sistema deve registrar a saída dos produtos vendidos.

- **RF12 — Registrar funcionário responsável:** O sistema deve identificar os funcionários envolvidos no registro ou processamento dos pedidos.

- **RF13 — Registrar cancelamentos:** O sistema deve permitir registrar o cancelamento de pedidos conforme as regras estabelecidas pela organização.

- **RF14 — Registrar estornos:** O sistema deve permitir registrar os estornos associados a pedidos cancelados.

### 3.2 Requisitos Não Funcionais

- **RNF01 — Usabilidade:** O sistema deve possuir uma interface simples, organizada e de fácil utilização pelos funcionários da Oya Cell.

- **RNF02 — Segurança:** O sistema deve exigir autenticação dos funcionários para acesso às funcionalidades e informações internas.

- **RNF03 — Integridade dos dados:** O sistema deve manter consistência entre pedidos, pagamentos e movimentações de estoque, evitando registros incompatíveis.

- **RNF04 — Desempenho:** O sistema deve permitir consultas de clientes, produtos, pedidos e estoque em tempo adequado para não prejudicar o atendimento.

- **RNF05 — Disponibilidade:** O sistema deve estar disponível durante o horário de funcionamento da organização, exceto em períodos necessários de manutenção.

- **RNF06 — Rastreabilidade:** O sistema deve manter registros das principais operações realizadas, permitindo identificar movimentações de pedidos, pagamentos e estoque.

- **RNF07 — Privacidade:** O sistema deve proteger os dados cadastrais dos clientes, restringindo o acesso às informações às pessoas autorizadas.

## 4. Regras de Negócio

As regras de negócio foram definidas com base nas informações obtidas durante o levantamento realizado na Oya Cell e também nas necessidades identificadas para o sistema proposto.

- **RN01 — Cliente e pedido:** Um cliente pode realizar vários pedidos, enquanto cada pedido deve estar associado a um cliente.

- **RN02 — Produtos do pedido:** Um pedido pode possuir vários produtos, e um mesmo produto pode estar presente em diferentes pedidos.

- **RN03 — Quantidade do item:** Para cada produto incluído em um pedido deve ser registrada a quantidade solicitada.

- **RN04 — Valor do pedido:** O valor total do pedido deve ser determinado a partir dos produtos, das quantidades e dos valores registrados no pedido.

- **RN05 — Pagamento:** Todo pagamento deve estar associado a um pedido.

- **RN06 — Múltiplos pagamentos:** Um pedido pode possuir mais de um pagamento associado.

- **RN07 — Forma de pagamento:** Os pagamentos podem ser realizados por PIX, cartão de débito, cartão de crédito ou boleto.

- **RN08 — Liberação do pedido:** O pedido deve ser liberado para retirada ou entrega após a confirmação do pagamento.

- **RN09 — Funcionários e pedidos:** Um funcionário pode participar de vários pedidos, e um pedido pode possuir a participação de mais de um funcionário.

- **RN10 — Saída de estoque:** A venda de um produto deve gerar uma saída de estoque correspondente à quantidade vendida.

- **RN11 — Entrada de estoque:** O recebimento de novas mercadorias deve gerar um registro de entrada no estoque.

- **RN12 — Movimentação de estoque:** Toda movimentação de estoque deve identificar o produto, o tipo de movimentação, a quantidade e a data da movimentação.

- **RN13 — Quantidade disponível:** A quantidade disponível de um produto deve ser atualizada de acordo com suas entradas e saídas.

- **RN14 — Forma de recebimento:** O pedido pode ser retirado no balcão ou encaminhado para entrega.

- **RN15 — Finalização no balcão:** O pedido retirado e entregue ao cliente no balcão deve ser marcado como finalizado.

- **RN16 — Status do pedido:** O pedido deve possuir um status que represente sua situação durante o processo, como em separação, saiu para entrega, finalizado ou cancelado.

- **RN17 — Cancelamento antes da saída:** Caso o pedido já tenha sido pago, mas ainda não tenha saído da loja, o cancelamento poderá ser realizado com estorno integral do valor pago.

- **RN18 — Cancelamento após a saída:** Caso o cancelamento seja permitido após o pedido ter saído da loja, o cliente receberá o estorno correspondente a 60% do valor pago.
