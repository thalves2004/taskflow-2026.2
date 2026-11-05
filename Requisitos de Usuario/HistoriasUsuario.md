# Histórias de Usuário – TaskFlow

## Introdução

Este documento apresenta as histórias de usuário do TaskFlow, descrevendo as funcionalidades do sistema sob a perspectiva de seus usuários.

## HU01 – Cadastro de usuário

**História:**

Como visitante, quero criar uma conta no sistema, para poder utilizar o TaskFlow.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF01

**Critérios de aceitação:**
- O usuário deve conseguir informar os dados necessários para cadastro.
- O sistema deve validar os dados informados.
- Após um cadastro válido, a conta deve ser criada.

## HU02 – Login

**História:**

Como usuário cadastrado, quero realizar login, para acessar minhas tarefas.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF02, RNF03

**Critérios de aceitação:**
- O usuário deve informar suas credenciais.
- O sistema deve permitir o acesso quando as credenciais forem válidas.
- O sistema deve impedir o acesso quando as credenciais forem inválidas.

## HU03 – Cadastrar tarefa

**História:**

Como usuário, quero cadastrar novas tarefas, para organizar minhas atividades.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF03, RNF01, RNF02

**Critérios de aceitação:**
- O usuário deve conseguir informar os dados da tarefa.
- O sistema deve validar os campos obrigatórios.
- Após o cadastro, a tarefa deve aparecer na lista de tarefas.

## HU04 – Editar tarefa

**História:**

Como usuário, quero editar uma tarefa existente, para manter suas informações atualizadas.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF04, RNF01

**Critérios de aceitação:**
- O usuário deve conseguir selecionar uma tarefa cadastrada.
- O sistema deve permitir alterar suas informações.
- As alterações devem aparecer ao consultar a tarefa novamente.

## HU05 – Excluir tarefa

**História:**

Como usuário, quero excluir uma tarefa, para remover atividades que não são mais necessárias.

- **Prioridade:** Média
- **Requisitos relacionados:** RF05, RNF05

**Critérios de aceitação:**
- O usuário deve conseguir selecionar uma tarefa.
- O sistema deve solicitar confirmação antes da exclusão.
- Após a confirmação, a tarefa não deve aparecer na lista.

## HU06 – Definir prioridade

**História:**

Como usuário, quero definir a prioridade de uma tarefa, para identificar quais atividades são mais importantes.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF06

**Critérios de aceitação:**
- O sistema deve oferecer as opções Alta, Média e Baixa.
- O usuário deve conseguir selecionar uma prioridade.
- A prioridade escolhida deve ser exibida na tarefa.

## HU07 – Definir prazo

**História:**

Como usuário, quero definir uma data de vencimento para uma tarefa, para organizar meus compromissos.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF07

**Critérios de aceitação:**
- O usuário deve conseguir informar uma data de vencimento.
- O sistema deve armazenar a data informada.
- A data deve aparecer nas informações da tarefa.

## HU08 – Atualizar status

**História:**

Como usuário, quero atualizar o status de uma tarefa, para acompanhar seu andamento.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF08

**Critérios de aceitação:**
- O sistema deve oferecer os status A fazer, Em andamento e Concluída.
- O usuário deve conseguir alterar o status.
- O novo status deve ser exibido na tarefa.

## HU09 – Consultar tarefas

**História:**

Como usuário, quero visualizar minhas tarefas cadastradas, para acompanhar minhas atividades.

- **Prioridade:** Alta
- **Requisitos relacionados:** RF09, RNF01, RNF02

**Critérios de aceitação:**
- O sistema deve apresentar a lista de tarefas cadastradas.
- As informações principais de cada tarefa devem ser exibidas.
- A consulta deve apresentar os dados atualizados.

## HU10 – Pesquisar tarefas

**História:**

Como usuário, quero pesquisar e filtrar minhas tarefas, para encontrar atividades específicas com facilidade.

- **Prioridade:** Média
- **Requisitos relacionados:** RF10

**Critérios de aceitação:**
- O usuário deve conseguir pesquisar tarefas.
- O sistema deve apresentar os resultados correspondentes.
- Quando não houver resultados, o sistema deve informar que nenhuma tarefa foi encontrada.

## Considerações finais

As histórias de usuário representam as principais necessidades dos usuários do TaskFlow e servirão como base para o desenvolvimento e a validação do sistema.
