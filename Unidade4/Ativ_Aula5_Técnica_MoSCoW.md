# 11_Matriz MoSCoW

| ID | Requisito | M | S | C | W | Justificativa |
|---|---|:---:|:---:|:---:|:---:|---|
| **RF01** | Cadastro de pacientes. | **X** | | | | É necessário para identificar e registrar os pacientes no sistema. |
| **RF02** | Cadastro de médicos. | **X** | | | | Necessário para disponibilizar os médicos para agendamento. |
| **RF03** | Cadastro de especialidades. | **X** | | | | Permite organizar os médicos de acordo com suas especialidades. |
| **RF04** | Consulta de horários disponíveis. | **X** | | | | É essencial para verificar os horários livres e evitar conflitos. |
| **RF05** | Realização de agendamentos. | **X** | | | | É uma das principais funções do sistema. |
| **RF06** | Cancelamento de consultas. | **X** | | | | Necessário para liberar horários e manter a agenda atualizada. |
| **RF07** | Confirmação de consultas. | | **X** | | | É importante para garantir que o paciente tenha conhecimento do agendamento. |
| **RF08** | Envio de lembretes. | | **X** | | | Ajuda a reduzir faltas, mas o sistema pode funcionar sem essa funcionalidade inicialmente. |
| **RF09** | Gerenciamento da agenda dos médicos. | **X** | | | | É necessário para organizar os horários e evitar conflitos de agendamento. |
| **RF10** | Registro de consultas realizadas e faltas. | **X** | | | | Permite controlar o comparecimento dos pacientes e os atendimentos realizados. |
| **RF11** | Acompanhamento de indicadores. | | | **X** | | É importante para auxiliar a direção na análise do desempenho da clínica. |
| **RF12** | Cálculo de consultas realizadas. | | **X** | | | Ajuda no acompanhamento dos atendimentos, mas pode ser implementado após as funções principais. |
| **RF13** | Registro de cancelamentos. | | **X** | | | Permite acompanhar a quantidade de cancelamentos e gerar informações para a gestão. |
| **RF14** | Registro de faltas. | | **X** | | | Permite acompanhar a quantidade de faltas e auxiliar na análise dos indicadores. |
| **RF15** | Cálculo do tempo médio de atendimento e taxa de ocupação. | | | **X** | | É útil para a gestão da clínica, mas pode ser implementado em uma versão posterior. |
| **RQ01** | O sistema deve possuir controle de acesso por usuário. | **X** | | | | É necessário para proteger as informações e limitar o acesso às funções. |
| **RQ02** | O sistema deve manter os dados dos pacientes armazenados de forma segura. | **X** | | | | Os dados dos pacientes precisam ser protegidos. |
| **RQ03** | O sistema deve atualizar a agenda em tempo real. | **X** | | | | É fundamental para evitar conflitos entre agendamentos. |
| **RQ04** | O sistema deve realizar backups periódicos dos dados. | | **X** | | | É importante para recuperação das informações em caso de falha. |
| **RQ05** | O sistema deve apresentar uma interface personalizável para cada usuário. | | | **X** | | Pode melhorar a experiência, mas não é necessária para o funcionamento principal. |

# 12. Definindo a primeira versão

## Parte A - 5 requisitos indispensáveis

| Ordem | ID | Requisito | Por que precisa permanecer? |
|---:|---|---|---|
| **1** | **RF03** | Realizar agendamentos | É a principal finalidade do sistema. |
| **2** | **RF02** | Consultar horários disponíveis | Evita conflitos e permite realizar os agendamentos corretamente. |
| **3** | **RF01** | Cadastrar pacientes | Necessário para identificar e registrar os pacientes. |
| **4** | **RF04** | Cancelar consultas | Permite liberar horários e manter a agenda atualizada. |

## Parte B - 3 requisitos que podem ir para uma versão futura

| ID | Requisito | Impacto de adiar |
|---|---|---|
| **RF08** | Recomendar médicos utilizando IA | O sistema continuará permitindo o agendamento normalmente, apenas sem recomendações inteligentes. |
| **RF07** | Visualizar indicadores da clínica | A direção poderá inicialmente acompanhar os dados de forma manual. |
| **RQ05** | Interface personalizável para cada usuário | Não impede o uso do sistema, apenas reduz as possibilidades de personalização. |

---

# 13. Desafio - Definindo o MVP

Sim. Os requisitos classificados como **Must Have** permitem entregar uma primeira versão capaz de resolver o principal problema da clínica: **organizar os agendamentos e evitar conflitos de horários**.

O MVP seria composto principalmente por:

**Cadastro de pacientes + consulta de horários + agendamento + cancelamento + atualização da agenda em tempo real.**

Esses requisitos atacam diretamente os principais problemas encontrados no processo atual, como **conflitos de horários, informações descentralizadas e problemas com cancelamentos**.

---

# 14. Checklist MoSCoW

- [x] **Todos os requisitos possuem uma prioridade?**  
  Sim. Todos os requisitos foram classificados como Must, Should, Could ou Won't.

- [x] **Cada requisito possui apenas uma classificação?**  
  Sim. Cada requisito recebeu apenas uma categoria de prioridade.

- [x] **Os Must são realmente indispensáveis?**  
  Sim. Os requisitos classificados como Must são necessários para que o sistema cumpra seu objetivo principal.

- [x] **Existe justificativa para cada prioridade?**  
  Sim. Cada requisito possui uma justificativa de acordo com sua importância para o funcionamento do sistema.

- [x] **O grupo considerou valor para o negócio e necessidades dos stakeholders?**  
  Sim. A priorização considerou as necessidades dos pacientes, recepcionistas, médicos, gerência, direção e equipe de TI.

- [x] **Foram analisadas dependências, riscos e obrigações?**  
  Sim. Foram consideradas as dependências entre os requisitos e os riscos relacionados principalmente a conflitos de horários, cancelamentos, faltas e organização da agenda.

- [x] **Requisitos de qualidade também foram priorizados?**  
  Sim. Os requisitos de qualidade (RQ01 a RQ05) também foram classificados de acordo com sua importância para o sistema.

- [x] **Existem requisitos classificados como Could ou Won't?**  
  Sim. Existem requisitos classificados como Could, como o RF15. Não foram classificados requisitos como Won't nesta versão.

- [x] **A equipe consegue explicar o impacto de retirar cada Must?**  
  Sim. A retirada de qualquer requisito Must comprometeria o funcionamento básico do sistema e sua capacidade de organizar os agendamentos.

- [x] **A primeira versão é viável considerando as restrições do projeto?**  
  Sim. A primeira versão prioriza apenas as funcionalidades essenciais para resolver os principais problemas do processo atual.
