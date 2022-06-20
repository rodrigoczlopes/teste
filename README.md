# Adonis API application

This is the boilerplate for creating an API server in AdonisJs, it comes pre-configured with.

1. Bodyparser
2. Authentication
3. CORS
4. Lucid ORM
5. Migrations and seeds

## Setup

Use the adonis command to install the blueprint

```bash
adonis new yardstick --api-only
```

or manually clone the repo and then run `npm install`.


### Migrations

Run the following command to run startup migrations.

```js
adonis migration:run
```

### Todo
- Style guides
- Validations

## About The System
- Sistema para acompanhamento das Avaliações de Desempenho da Unimed Varginha
  #### Requisitos Funcionais
  - Cadastro de empresa (Unimeds)
  - Cadastro de usuários (Colaboradores)
  - Cadastro de Trajetória/Complexidade
  - Cadastro de Cargos
  - Cadastro de Áreas
  - Cadastro de Email
  - Cadastro de Hierarquias
  - Cadastro de Competências
  - Cadastro de Comportamentos
  - Cadastro de Planos de Desenvolvimento
  - Cadastro de Ciclo ou Período de avaliação
  - Geração de relatório da avaliação individual
  - Geração de relatório da avaliação por setor
  - Geração de relatório da avaliação por gerência
  #### Requisitos Não Funcionais
  - Utilizar o Banco de Dados SQL Server
  - Utilizar a hospedagem da Umbler
  - Utilizar um serviço de Mensageria (Redis ou Kafka)
  - Utilizar AdonisJS
  - Utilizar um Framework de Gráficos (definir)
  #### Regras de Negócio
  - Somente Superiores tem acesso às avaliações dos subordinados
  - Cada Funcionário faz a sua avaliação e o superior faz uma contra avaliação para que se faça o confronto das duas avaliações
  - O administrador cria um periodo de avaliações com data inicial e final
  - Todas as avaliações devem ter um campo de justificativa como campo obrigatório
  - Sempre que um período de avaliação começar deve ser enviado um e-mail para todos informando sobre o preenchimento e a data limite para preenchimento
  - O gestores terão duas áreas para acesso, uma onde estará listado todos os seus subordinados e outra onde ele irá responder a sua avaliação
  - O administrador deve selecionar os comportamentos que cada competência terá
  - O administrador deve selecionar as competências em que cada área será avaliada
  



  