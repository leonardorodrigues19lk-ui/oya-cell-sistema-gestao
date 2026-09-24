# oya-cell-sistema-gestao
Projeto acadêmico de modelagem de um sistema de gestão de informações para a Oya Cell, com foco na organização de pedidos, clientes, produtos e controle de estoque.

---

## Metadados

- **Nome dos alunos e RGM:**
  - Leonardo Oliveira Rodrigues — 47569590 
  - Nome do integrante — RGM
  - Nome do integrante — RGM

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

Para comprovar a existência da organização e a realização da pesquisa de campo, foram coletadas as seguintes informações:

- **Endereço:** Rua Barão de Duplat, 389
- **Telefone/Contato:** (11) 98387-1006
- **Localização:** [Google Maps](https://maps.app.goo.gl/D424JzgShK8uoQkv9)
- **Nome e função do responsável entrevistado:** A preencher
- **Data da entrevista:** 19/09/2026
- **Fotos da fachada:** Disponibilizadas na pasta `Evidencias` deste repositório.

As informações utilizadas no desenvolvimento do projeto foram obtidas por meio de pesquisa de campo e entrevista com a organização.

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
